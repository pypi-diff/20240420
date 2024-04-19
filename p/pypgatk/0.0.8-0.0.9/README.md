# Comparing `tmp/pypgatk-0.0.8.tar.gz` & `tmp/pypgatk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypgatk-0.0.8.tar", last modified: Tue Jan 19 17:37:43 2021, max compression
+gzip compressed data, was "pypgatk-0.0.9.tar", last modified: Wed Feb  3 20:27:43 2021, max compression
```

## Comparing `pypgatk-0.0.8.tar` & `pypgatk-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.159258 pypgatk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     5334 2021-01-19 17:37:43.159258 pypgatk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4235 2021-01-19 17:37:31.000000 pypgatk-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.151259 pypgatk-0.0.8/pypgatk/
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.151259 pypgatk-0.0.8/pypgatk/cgenomes/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/cgenomes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5848 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/cgenomes/cbioportal_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)    20721 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/cgenomes/cgenomes_proteindb.py
--rw-r--r--   0 runner    (1001) docker     (116)     6250 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/cgenomes/cosmic_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)      409 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/cgenomes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2097 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/cbioportal_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)     2509 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/cbioportal_to_proteindb.py
--rw-r--r--   0 runner    (1001) docker     (116)     1843 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/cosmic_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)     2238 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/cosmic_to_proteindb.py
--rw-r--r--   0 runner    (1001) docker     (116)     3282 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/dnaseq_to_proteindb.py
--rw-r--r--   0 runner    (1001) docker     (116)      992 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/ensembl_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     4904 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/ensembl_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)     4628 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/proteindb_decoy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/threeframe_translation.py
--rw-r--r--   0 runner    (1001) docker     (116)      664 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5797 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/commands/vcf_to_proteindb.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/config/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/db/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4502 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/db/digest_mutant_protein.py
--rw-r--r--   0 runner    (1001) docker     (116)    10779 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/db/map_peptide2genome.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/ensembl/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/ensembl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17823 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/ensembl/data_downloader.py
--rw-r--r--   0 runner    (1001) docker     (116)    32937 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/ensembl/ensembl.py
--rw-r--r--   0 runner    (1001) docker     (116)      377 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/ensembl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     8051 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/ensembl/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/proteomics/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/proteomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/proteomics/db/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/proteomics/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14582 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/proteomics/db/decoy_pyrat.py
--rw-r--r--   0 runner    (1001) docker     (116)     1834 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/pypgatk_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9434 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/tests/pypgatk_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.155259 pypgatk-0.0.8/pypgatk/toolbox/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      771 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/toolbox/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    12019 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/toolbox/general.py
--rw-r--r--   0 runner    (1001) docker     (116)      988 2021-01-19 17:37:31.000000 pypgatk-0.0.8/pypgatk/toolbox/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:37:43.151259 pypgatk-0.0.8/pypgatk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5334 2021-01-19 17:37:42.000000 pypgatk-0.0.8/pypgatk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1438 2021-01-19 17:37:43.000000 pypgatk-0.0.8/pypgatk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 17:37:42.000000 pypgatk-0.0.8/pypgatk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-19 17:37:42.000000 pypgatk-0.0.8/pypgatk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 17:37:42.000000 pypgatk-0.0.8/pypgatk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      497 2021-01-19 17:37:42.000000 pypgatk-0.0.8/pypgatk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-19 17:37:42.000000 pypgatk-0.0.8/pypgatk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-19 17:37:43.159258 pypgatk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1730 2021-01-19 17:37:31.000000 pypgatk-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.869448 pypgatk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (117)     5813 2021-02-03 20:27:43.869448 pypgatk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     4682 2021-02-03 20:27:31.000000 pypgatk-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/
+-rw-r--r--   0 runner    (1001) docker     (117)       17 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/cgenomes/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/cgenomes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)     5848 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/cgenomes/cbioportal_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (117)    20375 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/cgenomes/cgenomes_proteindb.py
+-rw-r--r--   0 runner    (1001) docker     (117)     6783 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/cgenomes/cosmic_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (117)      409 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/cgenomes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/commands/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)     2061 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/cbioportal_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (117)     2489 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/cbioportal_to_proteindb.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1778 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/cosmic_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (117)     2219 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/cosmic_to_proteindb.py
+-rw-r--r--   0 runner    (1001) docker     (117)     3251 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/dnaseq_to_proteindb.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1298 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/ensembl_database.py
+-rw-r--r--   0 runner    (1001) docker     (117)     4989 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/ensembl_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (117)     4614 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/proteindb_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1183 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/threeframe_translation.py
+-rw-r--r--   0 runner    (1001) docker     (117)      664 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (117)     5780 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/commands/vcf_to_proteindb.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/config/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/db/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)     4501 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/db/digest_mutant_protein.py
+-rw-r--r--   0 runner    (1001) docker     (117)    10769 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/db/map_peptide2genome.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/ensembl/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/ensembl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)    17977 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/ensembl/data_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (117)    31139 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/ensembl/ensembl.py
+-rw-r--r--   0 runner    (1001) docker     (117)      377 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/ensembl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (117)     8051 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/ensembl/models.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/proteomics/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/proteomics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk/proteomics/db/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/proteomics/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)    14571 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/proteomics/db/decoy_pyrat.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1834 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/pypgatk_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.869448 pypgatk-0.0.9/pypgatk/tests/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)      163 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/tests/ensembl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (117)    10316 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/tests/pypgatk_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.869448 pypgatk-0.0.9/pypgatk/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)      771 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/toolbox/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (117)    12019 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/toolbox/general.py
+-rw-r--r--   0 runner    (1001) docker     (117)      988 2021-02-03 20:27:31.000000 pypgatk-0.0.9/pypgatk/toolbox/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 20:27:43.865448 pypgatk-0.0.9/pypgatk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (117)     5813 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     1469 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       58 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (117)      497 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        8 2021-02-03 20:27:43.000000 pypgatk-0.0.9/pypgatk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       38 2021-02-03 20:27:43.869448 pypgatk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (117)     1730 2021-02-03 20:27:31.000000 pypgatk-0.0.9/setup.py
```

### Comparing `pypgatk-0.0.8/PKG-INFO` & `pypgatk-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pypgatk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python tools for proteogenomics
 Home-page: http://github.com/bigbio/py-pgatk
 Author: PgAtk Team
 Author-email: ypriverol@gmail.com
 License: LICENSE.txt
 Description: # Python tools for ProteoGenomics Analysis Toolkit
         
         
         ![Python application](https://github.com/bigbio/py-pgatk/workflows/Python%20application/badge.svg)
         [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pypgatk/README.html)
-        
+        [![Codacy Badge](https://app.codacy.com/project/badge/Grade/f6d030fd7d69413987f7265a01193324)](https://www.codacy.com/gh/bigbio/py-pgatk/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bigbio/py-pgatk&amp;utm_campaign=Badge_Grade)
+        [![PyPI version](https://badge.fury.io/py/pypgatk.svg)](https://badge.fury.io/py/pypgatk)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dm/pypgatk)
         
         **pypgatk** is a Python library part of the [ProteoGenomics Analysis Toolkit](https://pgatk.readthedocs.io/en/latest). It provides different bioinformatics tools for proteogenomics data analysis.
         
         # Requirements:
         
         This package requirements vary depending on the way that you want to install it (all three are independent, you don't need all these requirements):
         
@@ -103,11 +105,13 @@
           vcf-to-proteindb         Generate peptides based on DNA variants from
                                    ENSEMBL VEP VCF files
         
         ```
         
         The library provides multiple commands to download, translate and generate protein sequence databases from reference and mutation genome databases.
         
-        ### Please read full docs here: <https://pgatk.readthedocs.io/en/latest/pypgatk.html>
+        # Full Documentation
+        
+        [https://pgatk.readthedocs.io/en/latest/pypgatk.html](https://pgatk.readthedocs.io/en/latest/pypgatk.html)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pypgatk-0.0.8/README.md` & `pypgatk-0.0.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Python tools for ProteoGenomics Analysis Toolkit
 
 
 ![Python application](https://github.com/bigbio/py-pgatk/workflows/Python%20application/badge.svg)
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pypgatk/README.html)
-
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/f6d030fd7d69413987f7265a01193324)](https://www.codacy.com/gh/bigbio/py-pgatk/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bigbio/py-pgatk&amp;utm_campaign=Badge_Grade)
+[![PyPI version](https://badge.fury.io/py/pypgatk.svg)](https://badge.fury.io/py/pypgatk)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pypgatk)
 
 **pypgatk** is a Python library part of the [ProteoGenomics Analysis Toolkit](https://pgatk.readthedocs.io/en/latest). It provides different bioinformatics tools for proteogenomics data analysis.
 
 # Requirements:
 
 This package requirements vary depending on the way that you want to install it (all three are independent, you don't need all these requirements):
 
@@ -95,8 +97,10 @@
   vcf-to-proteindb         Generate peptides based on DNA variants from
                            ENSEMBL VEP VCF files
 
 ```
 
 The library provides multiple commands to download, translate and generate protein sequence databases from reference and mutation genome databases.
 
-### Please read full docs here: <https://pgatk.readthedocs.io/en/latest/pypgatk.html>
+# Full Documentation
+
+[https://pgatk.readthedocs.io/en/latest/pypgatk.html](https://pgatk.readthedocs.io/en/latest/pypgatk.html)
```

### Comparing `pypgatk-0.0.8/pypgatk/cgenomes/cbioportal_downloader.py` & `pypgatk-0.0.9/pypgatk/cgenomes/cbioportal_downloader.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk/cgenomes/cgenomes_proteindb.py` & `pypgatk-0.0.9/pypgatk/cgenomes/cgenomes_proteindb.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     CONFIG_COSMIC_DATA = "cosmic_data"
     CONFIG_KEY_DATA = 'proteindb'
     CONFIG_FILTER_INFO = 'filter_info'
     FILTER_COLUMN = "filter_column"
     ACCEPTED_VALUES = "accepted_values"
     SPLIT_BY_FILTER_COLUMN = "split_by_filter_column"
     CLINICAL_SAMPLE_FILE = 'clinical_sample_file'
-    
+
     def __init__(self, config_file, pipeline_arguments):
         """
         Init the class with the specific parameters.
         :param config_file configuration file
         :param pipeline_arguments pipelines arguments
         """
         super(CancerGenomesService, self).__init__(self.CONFIG_COSMIC_DATA, config_file, pipeline_arguments)
@@ -30,32 +30,32 @@
             self._local_mutation_file = self.get_pipeline_parameters()[self.CONFIG_CANCER_GENOMES_MUTATION_FILE]
 
         if self.CONFIG_COMPLETE_GENES_FILE in self.get_pipeline_parameters():
             self._local_complete_genes = self.get_pipeline_parameters()[self.CONFIG_COMPLETE_GENES_FILE]
 
         if self.CONFIG_OUTPUT_FILE in self.get_pipeline_parameters():
             self._local_output_file = self.get_pipeline_parameters()[self.CONFIG_OUTPUT_FILE]
-        
+
         self._filter_column = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_FILTER_INFO][self.FILTER_COLUMN]
         if self.FILTER_COLUMN in self.get_pipeline_parameters():
             self._filter_column = self.get_pipeline_parameters()[self.FILTER_COLUMN]
 
         self._accepted_values = self.get_multiple_options(
             self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_FILTER_INFO][self.ACCEPTED_VALUES])
         if self.ACCEPTED_VALUES in self.get_pipeline_parameters():
             self._accepted_values = self.get_multiple_options(self.get_pipeline_parameters()[self.ACCEPTED_VALUES])
 
         self._split_by_filter_column = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_FILTER_INFO][self.SPLIT_BY_FILTER_COLUMN]
         if self.SPLIT_BY_FILTER_COLUMN in self.get_pipeline_parameters():
             self._split_by_filter_column = self.get_pipeline_parameters()[self.SPLIT_BY_FILTER_COLUMN]
-        
+
         self._local_clinical_sample_file = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_FILTER_INFO][self.CLINICAL_SAMPLE_FILE]
         if self.CLINICAL_SAMPLE_FILE in self.get_pipeline_parameters():
             self._local_clinical_sample_file = self.get_pipeline_parameters()[self.CLINICAL_SAMPLE_FILE]
-    
+
     @staticmethod
     def get_multiple_options(options_str: str):
         """
         This method takes an String like option1, option2, ... and produce and array [option1, option2,... ]
         :param options_str:
         :return: Array
         """
@@ -125,27 +125,27 @@
                     except ValueError:
                         return ''
                     mut_aa = snp.aa_mut[index + 1:]
                     if "deletion" in snp.type:
                         del_index1 = int(positions[0]) - 1
                         del_index2 = int(positions[1])
                         mut_pro_seq = protein_seq[:del_index1] + mut_aa + protein_seq[del_index2:]
-                        
+
                     elif "insertion" in snp.type:
                         ins_index1 = int(positions[0]) - 1
                         mut_pro_seq = protein_seq[:ins_index1] + mut_aa + protein_seq[ins_index1 + 1:]
                     elif "compound substitution" in snp.type:
                         if "*" not in mut_aa:
                             del_index1 = int(positions[0]) - 1
                             del_index2 = int(positions[1])
                             mut_pro_seq = protein_seq[:del_index1] + mut_aa + protein_seq[del_index2:]
                         else:
                             del_index1 = int(positions[0]) - 1
                             mut_pro_seq = protein_seq[:del_index1] + mut_aa.replace("*", "")
-                            
+
         return mut_pro_seq
 
 
     def cosmic_to_proteindb(self):
         """
         This function translate the mutation file + COSMIC genes into a protein Fasta database. The
         method write into the file system the output Fasta.
@@ -154,28 +154,28 @@
         self.get_logger().debug("Starting reading the All cosmic genes")
         COSMIC_CDS_DB = {}
         for record in SeqIO.parse(self._local_complete_genes, 'fasta'):
             try:
                 COSMIC_CDS_DB[record.id].append(record)
             except KeyError:
                 COSMIC_CDS_DB[record.id] = [record]
-        
+
         cosmic_input = open(self._local_mutation_file, encoding="latin-1")  # CosmicMutantExport.tsv
 
         header = cosmic_input.readline().split("\t")
         regex = re.compile('[^a-zA-Z]')
         gene_col = header.index("Gene name")
         enst_col = header.index("Accession Number")
         cds_col = header.index("Mutation CDS")
         aa_col = header.index("Mutation AA")
         muttype_col = header.index("Mutation Description")
         filter_col = None
         if self._filter_column:
             filter_col = header.index(self._filter_column)
-        
+
         output = open(self._local_output_file, 'w')
 
         mutation_dic = {}
         groups_mutations_dict = {}
         self.get_logger().debug("Reading input CosmicMutantExport.tsv ...")
         line_counter = 1
         for line in cosmic_input:
@@ -184,73 +184,73 @@
                 self.get_logger().debug(msg)
             line_counter += 1
             row = line.strip().split("\t")
             #filter out mutations from unspecified groups
             if filter_col:
                 if row[filter_col] not in self._accepted_values and self._accepted_values!=['all']:
                     continue
-            
+
             if "coding silent" in row[muttype_col]:
                 continue
 
             snp = SNP(gene=row[gene_col], mrna=row[enst_col], dna_mut=row[cds_col], aa_mut=row[aa_col],
                       type=row[muttype_col])
             header = "COSMIC:%s:%s:%s" % (snp.gene, snp.aa_mut, snp.type.replace(" ", ""))
             try:
                 this_gene_records  = COSMIC_CDS_DB[snp.gene]
                 seqs = []
                 for record in this_gene_records:
                     seqs.append(record.seq)
-                 
+
             except KeyError:  # geneID is not in All_COSMIC_Genes.fasta
                 continue
-            
+
             for seq in seqs:
                 try:
                     mut_pro_seq = self.get_mut_pro_seq(snp, seq)
                 except IndexError:
                     continue
                 if mut_pro_seq:
                     break
-            
+
             if mut_pro_seq:
                 entry = ">%s\n%s\n" % (header, mut_pro_seq)
                 if header not in mutation_dic:
                     output.write(entry)
                     mutation_dic[header] = 1
-                
+
                 if self._split_by_filter_column and filter_col:
                     try:
                         groups_mutations_dict[row[filter_col]][header] = entry
                     except KeyError:
                         groups_mutations_dict[row[filter_col]] = {header: entry}
-            
+
         for group_name in groups_mutations_dict.keys():
             with open(self._local_output_file.replace('.fa', '')+ '_' + regex.sub('', group_name) +'.fa', 'w') as fn:
                 for header in groups_mutations_dict[group_name].keys():
                     fn.write(groups_mutations_dict[group_name][header])
-            
+
         self.get_logger().debug("COSMIC contains in total {} non redundant mutations".format(len(mutation_dic)))
         cosmic_input.close()
         output.close()
-    
+
     @staticmethod
     def get_sample_headers(header_line):
         try:
             tissue_type_col = header_line.index('CANCER_TYPE')
         except ValueError:
             print('CANCER_TYPE was not found in the header row:', header_line)
             return None, None
         try:
             sample_id_col = header_line.index('SAMPLE_ID')
         except ValueError:
             print('SAMPLE_ID was not found in the header row:', header_line)
             return None, None
         return tissue_type_col, sample_id_col
-    
+
     def get_tissue_type_per_sample(self, local_clinical_sample_file):
         sample_tissue_type = {}
         if local_clinical_sample_file:
             with open(local_clinical_sample_file, 'r') as clin_fn:
                 tissue_type_col, sample_id_col = None, None
                 for line in clin_fn.readlines():
                     if line.startswith('#'):
@@ -258,64 +258,64 @@
                     sl = line.strip().split('\t')
                     #check for header and re-assign columns
                     if 'SAMPLE_ID' in sl and 'CANCER_TYPE' in sl:
                         tissue_type_col, sample_id_col = self.get_sample_headers(sl)
                     if tissue_type_col and sample_id_col:
                         sample_tissue_type[sl[sample_id_col]] = sl[tissue_type_col].strip().replace(' ','_')
         return sample_tissue_type
-    
+
     @staticmethod
     def get_mut_header_cols(header_cols, row, filter_column, accepted_values, split_by_filter_column):
         for col in header_cols.keys():
             header_cols[col] = row.index(col)
-        
+
         #check if (filter_column) tissue type should be considered
         if accepted_values!=['all'] or split_by_filter_column:
             try:
                 header_cols[filter_column] = row.index(filter_column)
             except ValueError:
                 print("{} was not found in the header {} of mutations file".format(filter_column, row))
                 header_cols[filter_column] = None
-        
+
         return header_cols
-    
+
     def cbioportal_to_proteindb(self):
-        """cBioportal studies have a data_clinical_sample.txt file 
+        """cBioportal studies have a data_clinical_sample.txt file
         that shows the Primary Tumor Site per Sample Identifier
         it matches the the (filter_column) Tumor_Sample_Barcode column in the mutations file.
         """
         regex = re.compile('[^a-zA-Z]')
         mutfile = open(self._local_mutation_file, "r")
         fafile = SeqIO.parse(self._local_complete_genes, "fasta")
         output = open(self._local_output_file, "w")
         sample_groups_dict = {}
         group_mutations_dict = {}
-        
+
         seq_dic = {}
         for record in fafile:
             newacc = record.id.split(".")[0]
             if newacc not in seq_dic:
                 seq_dic[newacc] = record.seq
-        
-        header_cols = {"HGVSc": None, "Transcript_ID": None, "Variant_Classification": None, 
+
+        header_cols = {"HGVSc": None, "Transcript_ID": None, "Variant_Classification": None,
                        "Variant_Type": None, "HGVSp_Short": None}
         nucleotide = ["A", "T", "C", "G"]
         mutclass = ["Frame_Shift_Del", "Frame_Shift_Ins", "In_Frame_Del", "In_Frame_Ins", "Missense_Mutation",
                     "Nonsense_Mutation"]
-        
+
         # check if sample id and clinical files are given, if not and tissue type is required then exit
         if self._accepted_values!=['all'] or self._split_by_filter_column:
             if self._local_clinical_sample_file:
                 sample_groups_dict = self.get_tissue_type_per_sample(self._local_clinical_sample_file)
                 if sample_groups_dict=={}:
                     return
             else:
                 print('No clinical sample file is given therefore no tissue type can be detected.')
                 return
-            
+
         for i,line in enumerate(mutfile):
             row = line.strip().split("\t")
             if row[0]=='#':
                 print("skipping line ({}): {}".format(i, row))
                 continue
             #check for header in the mutations file and get column indecis
             if set(header_cols.keys()).issubset(set(row)):
@@ -333,15 +333,15 @@
                     if self._accepted_values!=['all'] or self._split_by_filter_column:
                         print("No clinical info was found for sample {}. Skipping (line {}): {}".format(row[header_cols[self._filter_column]], i, line))
                         continue
                 except IndexError:
                     print("No sampleID was found in (line {}): {}".format(i, row))
             if group not in self._accepted_values and self._accepted_values != ['all']:
                 continue
-            
+
             gene = row[0]
             try:
                 pos = row[header_cols["HGVSc"]]
                 enst = row[header_cols["Transcript_ID"]]
 
                 seq_mut = ""
                 aa_mut = row[header_cols["HGVSp_Short"]]
@@ -349,21 +349,21 @@
                 vartype = row[header_cols["Variant_Type"]]
                 varclass = row[header_cols["Variant_Classification"]]
             except IndexError:
                 print("Incorrect line (i):", row)
                 continue
             if varclass not in mutclass:
                 continue
-            
+
             try:
                 seq = seq_dic[enst]
             except KeyError:
                 print("%s not found:" % enst)
                 continue
-            
+
             if ":" in pos:
                 cdna_pos = pos.split(":")[1]
             else:
                 cdna_pos = pos
 
             if vartype == "SNP":
                 try:
@@ -407,34 +407,34 @@
                     ins_dna = pos.split("ins")[1]
                 elif "dup" in pos:
                     ins_dna = pos.split("dup")[1]
                     if len(ins_dna) > 1:
                         enst_pos = int(re.findall(r'\d+', cdna_pos.split("_")[1])[0])
                 else:
                     print("unexpected insertion format")
-                    continue;
+                    continue
 
                 seq_mut = seq[:enst_pos] + ins_dna + seq[enst_pos:]
 
             if seq_mut == "":
-                continue;
+                continue
 
             mut_pro_seq = seq_mut.translate(to_stop=True)
             if len(mut_pro_seq) > 6:
                 header = "cbiomut:%s:%s:%s:%s" % (enst, gene, aa_mut, varclass)
                 output.write(">%s\n%s\n" % (header, mut_pro_seq))
-                
+
                 if self._split_by_filter_column:
                     try:
                         group_mutations_dict[group][header] = mut_pro_seq
                     except KeyError:
                         group_mutations_dict[group] = {header: mut_pro_seq}
-                    
+
         output.close()
         mutfile.close()
         fafile.close()
-        
+
         for group in group_mutations_dict.keys():
             with open(self._local_output_file.replace('.fa', '')+ '_' + regex.sub('', group) +'.fa', 'w') as fn:
                 for header in group_mutations_dict[group].keys():
                     fn.write(">{}\n{}\n".format(header, group_mutations_dict[group][header]))
-         
+
```

### Comparing `pypgatk-0.0.8/pypgatk/cgenomes/cosmic_downloader.py` & `pypgatk-0.0.9/pypgatk/cgenomes/cosmic_downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,133 @@
 import base64
 import json
 
 import requests
 
+from pypgatk.toolbox.exceptions import AppConfigException
 from pypgatk.toolbox.general import ParameterConfiguration, check_create_folders
 
 
 class CosmicDownloadService(ParameterConfiguration):
-    CONFIG_KEY_DATA_DOWNLOADER = 'cosmic_data'
-    CONFIG_OUTPUT_DIRECTORY = 'output_directory'
-    CONFIG_COSMIC_SERVER = 'cosmic_server'
-    CONFIG_COSMIC_FTP_URL = 'cosmic_ftp'
-    CONFIG_COSMIC_FTP_USER = "cosmic_user"
-    CONFIG_COSMIC_FTP_PASSWORD = "cosmic_password"
-    CONFIG_COSMIC_MUTATIONS_URL = "mutations_url"
-    CONFIG_COSMIC_MUTATIONS_FILE = "mutations_file"
-    CONFIG_COSMIC_CELLLINE_MUTATIONS_URL = "mutations_cellline_url"
-    CONFIG_COSMIC_CELLLINE_MUTATIONS_FILE = "mutations_cellline_file"
-    CONFIG_COSMIC_CDS_GENES_FILE = "all_cds_genes_file"
-    CONFIG_COSMIC_CELLLINES_GENES_FILE = "all_celllines_genes_file"
+  CONFIG_KEY_DATA_DOWNLOADER = 'cosmic_data'
+  CONFIG_OUTPUT_DIRECTORY = 'output_directory'
+  CONFIG_COSMIC_SERVER = 'cosmic_server'
+  CONFIG_COSMIC_FTP_URL = 'cosmic_ftp'
+  CONFIG_COSMIC_FTP_USER = "cosmic_user"
+  CONFIG_COSMIC_FTP_PASSWORD = "cosmic_password"
+  CONFIG_COSMIC_MUTATIONS_URL = "mutations_url"
+  CONFIG_COSMIC_MUTATIONS_FILE = "mutations_file"
+  CONFIG_COSMIC_CELLLINE_MUTATIONS_URL = "mutations_cellline_url"
+  CONFIG_COSMIC_CELLLINE_MUTATIONS_FILE = "mutations_cellline_file"
+  CONFIG_COSMIC_CDS_GENES_FILE = "all_cds_genes_file"
+  CONFIG_COSMIC_CELLLINES_GENES_FILE = "all_celllines_genes_file"
 
-
-    def __init__(self, config_file, pipeline_arguments):
-        """
+  def __init__(self, config_file, pipeline_arguments):
+    """
         Init the class with the specific parameters.
         :param config_file configuration file
         :param pipeline_arguments pipelines arguments
         """
-        super(CosmicDownloadService, self).__init__(self.CONFIG_KEY_DATA_DOWNLOADER, config_file, pipeline_arguments)
+    super(CosmicDownloadService, self).__init__(self.CONFIG_KEY_DATA_DOWNLOADER, config_file, pipeline_arguments)
 
-        if self.CONFIG_OUTPUT_DIRECTORY in self.get_pipeline_parameters():
-            self._local_path_cosmic = self.get_pipeline_parameters()[self.CONFIG_OUTPUT_DIRECTORY]
-        else:
-            self._local_path_cosmic = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
-                self.CONFIG_OUTPUT_DIRECTORY]
-
-        self._cosmic_token = base64.b64encode("{}:{}".format(self.get_pipeline_parameters()[self.CONFIG_COSMIC_FTP_USER], self.get_pipeline_parameters()[self.CONFIG_COSMIC_FTP_PASSWORD])
-                                              .encode()).decode('utf-8')
-
-        self.prepare_local_cosmic_repository()
-
-    def prepare_local_cosmic_repository(self):
-        self.get_logger().debug("Preparing local cbioportal repository, root folder - '{}'".format(
-            self.get_local_path_root_cosmic_repo()))
-        check_create_folders([self.get_local_path_root_cosmic_repo()])
-        self.get_logger().debug(
-            "Local path for cbioportal Release - '{}'".format(self.get_local_path_root_cosmic_repo()))
+    if self.CONFIG_OUTPUT_DIRECTORY in self.get_pipeline_parameters():
+      self._local_path_cosmic = self.get_pipeline_parameters()[self.CONFIG_OUTPUT_DIRECTORY]
+    else:
+      self._local_path_cosmic = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
+        self.CONFIG_OUTPUT_DIRECTORY]
+
+    self._cosmic_token = base64.b64encode("{}:{}".format(self.get_pipeline_parameters()[self.CONFIG_COSMIC_FTP_USER],
+                                                         self.get_pipeline_parameters()[
+                                                           self.CONFIG_COSMIC_FTP_PASSWORD])
+                                          .encode()).decode('utf-8')
+
+    self.prepare_local_cosmic_repository()
+
+  def prepare_local_cosmic_repository(self):
+    self.get_logger().debug("Preparing local cbioportal repository, root folder - '{}'".format(
+      self.get_local_path_root_cosmic_repo()))
+    check_create_folders([self.get_local_path_root_cosmic_repo()])
+    self.get_logger().debug(
+      "Local path for cbioportal Release - '{}'".format(self.get_local_path_root_cosmic_repo()))
 
-    def get_local_path_root_cosmic_repo(self):
-        return self._local_path_cosmic
+  def get_local_path_root_cosmic_repo(self):
+    return self._local_path_cosmic
 
-    def download_mutation_file(self):
-        """
+  def download_mutation_file(self):
+    """
         This function will download the mutations file from Cosmic Database.
         :return: None
         """
 
-        mutation_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(), self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_MUTATIONS_FILE])
-        cds_genes_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(), self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_CDS_GENES_FILE])
-        
-        mutation_celline_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(), self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_CELLLINE_MUTATIONS_FILE])
-        cellines_genes_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(), self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_CELLLINES_GENES_FILE])
-        
-        server = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-            self.CONFIG_COSMIC_FTP_URL]
-
-        cosmic_version = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-            self.CONFIG_COSMIC_MUTATIONS_URL]
-        mutation_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-            self.CONFIG_COSMIC_MUTATIONS_FILE]
-
-        cosmic_cellline_version = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-          self.CONFIG_COSMIC_CELLLINE_MUTATIONS_URL]
-        mutation_celline_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-          self.CONFIG_COSMIC_CELLLINE_MUTATIONS_FILE]
-
-        all_cds_gene_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-            self.CONFIG_COSMIC_CDS_GENES_FILE]
-
-        all_celllines_gene_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
-            self.CONFIG_COSMIC_CELLLINES_GENES_FILE]
-        
-        mutation_url = "{}/{}/{}".format(server, cosmic_version, mutation_file)
-        cds_gene_url = "{}/{}/{}".format(server, cosmic_version, all_cds_gene_file)
-        
-        celllines_gene_url = "{}/{}/{}".format(server, cosmic_cellline_version, all_celllines_gene_file)
-        mutation_cellline_url = "{}/{}/{}".format(server, cosmic_cellline_version, mutation_celline_file)
-        
-        token = "Basic {}".format(self._cosmic_token)
-        self.download_file_cosmic(mutation_url, mutation_output_file, token)
-        self.download_file_cosmic(cds_gene_url, cds_genes_output_file, token)
-        
-        self.download_file_cosmic(celllines_gene_url, cellines_genes_output_file, token)
-        self.download_file_cosmic(mutation_cellline_url, mutation_celline_output_file, token)
-        
+    mutation_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(),
+                                          self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
+                                            self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_MUTATIONS_FILE])
+    cds_genes_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(),
+                                           self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
+                                             self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_CDS_GENES_FILE])
+
+    mutation_celline_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(),
+                                                  self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
+                                                    self.CONFIG_COSMIC_SERVER][
+                                                    self.CONFIG_COSMIC_CELLLINE_MUTATIONS_FILE])
+    cellines_genes_output_file = "{}/{}".format(self.get_local_path_root_cosmic_repo(),
+                                                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
+                                                  self.CONFIG_COSMIC_SERVER][self.CONFIG_COSMIC_CELLLINES_GENES_FILE])
+
+    server = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_FTP_URL]
+
+    cosmic_version = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_MUTATIONS_URL]
+    mutation_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_MUTATIONS_FILE]
+
+    cosmic_cellline_version = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_CELLLINE_MUTATIONS_URL]
+    mutation_celline_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_CELLLINE_MUTATIONS_FILE]
+
+    all_cds_gene_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_CDS_GENES_FILE]
+
+    all_celllines_gene_file = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_COSMIC_SERVER][
+      self.CONFIG_COSMIC_CELLLINES_GENES_FILE]
+
+    mutation_url = "{}/{}/{}".format(server, cosmic_version, mutation_file)
+    cds_gene_url = "{}/{}/{}".format(server, cosmic_version, all_cds_gene_file)
+
+    celllines_gene_url = "{}/{}/{}".format(server, cosmic_cellline_version, all_celllines_gene_file)
+    mutation_cellline_url = "{}/{}/{}".format(server, cosmic_cellline_version, mutation_celline_file)
+
+    token = "Basic {}".format(self._cosmic_token)
+    self.download_file_cosmic(mutation_url, mutation_output_file, token)
+    self.download_file_cosmic(cds_gene_url, cds_genes_output_file, token)
 
-    def download_file_cosmic(self, url, local_file, token):
-        """
+    self.download_file_cosmic(celllines_gene_url, cellines_genes_output_file, token)
+    self.download_file_cosmic(mutation_cellline_url, mutation_celline_output_file, token)
+
+  def download_file_cosmic(self, url, local_file, token):
+    """
         Download file from cosmic repository using requests
         :param url: url of the file to be download
         :param local_file: local file
         :param token: token to be used
         :return:
         """
 
-        response = requests.get(url, stream=True, headers={'Authorization': token})
-        if response.status_code == 200:
-            url = json.loads(response.text)['url']
-            msg = "Downloading file from url '{}'".format(url)
-            self.get_logger().debug(msg)
-
-            response = requests.get(url, stream=True)
-            if response.status_code == 200:
-                with open(local_file, 'wb') as f:
-                    f.write(response.content)
-                    msg = "Download Finish for file '{}'".format(local_file)
-                    self.get_logger().debug(msg)
+    response = requests.get(url, stream=True, headers={'Authorization': token})
+    if response.status_code == 200:
+      url = json.loads(response.text)['url']
+      msg = "Downloading file from url '{}'".format(url)
+      self.get_logger().debug(msg)
+
+      response = requests.get(url, stream=True)
+      if response.status_code == 200:
+        with open(local_file, 'wb') as f:
+          f.write(response.content)
+          msg = "Download Finish for file '{}'".format(local_file)
+          self.get_logger().debug(msg)
+    else:
+      msg = "Error downloading the COSMIC data, error code {} , error message '{}'".format(response.status_code,
+                                                                                           local_file)
+      self.get_logger().debug(msg)
+      raise AppConfigException(msg)
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/cbioportal_downloader.py` & `pypgatk-0.0.9/pypgatk/commands/cbioportal_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,42 @@
 import click
 
 from pypgatk.cgenomes.cbioportal_downloader import CbioPortalDownloadService
 from pypgatk.toolbox.exceptions import AppConfigException
 
 this_dir, this_filename = os.path.split(__file__)
 
+
 @click.command('cbioportal-downloader', short_help=' Command to download the the cbioportal studies')
-@click.option('--config_file', '-c', help='Configuration file for the ensembl data downloader pipeline',
-              default=this_dir + '../config/cbioportal_config.yaml')
-@click.option('--output_directory', '-o', help='Output directory for the peptide databases',
+@click.option('-c', '--config_file', help='Configuration file for the ensembl data downloader pipeline',
+              default=this_dir + '/../config/cbioportal_config.yaml')
+@click.option('-o', '--output_directory', help='Output directory for the peptide databases',
               default="./database_cbioportal/")
-@click.option('--list_studies', '-l',
+@click.option('-l', '--list_studies',
               help='Print the list of all the studies in cBioPortal (https://www.cbioportal.org)', is_flag=True)
-@click.option('--download_study', '-d',
+@click.option('-d', '--download_study',
               help="Download a specific Study from cBioPortal -- (all to download all studies)")
-@click.option('--multithreading', '-th', help=' Enable multithreading to download multiple files ad the same time', is_flag=True)
+@click.option('-th', '--multithreading', help=' Enable multithreading to download multiple files ad the same time',
+              is_flag=True)
 @click.pass_context
 def cbioportal_downloader(ctx, config_file, output_directory, list_studies, download_study, multithreading):
-    if config_file is None:
-        msg = "The config file for the pipeline is missing, please provide one "
-        logging.error(msg)
-        raise AppConfigException(msg)
-
-    pipeline_arguments = {}
-    if output_directory is not None:
-        pipeline_arguments[CbioPortalDownloadService.CONFIG_OUTPUT_DIRECTORY] = output_directory
-    if list_studies:
-        pipeline_arguments[CbioPortalDownloadService.CONFIG_LIST_STUDIES] = list_studies
-    if multithreading is not None:
-        pipeline_arguments[CbioPortalDownloadService.CONFIG_MULTITHREADING] = multithreading
-
-    cbioportal_downloader_service = CbioPortalDownloadService(config_file, pipeline_arguments)
-
-    if list_studies:
-        list_of_studies = cbioportal_downloader_service.get_cancer_studies()
-        print(list_of_studies)
+  if config_file is None:
+    msg = "The config file for the pipeline is missing, please provide one "
+    logging.error(msg)
+    raise AppConfigException(msg)
+
+  pipeline_arguments = {}
+  if output_directory is not None:
+    pipeline_arguments[CbioPortalDownloadService.CONFIG_OUTPUT_DIRECTORY] = output_directory
+  if list_studies:
+    pipeline_arguments[CbioPortalDownloadService.CONFIG_LIST_STUDIES] = list_studies
+  if multithreading is not None:
+    pipeline_arguments[CbioPortalDownloadService.CONFIG_MULTITHREADING] = multithreading
+
+  cbioportal_downloader_service = CbioPortalDownloadService(config_file, pipeline_arguments)
+
+  if list_studies:
+    list_of_studies = cbioportal_downloader_service.get_cancer_studies()
+    print(list_of_studies)
 
-    if download_study is not None:
-        cbioportal_downloader_service.download_study(download_study)
+  if download_study is not None:
+    cbioportal_downloader_service.download_study(download_study)
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/cbioportal_to_proteindb.py` & `pypgatk-0.0.9/pypgatk/commands/cbioportal_to_proteindb.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 import click
 
 from pypgatk.cgenomes.cgenomes_proteindb import CancerGenomesService
 from pypgatk.commands.utils import print_help
 
 this_dir, this_filename = os.path.split(__file__)
 
+
 @click.command('cbioportal-to-proteindb', short_help='Command to translate cbioportal mutation data into proteindb')
-@click.option('--config_file',
-              '-c',
+@click.option('-c', '--config_file',
               help='Configuration for cbioportal to proteindb tool',
-              default= this_dir + '../config/cbioportal_config.yaml')
+              default=this_dir + '/../config/cbioportal_config.yaml')
 @click.option('-in', '--input_mutation', help='Cbioportal mutation file')
 @click.option('-fa', '--input_cds', help='CDS genes from ENSEMBL database')
 @click.option('-out', '--output_db', help='Protein database including all the mutations')
-@click.option('-f',   '--filter_column', default='Tumor_Sample_Barcode', 
+@click.option('-f', '--filter_column', default='Tumor_Sample_Barcode',
               help='Column in the VCF file to be used for filtering or splitting mutations')
-@click.option('-a',   '--accepted_values', default='all', 
+@click.option('-a', '--accepted_values', default='all',
               help='Limit mutations to values (tissue type, sample name, etc) considered for generating proteinDBs, by default mutations from all records are considered')
-@click.option('-s',   '--split_by_filter_column', 
-              help='Use this flag to generate a proteinDB per group as specified in the filter_column, default is False', is_flag=True)
-@click.option('-cl', '--clinical_sample_file', help='File to get tissue type from for the samples in input_mutation file')
-
+@click.option('-s', '--split_by_filter_column',
+              help='Use this flag to generate a proteinDB per group as specified in the filter_column, default is False',
+              is_flag=True)
+@click.option('-cl', '--clinical_sample_file',
+              help='File to get tissue type from for the samples in input_mutation file')
 @click.pass_context
-def cbioportal_to_proteindb(ctx, config_file, input_mutation, input_cds, output_db, 
+def cbioportal_to_proteindb(ctx, config_file, input_mutation, input_cds, output_db,
                             clinical_sample_file, filter_column, accepted_values, split_by_filter_column):
-    if input_mutation is None or input_cds is None or output_db is None:
-        print_help()
+  if input_mutation is None or input_cds is None or output_db is None:
+    print_help()
 
-    pipeline_arguments = {CancerGenomesService.CONFIG_CANCER_GENOMES_MUTATION_FILE: input_mutation,
-                          CancerGenomesService.CONFIG_COMPLETE_GENES_FILE: input_cds,
-                          CancerGenomesService.CONFIG_OUTPUT_FILE: output_db,
-                          CancerGenomesService.CLINICAL_SAMPLE_FILE: clinical_sample_file,
-                          CancerGenomesService.FILTER_COLUMN: filter_column,
-                          CancerGenomesService.ACCEPTED_VALUES: accepted_values,
-                          CancerGenomesService.SPLIT_BY_FILTER_COLUMN: split_by_filter_column}
+  pipeline_arguments = {CancerGenomesService.CONFIG_CANCER_GENOMES_MUTATION_FILE: input_mutation,
+                        CancerGenomesService.CONFIG_COMPLETE_GENES_FILE: input_cds,
+                        CancerGenomesService.CONFIG_OUTPUT_FILE: output_db,
+                        CancerGenomesService.CLINICAL_SAMPLE_FILE: clinical_sample_file,
+                        CancerGenomesService.FILTER_COLUMN: filter_column,
+                        CancerGenomesService.ACCEPTED_VALUES: accepted_values,
+                        CancerGenomesService.SPLIT_BY_FILTER_COLUMN: split_by_filter_column}
 
-    cosmic_to_proteindb_service = CancerGenomesService(config_file, pipeline_arguments)
-    cosmic_to_proteindb_service.cbioportal_to_proteindb()
+  cosmic_to_proteindb_service = CancerGenomesService(config_file, pipeline_arguments)
+  cosmic_to_proteindb_service.cbioportal_to_proteindb()
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/cosmic_downloader.py` & `pypgatk-0.0.9/pypgatk/commands/cosmic_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,36 @@
 from pypgatk.cgenomes.cosmic_downloader import CosmicDownloadService
 from pypgatk.toolbox.exceptions import AppConfigException
 
 this_dir, this_filename = os.path.split(__file__)
 
 
 @click.command('cosmic-downloader', short_help='Command to download the cosmic mutation database')
-@click.option('--config_file',
-              '-c',
+@click.option('-c', '--config_file',
               help='Configuration file for the ensembl data downloader pipeline',
-              default=this_dir + '../config/cosmic_config.yaml')
-@click.option('--output_directory',
-              '-o',
+              default=this_dir + '/../config/cosmic_config.yaml')
+@click.option('-o', '--output_directory',
               help='Output directory for the peptide databases',
               default="./database_cosmic/")
-@click.option('--username', '-u',
+@click.option('-u', '--username',
               help="Username for cosmic database -- please if you don't have one register here (https://cancer.sanger.ac.uk/cosmic/register)")
-@click.option('--password', '-p',
+@click.option('-p', '--password',
               help="Password for cosmic database -- please if you don't have one register here (https://cancer.sanger.ac.uk/cosmic/register)")
 @click.pass_context
 def cosmic_downloader(ctx, config_file, output_directory, username, password):
-    if config_file is None:
-        msg = "The config file for the pipeline is missing, please provide one "
-        logging.error(msg)
-        raise AppConfigException(msg)
-
-    pipeline_arguments = {}
-    if output_directory is not None:
-        pipeline_arguments[CosmicDownloadService.CONFIG_OUTPUT_DIRECTORY] = output_directory
-    if username is not None:
-        pipeline_arguments[CosmicDownloadService.CONFIG_COSMIC_FTP_USER] = username
+  if config_file is None:
+    msg = "The config file for the pipeline is missing, please provide one "
+    logging.error(msg)
+    raise AppConfigException(msg)
+
+  pipeline_arguments = {}
+  if output_directory is not None:
+    pipeline_arguments[CosmicDownloadService.CONFIG_OUTPUT_DIRECTORY] = output_directory
+  if username is not None:
+    pipeline_arguments[CosmicDownloadService.CONFIG_COSMIC_FTP_USER] = username
 
-    if password is not None:
-        pipeline_arguments[CosmicDownloadService.CONFIG_COSMIC_FTP_PASSWORD] = password
+  if password is not None:
+    pipeline_arguments[CosmicDownloadService.CONFIG_COSMIC_FTP_PASSWORD] = password
 
-    cosmic_downloader_service = CosmicDownloadService(config_file, pipeline_arguments)
+  cosmic_downloader_service = CosmicDownloadService(config_file, pipeline_arguments)
 
-    cosmic_downloader_service.download_mutation_file()
+  cosmic_downloader_service.download_mutation_file()
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/cosmic_to_proteindb.py` & `pypgatk-0.0.9/pypgatk/commands/cosmic_to_proteindb.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 
 this_dir, this_filename = os.path.split(__file__)
 
 
 @click.command('cosmic-to-proteindb', short_help='Command to translate Cosmic mutation data into proteindb')
 @click.option('-c', '--config_file',
               help='Configuration file for the cosmic data pipelines',
-              default=this_dir + '../config/cosmic_config.yaml')
+              default=this_dir + '/../config/cosmic_config.yaml')
 @click.option('-in', '--input_mutation', help='Cosmic Mutation data file')
 @click.option('-fa', '--input_genes', help='All Cosmic genes')
-@click.option('-out', '--output_db', 
+@click.option('-out', '--output_db',
               help='Protein database including all the mutations')
-@click.option('-f',   '--filter_column', default='Primary site', 
+@click.option('-f', '--filter_column', default='Primary site',
               help='Column in the VCF file to be used for filtering or splitting mutations')
-@click.option('-a',   '--accepted_values', default='all', 
+@click.option('-a', '--accepted_values', default='all',
               help='Limit mutations to values (tissue type, sample name, etc) considered for generating proteinDBs, by default mutations from all records are considered')
-@click.option('-s',   '--split_by_filter_column', 
-              help='Use this flag to generate a proteinDB per group as specified in the filter_column, default is False', is_flag=True)
-
+@click.option('-s', '--split_by_filter_column',
+              help='Use this flag to generate a proteinDB per group as specified in the filter_column, default is False',
+              is_flag=True)
 @click.pass_context
-def cosmic_to_proteindb(ctx, config_file, input_mutation, input_genes, output_db, 
+def cosmic_to_proteindb(ctx, config_file, input_mutation, input_genes, output_db,
                         filter_column, accepted_values, split_by_filter_column):
-    if input_mutation is None or input_genes is None or output_db is None:
-        print_help()
+  if input_mutation is None or input_genes is None or output_db is None:
+    print_help()
 
-    pipeline_arguments = {CancerGenomesService.CONFIG_CANCER_GENOMES_MUTATION_FILE: input_mutation,
-                          CancerGenomesService.CONFIG_COMPLETE_GENES_FILE: input_genes,
-                          CancerGenomesService.CONFIG_OUTPUT_FILE: output_db,
-                          CancerGenomesService.FILTER_COLUMN: filter_column,
-                          CancerGenomesService.ACCEPTED_VALUES: accepted_values,
-                          CancerGenomesService.SPLIT_BY_FILTER_COLUMN: split_by_filter_column}
+  pipeline_arguments = {CancerGenomesService.CONFIG_CANCER_GENOMES_MUTATION_FILE: input_mutation,
+                        CancerGenomesService.CONFIG_COMPLETE_GENES_FILE: input_genes,
+                        CancerGenomesService.CONFIG_OUTPUT_FILE: output_db,
+                        CancerGenomesService.FILTER_COLUMN: filter_column,
+                        CancerGenomesService.ACCEPTED_VALUES: accepted_values,
+                        CancerGenomesService.SPLIT_BY_FILTER_COLUMN: split_by_filter_column}
 
-    cosmic_to_proteindb_service = CancerGenomesService(config_file, pipeline_arguments)
-    cosmic_to_proteindb_service.cosmic_to_proteindb()
+  cosmic_to_proteindb_service = CancerGenomesService(config_file, pipeline_arguments)
+  cosmic_to_proteindb_service.cosmic_to_proteindb()
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/dnaseq_to_proteindb.py` & `pypgatk-0.0.9/pypgatk/commands/dnaseq_to_proteindb.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pypgatk.commands.utils import print_help
 from pypgatk.ensembl.ensembl import EnsemblDataService
 
 this_dir, this_filename = os.path.split(__file__)
 
 
 @click.command("dnaseq-to-proteindb", short_help="Generate peptides based on DNA sequences")
-@click.option('--config_file', '-c', help='Configuration to perform conversion between ENSEMBL Files',
-              default= this_dir + '../config/ensembl_config.yaml')
+@click.option('-c', '--config_file', help='Configuration to perform conversion between ENSEMBL Files',
+              default= this_dir + '/../config/ensembl_config.yaml')
 @click.option('--input_fasta', help='Path to sequences fasta')
 @click.option('--translation_table', default=1, type=int, help='Translation Table (default 1)')
 @click.option('--num_orfs', default=3, type=int, help='Number of ORFs (default 0)')
 @click.option('--num_orfs_complement', default=0, type=int,
               help='Number of ORFs from the reverse side (default 0)')
 @click.option('--output_proteindb', default="peptide-database.fa", help="Output file name, exits if already exists")
 @click.option('-p', '--var_prefix', default="", help="String to add before the variant peptides")
@@ -34,23 +34,21 @@
 def dnaseq_to_proteindb(ctx, config_file, input_fasta, translation_table, num_orfs, num_orfs_complement,
                         output_proteindb, var_prefix,
                         skip_including_all_cds, include_biotypes, exclude_biotypes, biotype_str, expression_str,
                         expression_thresh):
     if input_fasta is None:
         print_help()
 
-    pipeline_arguments = {}
-    pipeline_arguments[EnsemblDataService.TRANSLATION_TABLE] = translation_table
-    pipeline_arguments[EnsemblDataService.PROTEIN_DB_OUTPUT] = output_proteindb
-    pipeline_arguments[EnsemblDataService.HEADER_VAR_PREFIX] = var_prefix
-    pipeline_arguments[EnsemblDataService.EXCLUDE_BIOTYPES] = exclude_biotypes
-    pipeline_arguments[EnsemblDataService.SKIP_INCLUDING_ALL_CDS] = skip_including_all_cds
-    pipeline_arguments[EnsemblDataService.INCLUDE_BIOTYPES] = include_biotypes
-    pipeline_arguments[EnsemblDataService.BIOTYPE_STR] = biotype_str
-    pipeline_arguments[EnsemblDataService.NUM_ORFS] = num_orfs
-    pipeline_arguments[EnsemblDataService.NUM_ORFS_COMPLEMENT] = num_orfs_complement
-    pipeline_arguments[EnsemblDataService.EXPRESSION_STR] = expression_str
-    pipeline_arguments[EnsemblDataService.EXPRESSION_THRESH] = expression_thresh
+    pipeline_arguments = {EnsemblDataService.TRANSLATION_TABLE: translation_table,
+                          EnsemblDataService.PROTEIN_DB_OUTPUT: output_proteindb,
+                          EnsemblDataService.HEADER_VAR_PREFIX: var_prefix,
+                          EnsemblDataService.EXCLUDE_BIOTYPES: exclude_biotypes,
+                          EnsemblDataService.SKIP_INCLUDING_ALL_CDS: skip_including_all_cds,
+                          EnsemblDataService.INCLUDE_BIOTYPES: include_biotypes,
+                          EnsemblDataService.BIOTYPE_STR: biotype_str, EnsemblDataService.NUM_ORFS: num_orfs,
+                          EnsemblDataService.NUM_ORFS_COMPLEMENT: num_orfs_complement,
+                          EnsemblDataService.EXPRESSION_STR: expression_str,
+                          EnsemblDataService.EXPRESSION_THRESH: expression_thresh}
 
     ensembl_data_service = EnsemblDataService(config_file, pipeline_arguments)
     ensembl_data_service.dnaseq_to_proteindb(input_fasta)
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/ensembl_database.py` & `pypgatk-0.0.9/pypgatk/commands/threeframe_translation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import logging
 import os
 
 import click
 
 from pypgatk.commands.utils import print_help
 from pypgatk.ensembl.ensembl import EnsemblDataService
 
 this_dir, this_filename = os.path.split(__file__)
 
-@click.command('ensembl-check', short_help="Command to check ensembl database for stop codons, gaps")
-@click.option('--config_file',
-              '-c',
-              help='Configuration to perform Ensembl database cehck',
+
+@click.command('threeframe-translation', short_help="Command to perform 3'frame translation")
+@click.option('-c', '--config_file',
+              help='Configuration to perform conversion between ENSEMBL Files',
               default= this_dir + '/../config/ensembl_config.yaml')
 @click.option('-in', '--input_fasta', help='input_fasta file to perform the translation')
+@click.option('-t', '--translation_table', help='Translation table default value 1', default='1')
 @click.option('-out', '--output', help='Output File', default="peptide-database.fa")
 @click.pass_context
-def ensembl_check(ctx, config_file, input_fasta,output):
+def threeframe_translation(ctx, config_file, input_fasta, translation_table, output):
     if input_fasta is None:
         print_help()
-
-    pipeline_arguments = {EnsemblDataService.PROTEIN_DB_OUTPUT: output}
+    pipeline_arguments = {EnsemblDataService.TRANSLATION_TABLE: translation_table,
+                          EnsemblDataService.PROTEIN_DB_OUTPUT: output}
 
     ensembl_data_service = EnsemblDataService(config_file, pipeline_arguments)
-    ensembl_data_service.check_proteindb(input_fasta)
+    ensembl_data_service.three_frame_translation(input_fasta)
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/ensembl_downloader.py` & `pypgatk-0.0.9/pypgatk/commands/ensembl_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,40 +5,38 @@
 
 from pypgatk.ensembl.data_downloader import EnsemblDataDownloadService
 from pypgatk.toolbox.exceptions import AppConfigException
 
 this_dir, this_filename = os.path.split(__file__)
 
 @click.command('ensembl-downloader', short_help='Command to download the ensembl information')
-@click.option('--config_file',
-              '-c',
+@click.option('-c', '--config_file',
               help='Configuration file for the ensembl data downloader pipeline',
-              default=this_dir + '../config/ensembl_downloader_config.yaml')
-@click.option('--output_directory',
-              '-o',
+              default=this_dir + '/../config/ensembl_downloader_config.yaml')
+@click.option('-o', '--output_directory',
               help='Output directory for the peptide databases',
               default="./database_ensembl/")
-@click.option('--folder_prefix_release',
-              '-fp', help='Output folder prefix to download the data',
+@click.option('-fp', '--folder_prefix_release',
+               help='Output folder prefix to download the data',
               default='release-')
-@click.option('--taxonomy',
-              '-t',
+@click.option('-t', '--taxonomy',
               help='Taxonomy identifiers (comma separated list can be given) that will be use to download the data from Ensembl',
               default='')
-@click.option('--list_taxonomies', '-l',
+@click.option('-l', '--list_taxonomies',
               help='Print the list of all the taxonomies in ENSEMBL (https://www.ensembl.org)', is_flag=True, default=False)
-@click.option('--skip_gtf', '-sg', help="Skip the gtf file during the download", is_flag=True)
-@click.option('--skip_protein', '-sp', help="Skip the protein fasta file during download", is_flag=True)
-@click.option('--skip_cds', '-sc', help='Skip the CDS file download', is_flag=True)
-@click.option('--skip_cdna', '-sd', help='Skip the cDNA file download', is_flag=True)
-@click.option('--skip_ncrna', '-sn', help='Skip the ncRNA file download', is_flag=True)
-@click.option('--skip_vcf', '-sv', help='Skip the VCF variant file', is_flag=True)
-@click.option('--ensembl_name', '-en', help='Ensembl name code to download, it can be use instead of taxonomy (e.g. homo_sapiens)', default='')
+@click.option('-sg', '--skip_gtf',  help="Skip the gtf file during the download", is_flag=True)
+@click.option('-sp', '--skip_protein', help="Skip the protein fasta file during download", is_flag=True)
+@click.option('-sc', '--skip_cds', help='Skip the CDS file download', is_flag=True)
+@click.option('-sd', '--skip_cdna', help='Skip the cDNA file download', is_flag=True)
+@click.option('-sn', '--skip_ncrna', help='Skip the ncRNA file download', is_flag=True)
+@click.option('-sv', '--skip_vcf', help='Skip the VCF variant file', is_flag=True)
+@click.option('-en', '--ensembl_name', help='Ensembl name code to download, it can be use instead of taxonomy (e.g. homo_sapiens)', default='')
+@click.option('--grch37', help='Download a previous version GRCh37 of ensembl genomes', is_flag=True)
 def ensembl_downloader(config_file, output_directory, folder_prefix_release, taxonomy, list_taxonomies,
-                       skip_gtf, skip_protein, skip_cds, skip_cdna, skip_ncrna, skip_vcf, ensembl_name):
+                       skip_gtf, skip_protein, skip_cds, skip_cdna, skip_ncrna, skip_vcf, ensembl_name, grch37 = False):
     """ This tool enables to download from enseml ftp the FASTA and GTF files"""
 
     if config_file is None:
         msg = "The config file for the pipeline is missing, please provide one "
         logging.error(msg)
         raise AppConfigException(msg)
 
@@ -85,10 +83,10 @@
     logger = ensembl_download_service.get_logger_for("Main Pipeline Ensembl Downloader")
     logger.info("Pipeline STARTING ... ")
     if list_taxonomies:
         list_of_taxonomies = ensembl_download_service.get_species_from_rest()
         for taxonomy_info in list_of_taxonomies:
             print(taxonomy_info)
 
-    ensembl_download_service.download_database_by_species()
+    ensembl_download_service.download_database_by_species(grch37)
 
     logger.info("Pipeline Finish !!!")
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/proteindb_decoy.py` & `pypgatk-0.0.9/pypgatk/commands/proteindb_decoy.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
 this_dir, this_filename = os.path.split(__file__)
 
 
 @click.command('generate-decoy', short_help='Create decoy protein sequences. Each protein '
                                              'is reversed and the cleavage sites switched with preceding amino acid. Peptides are checked for existence in target sequences if found'
                                              'the tool will attempt to shuffle them. James.Wright@sanger.ac.uk 2015')
-@click.option('--config_file',         '-c', help='Configuration file for the protein database decoy generation', default= this_dir + '../config/protein_decoy.yaml')
-@click.option('--output',              '-o', help='Output file for decoy database', default="protein-decoy.fa")
-@click.option('--input',               '-i', help='FASTA file of target proteins sequences for which to create decoys (*.fasta|*.fa)')
-@click.option('--cleavage_sites',      '-s', default='KR', help='A list of amino acids at which to cleave during digestion. Default = KR')
-@click.option('--anti_cleavage_sites', '-a', help='A list of amino acids at which not to cleave if following cleavage site ie. Proline. Default = none')
-@click.option('--cleavage_position',   '-p', default='c', help='Set cleavage to be c or n terminal of specified cleavage sites. Options [c, n], Default = c')
-@click.option('--min_peptide_length',  '-l', type=int, help='Set minimum length of peptides to compare between target and decoy. Default = 5')
-@click.option('--max_iterations',      '-n', type=int, help='Set maximum number of times to shuffle a peptide to make it non-target before failing. Default=100')
-@click.option('--do_not_shuffle',      '-x', help='Turn OFF shuffling of decoy peptides that are in the target database. Default=false')
-@click.option('--do_not_switch',       '-w', help='Turn OFF switching of cleavage site with preceding amino acid. Default=false')
-@click.option('--decoy_prefix',        '-d', help='Set accession prefix for decoy proteins in output. Default=DECOY_')
-@click.option('--temp_file',           '-t', help='Set temporary file to write decoys prior to shuffling. Default=protein-decoy.fa')
-@click.option('--no_isobaric',         '-b', help='Do not make decoy peptides isobaric. Default=false')
-@click.option('--memory_save',         '-m', help='Slower but uses less memory (does not store decoy peptide list). Default=false')
+@click.option('-c', '--config_file', help='Configuration file for the protein database decoy generation', default= this_dir + '/../config/protein_decoy.yaml')
+@click.option('-o', '--output',      help='Output file for decoy database', default="protein-decoy.fa")
+@click.option( '-i', '--input',               help='FASTA file of target proteins sequences for which to create decoys (*.fasta|*.fa)')
+@click.option('-s', '--cleavage_sites',      default='KR', help='A list of amino acids at which to cleave during digestion. Default = KR')
+@click.option('-a', '--anti_cleavage_sites',  help='A list of amino acids at which not to cleave if following cleavage site ie. Proline. Default = none')
+@click.option('-p', '--cleavage_position',    default='c', help='Set cleavage to be c or n terminal of specified cleavage sites. Options [c, n], Default = c')
+@click.option('-l', '--min_peptide_length',  type=int, help='Set minimum length of peptides to compare between target and decoy. Default = 5')
+@click.option('-n', '--max_iterations',      type=int, help='Set maximum number of times to shuffle a peptide to make it non-target before failing. Default=100')
+@click.option('-x', '--do_not_shuffle',       help='Turn OFF shuffling of decoy peptides that are in the target database. Default=false')
+@click.option('-w', '--do_not_switch',      help='Turn OFF switching of cleavage site with preceding amino acid. Default=false')
+@click.option('-d', '--decoy_prefix',       help='Set accession prefix for decoy proteins in output. Default=DECOY_')
+@click.option('-t', '--temp_file',          help='Set temporary file to write decoys prior to shuffling. Default=protein-decoy.fa')
+@click.option('-b', '--no_isobaric',         help='Do not make decoy peptides isobaric. Default=false')
+@click.option( '-m', '--memory_save',        help='Slower but uses less memory (does not store decoy peptide list). Default=false')
 @click.pass_context
 def generate_database(ctx, config_file, output, input, cleavage_sites, anti_cleavage_sites, cleavage_position, min_peptide_length,
                    max_iterations, do_not_shuffle, do_not_switch, decoy_prefix, temp_file, no_isobaric, memory_save):
 
     if config_file is None:
         msg = "The config file for the pipeline is missing, please provide one "
         logging.error(msg)
```

### Comparing `pypgatk-0.0.8/pypgatk/commands/utils.py` & `pypgatk-0.0.9/pypgatk/commands/utils.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk/commands/vcf_to_proteindb.py` & `pypgatk-0.0.9/pypgatk/commands/vcf_to_proteindb.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pypgatk.commands.utils import print_help
 from pypgatk.ensembl.ensembl import EnsemblDataService
 
 this_dir, this_filename = os.path.split(__file__)
 
 
 @click.command('vcf-to-proteindb', short_help="Generate peptides based on DNA variants from ENSEMBL VEP VCF files")
-@click.option('--config_file', '-c', help='Configuration to perform conversion between ENSEMBL Files',
-              default= this_dir + '../config/ensembl_config.yaml')
+@click.option('-c', '--config_file', help='Configuration to perform conversion between ENSEMBL Files',
+              default= this_dir + '/../config/ensembl_config.yaml')
 @click.option('-f', '--input_fasta', help='Path to the transcript sequence')
 @click.option('-v', '--vep_annotated_vcf', help='Path to the vep annotated VCF file')
 @click.option('-g', '--gene_annotations_gtf', help='Path to the gene annotations file')
 @click.option('-t', '--translation_table', default=1, type=int, help="Translation table (Default 1) ")
 @click.option('-m', '--mito_translation_table', default=2, type=int, help='Mito_trans_table (default 2)')
 @click.option('-p', '--var_prefix', default="var", help="String to add before the variant peptides")
 @click.option('--report_ref_seq', help='In addition to var peps, also report all ref peps', is_flag=True)
@@ -48,29 +48,27 @@
                      var_prefix, report_ref_seq, output_proteindb, annotation_field_name,
                      af_field, af_threshold, transcript_index, consequence_index, exclude_biotypes,
                      exclude_consequences, skip_including_all_cds, include_biotypes, include_consequences, biotype_str,
                      ignore_filters, accepted_filters):
     if input_fasta is None or vep_annotated_vcf is None or gene_annotations_gtf is None:
         print_help()
 
-    pipeline_arguments = {}
-    pipeline_arguments[EnsemblDataService.MITO_TRANSLATION_TABLE] = mito_translation_table
-    pipeline_arguments[EnsemblDataService.TRANSLATION_TABLE] = translation_table
-    pipeline_arguments[EnsemblDataService.HEADER_VAR_PREFIX] = var_prefix
-    pipeline_arguments[EnsemblDataService.REPORT_REFERENCE_SEQ] = report_ref_seq
-    pipeline_arguments[EnsemblDataService.PROTEIN_DB_OUTPUT] = output_proteindb
-    pipeline_arguments[EnsemblDataService.ANNOTATION_FIELD_NAME] = annotation_field_name
-    pipeline_arguments[EnsemblDataService.AF_FIELD] = af_field
-    pipeline_arguments[EnsemblDataService.AF_THRESHOLD] = af_threshold
-    pipeline_arguments[EnsemblDataService.TRANSCRIPT_INDEX] = transcript_index
-    pipeline_arguments[EnsemblDataService.CONSEQUENCE_INDEX] = consequence_index
-    pipeline_arguments[EnsemblDataService.EXCLUDE_BIOTYPES] = exclude_biotypes
-    pipeline_arguments[EnsemblDataService.EXCLUDE_CONSEQUENCES] = exclude_consequences
-    pipeline_arguments[EnsemblDataService.SKIP_INCLUDING_ALL_CDS] = skip_including_all_cds
-    pipeline_arguments[EnsemblDataService.INCLUDE_BIOTYPES] = include_biotypes
-    pipeline_arguments[EnsemblDataService.INCLUDE_CONSEQUENCES] = include_consequences
-    pipeline_arguments[EnsemblDataService.BIOTYPE_STR] = biotype_str
-    pipeline_arguments[EnsemblDataService.IGNORE_FILTERS] = ignore_filters
-    pipeline_arguments[EnsemblDataService.ACCEPTED_FILTERS] = accepted_filters
+    pipeline_arguments = {EnsemblDataService.MITO_TRANSLATION_TABLE: mito_translation_table,
+                          EnsemblDataService.TRANSLATION_TABLE: translation_table,
+                          EnsemblDataService.HEADER_VAR_PREFIX: var_prefix,
+                          EnsemblDataService.REPORT_REFERENCE_SEQ: report_ref_seq,
+                          EnsemblDataService.PROTEIN_DB_OUTPUT: output_proteindb,
+                          EnsemblDataService.ANNOTATION_FIELD_NAME: annotation_field_name,
+                          EnsemblDataService.AF_FIELD: af_field, EnsemblDataService.AF_THRESHOLD: af_threshold,
+                          EnsemblDataService.TRANSCRIPT_INDEX: transcript_index,
+                          EnsemblDataService.CONSEQUENCE_INDEX: consequence_index,
+                          EnsemblDataService.EXCLUDE_BIOTYPES: exclude_biotypes,
+                          EnsemblDataService.EXCLUDE_CONSEQUENCES: exclude_consequences,
+                          EnsemblDataService.SKIP_INCLUDING_ALL_CDS: skip_including_all_cds,
+                          EnsemblDataService.INCLUDE_BIOTYPES: include_biotypes,
+                          EnsemblDataService.INCLUDE_CONSEQUENCES: include_consequences,
+                          EnsemblDataService.BIOTYPE_STR: biotype_str,
+                          EnsemblDataService.IGNORE_FILTERS: ignore_filters,
+                          EnsemblDataService.ACCEPTED_FILTERS: accepted_filters}
 
     ensembl_data_service = EnsemblDataService(config_file, pipeline_arguments)
     ensembl_data_service.vcf_to_proteindb(vep_annotated_vcf, input_fasta, gene_annotations_gtf)
```

### Comparing `pypgatk-0.0.8/pypgatk/db/digest_mutant_protein.py` & `pypgatk-0.0.9/pypgatk/db/digest_mutant_protein.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         elif opt == '--min_len':
             min = int(arg)
         elif opt == '--max_len':
             max = int(arg)
         elif opt == '--miss':
             cleavageMiss = int(arg)
         else:
-            print("Warning! Command-line argument: %s not recognized. Exiting..." % opt);
+            print("Warning! Command-line argument: %s not recognized. Exiting..." % opt)
             sys.exit()
 
 handle1 = SeqIO.parse(fa_file, 'fasta')  # canonical protein sequences
 peptidome = {}
 
 for record in handle1:
     aa_seq = record.seq
```

### Comparing `pypgatk-0.0.8/pypgatk/db/map_peptide2genome.py` & `pypgatk-0.0.9/pypgatk/db/map_peptide2genome.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             pep_strand = exon.strand
             pep_start_exon = i + 1
             if pep_strand == '+':
                 pep_chr_start = exon.start + (n1 - exon.trans_start)
             else:
                 pep_chr_end = exon.end - (n1 - exon.trans_start)
 
-        if n2 <= exon.trans_end and n2 >= exon.trans_start:
+        if exon.trans_end >= n2 >= exon.trans_start:
             pep_chr = exon.chr
             pep_strand = exon.strand
             pep_end_exon = i + 1
             if pep_strand == '+':
                 pep_chr_end = exon.start + (n2 - exon.trans_start)
             else:  # chr_cor of n2 is pep_chr_start
                 pep_chr_start = exon.end - (n2 - exon.trans_start)
@@ -171,15 +171,15 @@
 
 for peptide, ensp in pep_dic.items():
     enst = id_dic[ensp]
     try:
         exons = feature_dic[enst]
     except KeyError:
         non_mapped_pep += 1
-        continue;
+        continue
 
     aa_seq = str(seq_dic[ensp].seq)
     pep_index = aa_seq.index(peptide)
 
     pep_trans_start = 3 * pep_index + 1
     pep_trans_end = pep_trans_start + 3 * len(peptide) - 1
 
@@ -189,19 +189,19 @@
     pep_chr, pep_strand, pep_chr_start, pep_chr_end, pep_start_exon, pep_end_exon = get_pep_cor(exons, pep_trans_start,
                                                                                                 pep_trans_end)
 
     # handle exceptions
     if pep_chr_start > pep_chr_end:
         non_mapped_pep += 1
         # print peptide,ensp,enst
-        continue;
+        continue
     if pep_chr_start <= 0:
         non_mapped_pep += 1
         # print peptide,ensp,enst,pep_trans_start,pep_trans_end
-        continue;
+        continue
 
     # print pep_chr_start,pep_chr_end
     # print pep_start_exon,pep_end_exon
     pep_chr = "chr" + pep_chr.replace("MT", "M")
     if pep_start_exon == pep_end_exon:  # if peptide map to one exon
         gff_format_line1 = [pep_chr, "MS", "mRNA", pep_chr_start, pep_chr_end, ".", pep_strand, ".", "ID=" + peptide]
         gff_format_line2 = [pep_chr, "MS", "CDS", pep_chr_start, pep_chr_end, ".", pep_strand, "0", "Parent=" + peptide]
```

### Comparing `pypgatk-0.0.8/pypgatk/ensembl/data_downloader.py` & `pypgatk-0.0.9/pypgatk/ensembl/data_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,330 +12,371 @@
 from requests import get
 
 from pypgatk.toolbox.general import ParameterConfiguration, check_create_folders, download_file
 from pypgatk.toolbox.rest import call_api
 
 
 class EnsemblDataDownloadService(ParameterConfiguration):
-    """
+  """
     This Service is in charge of grabbing data (download) from Ensembl to a local repository
     """
 
-    CONFIG_KEY_DATA_DOWNLOADER = 'ensembl_data_downloader'
-    CONFIG_OUTPUT_DIRECTORY = 'output_directory'
-    CONFIG_KEY_ENSEMBL_FTP = 'ensembl_ftp'
-    CONFIG_ENSEMBL_API = 'ensembl_api'
-    CONFIG_ENSEMBL_API_SERVER = 'server'
-    CONFIG_ENSEMBL_API_SPECIES = 'species'
-    CONFIG_KEY_BASE_URL = 'base_url'
-    CONFIG_KEY_FOLDER_PREFIX_RELEASE = 'folder_prefix_release'
-    CONFIG_KEY_FOLDER_NAME_FASTA = 'folder_name_fasta'
-    CONFIG_KEY_FOLDER_NAME_PROTEIN_SEQUENCES = 'folder_name_protein_sequences'
-    CONFIG_KEY_FOLDER_NAME_GTF = 'folder_name_gtf'
-    CONFIG_KEY_REWRITE_LOCAL_PATH_ENSEMBL_REPO = 'rewrite_local_path_ensembl_repo'
-    CONFIG_KEY_ENSEMBL_FILE_NAMES = 'ensembl_file_names'
-    CONFIG_KEY_PROTEIN_SEQUENCE_FILE = 'protein_sequence_file'
-    CONFIG_KEY_FILE_TYPE = 'file_type'
-    CONFIG_KEY_FILE_SUFFIXES = 'file_suffixes'
-    CONFIG_KEY_FILE_EXTENSION = 'file_extension'
-    CONFIG_KEY_GTF_FILE = 'gtf_file'
-    CONFIG_REST_API_TAXON_ID = 'taxon_id'
-    CONFIG_REST_API_NAME = 'name'
-    CONFIG_TAXONOMY = 'taxonomy'
-    CONFIG_ENSEMBL_NAME = 'name'
-    CONFIG_LIST_TAXONOMIES = 'list_taxonomies'
-    CONFIG_KEY_SKIP_PROTEIN = 'skip_protein'
-    CONFIG_KEY_SKIP_GTF = 'skip_gtf'
-    CONFIG_KEY_SKIP_CDS = 'skip_cds'
-    CONFIG_KEY_SKIP_CDNA = 'skip_cdna'
-    CONFIG_KEY_SKIP_NCRNA = 'skip_ncrna'
-    CONFIG_KEY_SKIP_VCF = 'skip_vcf'
+  CONFIG_KEY_DATA_DOWNLOADER = 'ensembl_data_downloader'
+  CONFIG_OUTPUT_DIRECTORY = 'output_directory'
+  CONFIG_KEY_ENSEMBL_FTP = 'ensembl_ftp'
+  CONFIG_ENSEMBL_API = 'ensembl_api'
+  CONFIG_ENSEMBL_API_SERVER = 'server'
+  CONFIG_ENSEMBL_API_SPECIES = 'species'
+  CONFIG_KEY_BASE_URL = 'base_url'
+  CONFIG_KEY_FOLDER_PREFIX_RELEASE = 'folder_prefix_release'
+  CONFIG_KEY_FOLDER_NAME_FASTA = 'folder_name_fasta'
+  CONFIG_KEY_FOLDER_NAME_PROTEIN_SEQUENCES = 'folder_name_protein_sequences'
+  CONFIG_KEY_FOLDER_NAME_GTF = 'folder_name_gtf'
+  CONFIG_KEY_REWRITE_LOCAL_PATH_ENSEMBL_REPO = 'rewrite_local_path_ensembl_repo'
+  CONFIG_KEY_ENSEMBL_FILE_NAMES = 'ensembl_file_names'
+  CONFIG_KEY_PROTEIN_SEQUENCE_FILE = 'protein_sequence_file'
+  CONFIG_KEY_FILE_TYPE = 'file_type'
+  CONFIG_KEY_FILE_SUFFIXES = 'file_suffixes'
+  CONFIG_KEY_FILE_EXTENSION = 'file_extension'
+  CONFIG_KEY_GTF_FILE = 'gtf_file'
+  CONFIG_REST_API_TAXON_ID = 'taxon_id'
+  CONFIG_REST_API_NAME = 'name'
+  CONFIG_TAXONOMY = 'taxonomy'
+  CONFIG_ENSEMBL_NAME = 'name'
+  CONFIG_LIST_TAXONOMIES = 'list_taxonomies'
+  CONFIG_KEY_SKIP_PROTEIN = 'skip_protein'
+  CONFIG_KEY_SKIP_GTF = 'skip_gtf'
+  CONFIG_KEY_SKIP_CDS = 'skip_cds'
+  CONFIG_KEY_SKIP_CDNA = 'skip_cdna'
+  CONFIG_KEY_SKIP_NCRNA = 'skip_ncrna'
+  CONFIG_KEY_SKIP_VCF = 'skip_vcf'
 
-    def __init__(self, config_file, pipeline_arguments):
-        """
+  def __init__(self, config_file, pipeline_arguments):
+    """
         Init the class with the specific parameters.
         :param config_file configuration file
         :param pipeline_arguments pipelines arguments
         """
-        super(EnsemblDataDownloadService, self).__init__(self.CONFIG_KEY_DATA_DOWNLOADER, config_file,
-                                                         pipeline_arguments)
-
-        self._ensembl_species = []
-        if self.CONFIG_OUTPUT_DIRECTORY in self.get_pipeline_parameters():
-            self._local_path_ensembl = self.get_pipeline_parameters()[self.CONFIG_OUTPUT_DIRECTORY]
-        else:
-            self._local_path_ensembl = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
-                self.CONFIG_OUTPUT_DIRECTORY]
-        
-        self._list_taxonomies = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_LIST_TAXONOMIES]
-        if self.CONFIG_LIST_TAXONOMIES in self.get_pipeline_parameters():
-            self._list_taxonomies = self.get_pipeline_parameters()[self.CONFIG_LIST_TAXONOMIES]
-
-        self.prepare_local_ensembl_repository()
+    super(EnsemblDataDownloadService, self).__init__(self.CONFIG_KEY_DATA_DOWNLOADER, config_file,
+                                                     pipeline_arguments)
 
-    def get_local_path_root_ensembl_repo(self):
-        return self._local_path_ensembl
+    self._ensembl_species = []
+    if self.CONFIG_OUTPUT_DIRECTORY in self.get_pipeline_parameters():
+      self._local_path_ensembl = self.get_pipeline_parameters()[self.CONFIG_OUTPUT_DIRECTORY]
+    else:
+      self._local_path_ensembl = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][
+        self.CONFIG_OUTPUT_DIRECTORY]
+
+    self._list_taxonomies = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_LIST_TAXONOMIES]
+    if self.CONFIG_LIST_TAXONOMIES in self.get_pipeline_parameters():
+      self._list_taxonomies = self.get_pipeline_parameters()[self.CONFIG_LIST_TAXONOMIES]
+
+    self.prepare_local_ensembl_repository()
+
+  def get_local_path_root_ensembl_repo(self):
+    return self._local_path_ensembl
+
+  def prepare_local_ensembl_repository(self):
+    self.get_logger().debug(
+      "Preparing local Ensembl repository, root folder - '{}'".format(self.get_local_path_root_ensembl_repo()))
+    check_create_folders([self.get_local_path_root_ensembl_repo()])
+    self.get_logger().debug(
+      "Local path for Ensembl Release - '{}'".format(self.get_local_path_root_ensembl_repo()))
 
-    def prepare_local_ensembl_repository(self):
-        self.get_logger().debug(
-            "Preparing local Ensembl repository, root folder - '{}'".format(self.get_local_path_root_ensembl_repo()))
-        check_create_folders([self.get_local_path_root_ensembl_repo()])
-        self.get_logger().debug(
-            "Local path for Ensembl Release - '{}'".format(self.get_local_path_root_ensembl_repo()))
-
-    def get_species_from_rest(self):
-        """
+  def get_species_from_rest(self):
+    """
         Get the list of species from ENSEMBL rest API.
         :return:
         """
-        server = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_ENSEMBL_API][
-            self.CONFIG_ENSEMBL_API_SERVER]
-        endpoint = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_ENSEMBL_API][
-            self.CONFIG_ENSEMBL_API_SPECIES]
-        species_info = loads(call_api(server + endpoint).text)
-        self._ensembl_species = species_info['species']
-        return self._ensembl_species
+    server = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_ENSEMBL_API][
+      self.CONFIG_ENSEMBL_API_SERVER]
+    endpoint = self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_ENSEMBL_API][
+      self.CONFIG_ENSEMBL_API_SPECIES]
+    species_info = loads(call_api(server + endpoint).text)
+    self._ensembl_species = species_info['species']
+    return self._ensembl_species
 
-    def download_database_by_species(self):
-        """
+  def download_database_by_species(self, grch37=False):
+    """
         This method takes a list of Taxonomies from the commandline parameters and download the Protein fasta files
         and the gtf files.
         :return:
         """
-        self.get_species_from_rest()
-        species_parameters = self.get_pipeline_parameters()[self.CONFIG_TAXONOMY]
-        species_list = species_parameters.split(",")
-
-        species_name = self.get_pipeline_parameters()[self.CONFIG_ENSEMBL_NAME]
-        species_name_parameters = ()
-        if species_name is not None:
-            species_name_parameters = species_name.split(",")
-
-        total_files = []
-        files = []
-        if species_list is not None and len(species_list) > 0 and len(species_parameters) > 0:
-            for species_id in species_list:
-                for species in self._ensembl_species:
-                    if species_id == species[self.CONFIG_REST_API_TAXON_ID]:
-                        self.get_logger().debug(
-                            "Downloading the data for the specie -- " + species[self.CONFIG_REST_API_TAXON_ID])
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_PROTEIN]:
-                            prot_files = self.get_pep_files(species)
-                            files.extend(prot_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_GTF]:
-                            gtf_files = self.get_gtf_files(species)
-                            files.extend(gtf_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDS]:
-                            cds_files = self.get_cds_files(species)
-                            files.extend(cds_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDNA]:
-                            cdna_files = self.get_cdna_files(species)
-                            files.extend(cdna_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_NCRNA]:
-                            ncrna_files = self.get_ncrna_files(species)
-                            files.extend(ncrna_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_VCF]:
-                            vcf_files = self.get_vcf_files(species)
-                            files.extend(vcf_files)
-                        
-                        total_files.extend(files)
-                        self.get_logger().debug("Files downloaded -- " + ",".join(files))
-                        total_files.extend(files)
-        elif species_name_parameters is not None and len(species_name_parameters) > 0:
-            for species_name in species_name_parameters:
-                for species in self._ensembl_species:
-                    if species_name == species[self.CONFIG_REST_API_NAME]:
-                        self.get_logger().debug(
-                            "Downloading the data for the specie -- " + species[self.CONFIG_REST_API_NAME])
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_PROTEIN]:
-                            prot_files = self.get_pep_files(species)
-                            files.extend(prot_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_GTF]:
-                            gtf_files = self.get_gtf_files(species)
-                            files.extend(gtf_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDS]:
-                            cds_files = self.get_cds_files(species)
-                            files.extend(cds_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDNA]:
-                            cdna_files = self.get_cdna_files(species)
-                            files.extend(cdna_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_NCRNA]:
-                            ncrna_files = self.get_ncrna_files(species)
-                            files.extend(ncrna_files)
-                        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_VCF]:
-                            vcf_files = self.get_vcf_files(species)
-                            files.extend(vcf_files)
-
-                        total_files.extend(files)
-                        self.get_logger().debug("Files downloaded -- " + ",".join(files))
-                        total_files.extend(files)
-        else:
-            for species in self._ensembl_species:
-                self.get_logger().debug(
-                    "Downloading the data for the specie -- " + species[self.CONFIG_REST_API_TAXON_ID])
-                if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_PROTEIN]:
-                    prot_files = self.get_pep_files(species)
-                    files.extend(prot_files)
-                if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_GTF]:
-                    gtf_files = self.get_gtf_files(species)
-                    files.extend(gtf_files)
-                if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDS]:
-                    cds_files = self.get_cds_files(species)
-                    files.extend(cds_files)
-                if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDNA]:
-                    cdna_files = self.get_cdna_files(species)
-                    files.extend(cdna_files)
-                if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_NCRNA]:
-                    ncrna_files = self.get_ncrna_files(species)
-                    files.extend(ncrna_files)
-                if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_VCF]:
-                    vcf_files = self.get_vcf_files(species)
-                    files.extend(vcf_files)
-
-                total_files.extend(files)
-                self.get_logger().debug("Files downloaded -- " + ",".join(files))
-                total_files.extend(files)
+    self.get_species_from_rest()
+    species_parameters = self.get_pipeline_parameters()[self.CONFIG_TAXONOMY]
+    species_list = species_parameters.split(",")
+
+    species_name = self.get_pipeline_parameters()[self.CONFIG_ENSEMBL_NAME]
+    species_name_parameters = ()
+    if species_name is not None:
+      species_name_parameters = species_name.split(",")
+
+    total_files = []
+    files = []
+    if species_list is not None and len(species_list) > 0 and len(species_parameters) > 0:
+      for species_id in species_list:
+        for species in self._ensembl_species:
+          if species_id == species[self.CONFIG_REST_API_TAXON_ID]:
+            self.get_logger().debug(
+              "Downloading the data for the specie -- " + species[self.CONFIG_REST_API_TAXON_ID])
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_PROTEIN]:
+              prot_files = self.get_pep_files(species, grch37)
+              files.extend(prot_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_GTF]:
+              gtf_files = self.get_gtf_files(species, grch37)
+              files.extend(gtf_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDS]:
+              cds_files = self.get_cds_files(species, grch37)
+              files.extend(cds_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDNA]:
+              cdna_files = self.get_cdna_files(species, grch37)
+              files.extend(cdna_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_NCRNA]:
+              ncrna_files = self.get_ncrna_files(species, grch37)
+              files.extend(ncrna_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_VCF]:
+              vcf_files = self.get_vcf_files(species)
+              files.extend(vcf_files)
+
+            total_files.extend(files)
+            self.get_logger().debug("Files downloaded -- " + ",".join(files))
+            total_files.extend(files)
+    elif species_name_parameters is not None and len(species_name_parameters) > 0:
+      for species_name in species_name_parameters:
+        for species in self._ensembl_species:
+          if species_name == species[self.CONFIG_REST_API_NAME]:
+            self.get_logger().debug(
+              "Downloading the data for the specie -- " + species[self.CONFIG_REST_API_NAME])
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_PROTEIN]:
+              prot_files = self.get_pep_files(species)
+              files.extend(prot_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_GTF]:
+              gtf_files = self.get_gtf_files(species)
+              files.extend(gtf_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDS]:
+              cds_files = self.get_cds_files(species)
+              files.extend(cds_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDNA]:
+              cdna_files = self.get_cdna_files(species)
+              files.extend(cdna_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_NCRNA]:
+              ncrna_files = self.get_ncrna_files(species)
+              files.extend(ncrna_files)
+            if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_VCF]:
+              vcf_files = self.get_vcf_files(species)
+              files.extend(vcf_files)
+
+            total_files.extend(files)
+            self.get_logger().debug("Files downloaded -- " + ",".join(files))
+            total_files.extend(files)
+    else:
+      for species in self._ensembl_species:
+        self.get_logger().debug(
+          "Downloading the data for the specie -- " + species[self.CONFIG_REST_API_TAXON_ID])
+        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_PROTEIN]:
+          prot_files = self.get_pep_files(species, grch37)
+          files.extend(prot_files)
+        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_GTF]:
+          gtf_files = self.get_gtf_files(species, grch37)
+          files.extend(gtf_files)
+        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDS]:
+          cds_files = self.get_cds_files(species, grch37)
+          files.extend(cds_files)
+        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_CDNA]:
+          cdna_files = self.get_cdna_files(species, grch37)
+          files.extend(cdna_files)
+        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_NCRNA]:
+          ncrna_files = self.get_ncrna_files(species, grch37)
+          files.extend(ncrna_files)
+        if not self.get_pipeline_parameters()[self.CONFIG_KEY_SKIP_VCF]:
+          vcf_files = self.get_vcf_files(species)
+          files.extend(vcf_files)
+
+        total_files.extend(files)
+        self.get_logger().debug("Files downloaded -- " + ",".join(files))
+        total_files.extend(files)
 
-        return total_files
+    return total_files
 
-    def get_cds_files(self, species: dict) -> list:
-        """
+  def get_cds_files(self, species: dict, grch37=False) -> list:
+    """
         Get the cds files for a specific species object.
         :return: List of files names.
         """
-        files = []
-        try:
-            file_name = '{}.{}.cds.all.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
-                                                     species['assembly'])
-            file_url = '{}/release-{}/fasta/{}/cds/{}'.format(
-                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
-                    self.CONFIG_KEY_BASE_URL],
-                species['release'], species['name'], file_name)
-            files.append(download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-        except KeyError:
-            print("No valid info is available species: ", species)
+    files = []
+    try:
+      if grch37:
+        species['assembly'] = 'GRCh37'
+      file_name = '{}.{}.cds.all.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
+                                               species['assembly'])
+      file_url = '{}/release-{}/fasta/{}/cds/{}'.format(
+        self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+          self.CONFIG_KEY_BASE_URL], species['release'], species['name'], file_name)
+      if grch37:
+        file_url = '{}/grch37/release-{}/fasta/{}/cds/{}'.format(
+          self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+            self.CONFIG_KEY_BASE_URL], species['release'], species['name'], file_name)
+      files.append(
+        download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
+    except KeyError:
+      print("No valid info is available species: ", species)
 
-        return files
+    return files
 
-    def get_cdna_files(self, species: dict) -> list:
-        """
+  def get_cdna_files(self, species: dict, grch37=False) -> list:
+    """
         Get the cds files for a specific species object.
         :return: List of files names.
         """
-        files = []
-        try:
-            file_name = '{}.{}.cdna.all.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
-                                                     species['assembly'])
-            file_url = '{}/release-{}/fasta/{}/cdna/{}'.format(
-                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
-                    self.CONFIG_KEY_BASE_URL],
-                species['release'], species['name'], file_name)
-            files.append(download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-        except KeyError:
-            print("No valid info is available species: ", species)
+    files = []
+    try:
+      if grch37:
+        species['assembly'] = 'GRCh37'
+      file_name = '{}.{}.cdna.all.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
+                                                species['assembly'])
+      file_url = '{}/release-{}/fasta/{}/cdna/{}'.format(
+        self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+          self.CONFIG_KEY_BASE_URL],
+        species['release'], species['name'], file_name)
+      if grch37:
+        file_url = '{}/grch37/release-{}/fasta/{}/cdna/{}'.format(
+          self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+            self.CONFIG_KEY_BASE_URL],
+          species['release'], species['name'], file_name)
+      files.append(
+        download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
+    except KeyError:
+      print("No valid info is available species: ", species)
 
-        return files
+    return files
 
-    def get_ncrna_files(self, species: dict) -> list:
-        """
+  def get_ncrna_files(self, species: dict, grch37=False) -> list:
+    """
         Get the cds files for a specific species object.
         :return: List of files names.
         """
-        files = []
-        try:
-            file_name = '{}.{}.ncrna.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
-                                                   species['assembly'])
-            file_url = '{}/release-{}/fasta/{}/ncrna/{}'.format(
-                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
-                    self.CONFIG_KEY_BASE_URL],
-                species['release'], species['name'], file_name)
-            files.append(download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-        except KeyError:
-            print("No valid info is available species: ", species)
+    files = []
+    try:
+      if grch37:
+        species['assembly'] = 'GRCh37'
+
+      file_name = '{}.{}.ncrna.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
+                                             species['assembly'])
+      file_url = '{}/release-{}/fasta/{}/ncrna/{}'.format(
+        self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+          self.CONFIG_KEY_BASE_URL],
+        species['release'], species['name'], file_name)
+      if grch37:
+        file_url = '{}/grch37/release-{}/fasta/{}/ncrna/{}'.format(
+          self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+            self.CONFIG_KEY_BASE_URL],
+          species['release'], species['name'], file_name)
+      files.append(
+        download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
+    except KeyError:
+      print("No valid info is available species: ", species)
 
-        return files
+    return files
 
-    def get_pep_files(self, species: dict) -> list:
-        """
-        Get the peptide files for a specific species object.
-        :return: List of files names.
-        """
-        files = []
-        try:
-            file_name = '{}.{}.pep.all.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
-                                                     species['assembly'])
-            file_url = '{}/release-{}/fasta/{}/pep/{}'.format(
-                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
-                    self.CONFIG_KEY_BASE_URL],
-                species['release'], species['name'], file_name)
-            files.append(download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-        except KeyError:
-            print("No valid info is available species: ", species)
+  def get_pep_files(self, species: dict, grch37=False) -> list:
+    """
+      Get the peptide files for a specific species object.
+      :return: List of files names.
+      """
+    files = []
+    try:
+      # TODO: Would be better to check by API the assembly version
+      if grch37:
+        species['assembly'] = 'GRCh37'
+      file_name = '{}.{}.pep.all.fa.gz'.format(species['name'][0].upper() + species['name'][1:],
+                                               species['assembly'])
+      file_url = '{}/release-{}/fasta/{}/pep/{}'.format(
+        self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+          self.CONFIG_KEY_BASE_URL],
+        species['release'], species['name'], file_name)
+      if grch37:
+        file_url = '{}/grch37/release-{}/fasta/{}/pep/{}'.format(
+          self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+            self.CONFIG_KEY_BASE_URL],
+          species['release'], species['name'], file_name)
+      files.append(
+        download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
+    except KeyError:
+      print("No valid info is available species: ", species)
 
-        return files
+    return files
 
-    def get_gtf_files(self, species: dict) -> list:
-        """
-        This method retrieve the gtf files for a specific specie object
-        :param species:
-        :return:
-        """
-        """
-          Generate GTF file name from the species info and download the GTF file
-        """
-        files = []
-        try:
-            file_name = '{}.{}.{}.gtf.gz'.format(species['name'][0].upper() + species['name'][1:], species['assembly'],
-                                                 species['release'], )
-            file_url = '{}/release-{}/gtf/{}/{}'.format(
-                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
-                    self.CONFIG_KEY_BASE_URL], species['release'], species['name'], file_name)
-            files.append(download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-        except KeyError:
-            self.get_logger().debug("No valid info is available species: ", species)
-
-        return files
-    
-    def get_vcf_files(self, species: dict) -> list:
-        """
-        This method retrieve the vcf file for a specific specie object
-        :param species:
-        :return:
-        """
-        """
-          Generate VCF file name from the species info and download it
-          ftp://ftp.ensembl.org/pub/release-97/variation/vcf/felis_catus/felis_catus_incl_consequences.vcf.gz
-        """
-        files = []
-        try:
-            file_name = '{}_incl_consequences.vcf.gz'.format(species['name'])
-            file_url = '{}/release-{}/variation/vcf/{}/'.format(
-                self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
-                    self.CONFIG_KEY_BASE_URL], species['release'], species['name'])
-            
-            downloaded_file = download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger())
-            if downloaded_file is not None:
-                files.append(downloaded_file)
-            
-            elif species['name']=='homo_sapiens':
-                "for humans the variants are stored per chromosome, so we need to download them all and combine them into one file here"
-                chrN=1
-                file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], chrN)
-                downloaded_file = download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger())
-                if downloaded_file is not None:
-                    "if chr1 is downloaded then try all others"
-                    files.append(downloaded_file)
-                    for chrN in range(2, 23):#chr2-22
-                        file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], chrN)
-                        files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-                    file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], 'X')
-                    files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-                    file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], 'Y')
-                    files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-                    file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], 'MT')
-                    files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
-                    
-        except KeyError:
-            self.get_logger().debug("No valid info is available species: ", species)
-            
-        return files
-    
+  def get_gtf_files(self, species: dict, grch37=False) -> list:
+    """
+      This method retrieve the gtf files for a specific specie object
+      :param grch37: if the GrCh37 genome assembly is desired enable to true
+      :param species: species to download the file.
+      :return:
+      """
+    files = []
+    try:
+      if grch37:
+        species['assembly'] = 'GRCh37'
+        species['release'] = '87'
+      file_name = '{}.{}.{}.gtf.gz'.format(species['name'][0].upper() + species['name'][1:], species['assembly'],
+                                           species['release'], )
+      file_url = '{}/release-{}/gtf/{}/{}'.format(
+        self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+          self.CONFIG_KEY_BASE_URL], species['release'], species['name'], file_name)
+      if grch37:
+        file_url = '{}/grch37/release-{}/gtf/{}/{}'.format(
+          self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+            self.CONFIG_KEY_BASE_URL], species['release'], species['name'], file_name)
+      files.append(
+        download_file(file_url, self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger()))
+
+    except KeyError:
+      self.get_logger().debug("No valid info is available species: ", species)
+
+    return files
+
+  def get_vcf_files(self, species: dict) -> list:
+    """
+      This method retrieve the vcf file for a specific specie object
+      :param species:
+      :return:
+      """
+    files = []
+    try:
+      file_name = '{}_incl_consequences.vcf.gz'.format(species['name'])
+      file_url = '{}/release-{}/variation/vcf/{}/'.format(
+        self.get_default_parameters()[self.CONFIG_KEY_DATA_DOWNLOADER][self.CONFIG_KEY_ENSEMBL_FTP][
+          self.CONFIG_KEY_BASE_URL], species['release'], species['name'])
+
+      downloaded_file = download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name,
+                                      self.get_logger())
+      if downloaded_file is not None:
+        files.append(downloaded_file)
+
+      elif species['name'] == 'homo_sapiens':
+        # for humans the variants are stored per chromosome, so we need to download them all and combine them into one file here"
+        chrN = 1
+        file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], chrN)
+        downloaded_file = download_file(file_url + file_name,
+                                        self.get_local_path_root_ensembl_repo() + '/' + file_name, self.get_logger())
+        if downloaded_file is not None:
+          # if chr1 is downloaded then try all others
+          files.append(downloaded_file)
+          for chrN in range(2, 23):  # chr2-22
+            file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], chrN)
+            files.append(
+              download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name,
+                            self.get_logger()))
+          file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], 'X')
+          files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name,
+                                     self.get_logger()))
+          file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], 'Y')
+          files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name,
+                                     self.get_logger()))
+          file_name = '{}_incl_consequences-chr{}.vcf.gz'.format(species['name'], 'MT')
+          files.append(download_file(file_url + file_name, self.get_local_path_root_ensembl_repo() + '/' + file_name,
+                                     self.get_logger()))
+
+    except KeyError:
+      self.get_logger().debug("No valid info is available species: ", species)
+
+    return files
```

### Comparing `pypgatk-0.0.8/pypgatk/ensembl/ensembl.py` & `pypgatk-0.0.9/pypgatk/ensembl/ensembl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,651 +1,691 @@
 import gffutils
 import vcf
 from Bio import SeqIO
 from Bio.Seq import Seq
-import sys
+
 from pypgatk.toolbox.general import ParameterConfiguration
 
 
 class EnsemblDataService(ParameterConfiguration):
-    CONFIG_KEY_VCF = "ensembl_translation"
-    INPUT_FASTA = "input_fasta"
-    TRANSLATION_TABLE = "translation_table"
-    MITO_TRANSLATION_TABLE = "mito_translation_table"
-    HEADER_VAR_PREFIX = "var_prefix"
-    REPORT_REFERENCE_SEQ = "report_ref_seq"
-    PROTEIN_DB_OUTPUT = "proteindb_output_file"
-    ANNOTATION_FIELD_NAME = "annotation_field_name"
-    AF_FIELD = "af_field"
-    AF_THRESHOLD = "af_threshold"
-    TRANSCRIPT_INDEX = "transcript_index"
-    CONSEQUENCE_INDEX = "consequence_index"
-    EXCLUDE_BIOTYPES = "exclude_biotypes"
-    EXCLUDE_CONSEQUENCES = "exclude_consequences"
-    SKIP_INCLUDING_ALL_CDS = "skip_including_all_cds"
-    INCLUDE_BIOTYPES = "include_biotypes"
-    INCLUDE_CONSEQUENCES = "include_consequences"
-    BIOTYPE_STR = "biotype_str"
-    SKIP_INCLUDING_ALL_CDSS = "skip_including_all_CDSs"
-    CONFIG_KEY_DATA = "ensembl_translation"
-    NUM_ORFS = "num_orfs"
-    NUM_ORFS_COMPLEMENT = "num_orfs_complement"
-    EXPRESSION_STR = "expression_str"
-    EXPRESSION_THRESH = "expression_thresh"
-    IGNORE_FILTERS = "ignore_filters"
-    ACCEPTED_FILTERS = "accepted_filters"
+  CONFIG_KEY_VCF = "ensembl_translation"
+  INPUT_FASTA = "input_fasta"
+  TRANSLATION_TABLE = "translation_table"
+  MITO_TRANSLATION_TABLE = "mito_translation_table"
+  HEADER_VAR_PREFIX = "var_prefix"
+  REPORT_REFERENCE_SEQ = "report_ref_seq"
+  PROTEIN_DB_OUTPUT = "proteindb_output_file"
+  ANNOTATION_FIELD_NAME = "annotation_field_name"
+  AF_FIELD = "af_field"
+  AF_THRESHOLD = "af_threshold"
+  TRANSCRIPT_INDEX = "transcript_index"
+  CONSEQUENCE_INDEX = "consequence_index"
+  EXCLUDE_BIOTYPES = "exclude_biotypes"
+  EXCLUDE_CONSEQUENCES = "exclude_consequences"
+  SKIP_INCLUDING_ALL_CDS = "skip_including_all_cds"
+  INCLUDE_BIOTYPES = "include_biotypes"
+  INCLUDE_CONSEQUENCES = "include_consequences"
+  BIOTYPE_STR = "biotype_str"
+  SKIP_INCLUDING_ALL_CDSS = "skip_including_all_CDSs"
+  CONFIG_KEY_DATA = "ensembl_translation"
+  NUM_ORFS = "num_orfs"
+  NUM_ORFS_COMPLEMENT = "num_orfs_complement"
+  EXPRESSION_STR = "expression_str"
+  EXPRESSION_THRESH = "expression_thresh"
+  IGNORE_FILTERS = "ignore_filters"
+  ACCEPTED_FILTERS = "accepted_filters"
 
-    def __init__(self, config_file, pipeline_arguments):
-        """
+  def __init__(self, config_file, pipeline_arguments):
+    """
         Init the class with the specific parameters.
         :param config_file configuration file
         :param pipeline_arguments pipelines arguments
         """
-        super(EnsemblDataService, self).__init__(self.CONFIG_KEY_DATA, config_file,
-                                                 pipeline_arguments)
+    super(EnsemblDataService, self).__init__(self.CONFIG_KEY_DATA, config_file,
+                                             pipeline_arguments)
 
-        self._proteindb_output = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.PROTEIN_DB_OUTPUT]
-        if self.PROTEIN_DB_OUTPUT in self.get_pipeline_parameters():
-            self._proteindb_output = self.get_pipeline_parameters()[self.PROTEIN_DB_OUTPUT]
-
-        self._translation_table = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.TRANSLATION_TABLE]
-        if self.TRANSLATION_TABLE in self.get_pipeline_parameters():
-            self._translation_table = self.get_pipeline_parameters()[self.TRANSLATION_TABLE]
-
-        self._mito_translation_table = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.MITO_TRANSLATION_TABLE]
-        if self.MITO_TRANSLATION_TABLE in self.get_pipeline_parameters():
-            self._mito_translation_table = self.get_pipeline_parameters()[self.MITO_TRANSLATION_TABLE]
-
-        self._header_var_prefix = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.HEADER_VAR_PREFIX]
-        if self.HEADER_VAR_PREFIX in self.get_pipeline_parameters():
-            self._header_var_prefix = self.get_pipeline_parameters()[self.HEADER_VAR_PREFIX]
-
-        self._report_reference_seq = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.REPORT_REFERENCE_SEQ]
-        if self.REPORT_REFERENCE_SEQ in self.get_pipeline_parameters():
-            self._report_reference_seq = self.get_pipeline_parameters()[self.REPORT_REFERENCE_SEQ]
-
-        self._annotation_field_name = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.ANNOTATION_FIELD_NAME]
-        if self.ANNOTATION_FIELD_NAME in self.get_pipeline_parameters():
-            self._annotation_field_name = self.get_pipeline_parameters()[self.ANNOTATION_FIELD_NAME]
-
-        self._af_field = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.AF_FIELD]
-        if self.AF_FIELD in self.get_pipeline_parameters():
-            self._af_field = self.get_pipeline_parameters()[self.AF_FIELD]
-
-        self._af_threshold = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.AF_THRESHOLD]
-        if self.AF_THRESHOLD in self.get_pipeline_parameters():
-            self._af_threshold = self.get_pipeline_parameters()[self.AF_THRESHOLD]
-
-        self._transcript_index = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.TRANSCRIPT_INDEX]
-        if self.TRANSCRIPT_INDEX in self.get_pipeline_parameters():
-            self._transcript_index = self.get_pipeline_parameters()[self.TRANSCRIPT_INDEX]
-
-        self._consequence_index = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.CONSEQUENCE_INDEX]
-        if self.CONSEQUENCE_INDEX in self.get_pipeline_parameters():
-            self._consequence_index = self.get_pipeline_parameters()[self.CONSEQUENCE_INDEX]
-
-        self._exclude_biotypes = self.get_multiple_options(
-            self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.EXCLUDE_BIOTYPES])
-        if self.EXCLUDE_BIOTYPES in self.get_pipeline_parameters():
-            self._exclude_biotypes = self.get_multiple_options(self.get_pipeline_parameters()[self.EXCLUDE_BIOTYPES])
-
-        self._exclude_consequences = self.get_multiple_options(
-            self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.EXCLUDE_CONSEQUENCES])
-        if self.EXCLUDE_CONSEQUENCES in self.get_pipeline_parameters():
-            self._exclude_consequences = self.get_multiple_options(
-                self.get_pipeline_parameters()[self.EXCLUDE_CONSEQUENCES])
-
-        self._skip_including_all_cds = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.SKIP_INCLUDING_ALL_CDS]
-        if self.SKIP_INCLUDING_ALL_CDS in self.get_pipeline_parameters():
-            self._skip_including_all_cds = self.get_pipeline_parameters()[self.SKIP_INCLUDING_ALL_CDS]
-
-        self._include_biotypes = self.get_multiple_options(
-            self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.INCLUDE_BIOTYPES])
-        if self.INCLUDE_BIOTYPES in self.get_pipeline_parameters():
-            self._include_biotypes = self.get_multiple_options(self.get_pipeline_parameters()[self.INCLUDE_BIOTYPES])
-
-        self._include_consequences = self.get_multiple_options(
-            self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.INCLUDE_CONSEQUENCES])
-        if self.INCLUDE_CONSEQUENCES in self.get_pipeline_parameters():
-            self._include_consequences = self.get_multiple_options(
-                self.get_pipeline_parameters()[self.INCLUDE_CONSEQUENCES])
-
-        self._biotype_str = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.BIOTYPE_STR]
-        if self.BIOTYPE_STR in self.get_pipeline_parameters():
-            self._biotype_str = self.get_pipeline_parameters()[self.BIOTYPE_STR]
-
-        self._num_orfs = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.NUM_ORFS]
-        if self.NUM_ORFS in self.get_pipeline_parameters():
-            self._num_orfs = self.get_pipeline_parameters()[self.NUM_ORFS]
-
-        self._num_orfs_complement = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.NUM_ORFS_COMPLEMENT]
-        if self.NUM_ORFS_COMPLEMENT in self.get_pipeline_parameters():
-            self._num_orfs_complement = self.get_pipeline_parameters()[self.NUM_ORFS_COMPLEMENT]
-
-        self._expression_str = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.EXPRESSION_STR]
-        if self.EXPRESSION_STR in self.get_pipeline_parameters():
-            self._expression_str = self.get_pipeline_parameters()[self.EXPRESSION_STR]
-
-        self._expression_thresh = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.EXPRESSION_THRESH]
-        if self.EXPRESSION_THRESH in self.get_pipeline_parameters():
-            self._expression_thresh = self.get_pipeline_parameters()[self.EXPRESSION_THRESH]
-
-        self._ignore_filters = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
-            self.IGNORE_FILTERS]
-        if self.IGNORE_FILTERS in self.get_pipeline_parameters():
-            self._ignore_filters = self.get_pipeline_parameters()[self.IGNORE_FILTERS]
-
-        self._accepted_filters = self.get_multiple_options(
-            self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.ACCEPTED_FILTERS])
-        if self.ACCEPTED_FILTERS in self.get_pipeline_parameters():
-            self._accepted_filters = self.get_multiple_options(
-                self.get_pipeline_parameters()[self.ACCEPTED_FILTERS])
+    self._proteindb_output = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.PROTEIN_DB_OUTPUT]
+    if self.PROTEIN_DB_OUTPUT in self.get_pipeline_parameters():
+      self._proteindb_output = self.get_pipeline_parameters()[self.PROTEIN_DB_OUTPUT]
+
+    self._translation_table = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.TRANSLATION_TABLE]
+    if self.TRANSLATION_TABLE in self.get_pipeline_parameters():
+      self._translation_table = self.get_pipeline_parameters()[self.TRANSLATION_TABLE]
+
+    self._mito_translation_table = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.MITO_TRANSLATION_TABLE]
+    if self.MITO_TRANSLATION_TABLE in self.get_pipeline_parameters():
+      self._mito_translation_table = self.get_pipeline_parameters()[self.MITO_TRANSLATION_TABLE]
+
+    self._header_var_prefix = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.HEADER_VAR_PREFIX]
+    if self.HEADER_VAR_PREFIX in self.get_pipeline_parameters():
+      self._header_var_prefix = self.get_pipeline_parameters()[self.HEADER_VAR_PREFIX]
+
+    self._report_reference_seq = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.REPORT_REFERENCE_SEQ]
+    if self.REPORT_REFERENCE_SEQ in self.get_pipeline_parameters():
+      self._report_reference_seq = self.get_pipeline_parameters()[self.REPORT_REFERENCE_SEQ]
+
+    self._annotation_field_name = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.ANNOTATION_FIELD_NAME]
+    if self.ANNOTATION_FIELD_NAME in self.get_pipeline_parameters():
+      self._annotation_field_name = self.get_pipeline_parameters()[self.ANNOTATION_FIELD_NAME]
+
+    self._af_field = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.AF_FIELD]
+    if self.AF_FIELD in self.get_pipeline_parameters():
+      self._af_field = self.get_pipeline_parameters()[self.AF_FIELD]
+
+    self._af_threshold = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.AF_THRESHOLD]
+    if self.AF_THRESHOLD in self.get_pipeline_parameters():
+      self._af_threshold = self.get_pipeline_parameters()[self.AF_THRESHOLD]
+
+    self._transcript_index = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.TRANSCRIPT_INDEX]
+    if self.TRANSCRIPT_INDEX in self.get_pipeline_parameters():
+      self._transcript_index = self.get_pipeline_parameters()[self.TRANSCRIPT_INDEX]
+
+    self._consequence_index = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.CONSEQUENCE_INDEX]
+    if self.CONSEQUENCE_INDEX in self.get_pipeline_parameters():
+      self._consequence_index = self.get_pipeline_parameters()[self.CONSEQUENCE_INDEX]
+
+    self._exclude_biotypes = self.get_multiple_options(
+      self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.EXCLUDE_BIOTYPES])
+    if self.EXCLUDE_BIOTYPES in self.get_pipeline_parameters():
+      self._exclude_biotypes = self.get_multiple_options(self.get_pipeline_parameters()[self.EXCLUDE_BIOTYPES])
+
+    self._exclude_consequences = self.get_multiple_options(
+      self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.EXCLUDE_CONSEQUENCES])
+    if self.EXCLUDE_CONSEQUENCES in self.get_pipeline_parameters():
+      self._exclude_consequences = self.get_multiple_options(
+        self.get_pipeline_parameters()[self.EXCLUDE_CONSEQUENCES])
+
+    self._skip_including_all_cds = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.SKIP_INCLUDING_ALL_CDS]
+    if self.SKIP_INCLUDING_ALL_CDS in self.get_pipeline_parameters():
+      self._skip_including_all_cds = self.get_pipeline_parameters()[self.SKIP_INCLUDING_ALL_CDS]
+
+    self._include_biotypes = self.get_multiple_options(
+      self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.INCLUDE_BIOTYPES])
+    if self.INCLUDE_BIOTYPES in self.get_pipeline_parameters():
+      self._include_biotypes = self.get_multiple_options(self.get_pipeline_parameters()[self.INCLUDE_BIOTYPES])
+
+    self._include_consequences = self.get_multiple_options(
+      self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.INCLUDE_CONSEQUENCES])
+    if self.INCLUDE_CONSEQUENCES in self.get_pipeline_parameters():
+      self._include_consequences = self.get_multiple_options(
+        self.get_pipeline_parameters()[self.INCLUDE_CONSEQUENCES])
+
+    self._biotype_str = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.BIOTYPE_STR]
+    if self.BIOTYPE_STR in self.get_pipeline_parameters():
+      self._biotype_str = self.get_pipeline_parameters()[self.BIOTYPE_STR]
+
+    self._num_orfs = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.NUM_ORFS]
+    if self.NUM_ORFS in self.get_pipeline_parameters():
+      self._num_orfs = self.get_pipeline_parameters()[self.NUM_ORFS]
+
+    self._num_orfs_complement = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.NUM_ORFS_COMPLEMENT]
+    if self.NUM_ORFS_COMPLEMENT in self.get_pipeline_parameters():
+      self._num_orfs_complement = self.get_pipeline_parameters()[self.NUM_ORFS_COMPLEMENT]
+
+    self._expression_str = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.EXPRESSION_STR]
+    if self.EXPRESSION_STR in self.get_pipeline_parameters():
+      self._expression_str = self.get_pipeline_parameters()[self.EXPRESSION_STR]
+
+    self._expression_thresh = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.EXPRESSION_THRESH]
+    if self.EXPRESSION_THRESH in self.get_pipeline_parameters():
+      self._expression_thresh = self.get_pipeline_parameters()[self.EXPRESSION_THRESH]
+
+    self._ignore_filters = self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][
+      self.IGNORE_FILTERS]
+    if self.IGNORE_FILTERS in self.get_pipeline_parameters():
+      self._ignore_filters = self.get_pipeline_parameters()[self.IGNORE_FILTERS]
+
+    self._accepted_filters = self.get_multiple_options(
+      self.get_default_parameters()[self.CONFIG_KEY_DATA][self.CONFIG_KEY_VCF][self.ACCEPTED_FILTERS])
+    if self.ACCEPTED_FILTERS in self.get_pipeline_parameters():
+      self._accepted_filters = self.get_multiple_options(
+        self.get_pipeline_parameters()[self.ACCEPTED_FILTERS])
 
-    def three_frame_translation(self, input_fasta):
-        """
+  def three_frame_translation(self, input_fasta):
+    """
         This function translate a transcriptome into a 3'frame translation protein sequence database
         :param input_fasta: fasta input file
         :return:
         """
 
-        input_handle = open(input_fasta, 'r')
-        output_handle = open(self._proteindb_output, 'rw')
+    input_handle = open(input_fasta, 'r')
+    output_handle = open(self._proteindb_output, 'w')
 
-        for record in SeqIO.parse(input_handle, 'fasta'):
-            seq = record.seq
-            RF1 = seq.translate(table=self._translation_table)
-            RF2 = seq[1::].translate(table=self._translation_table)
-            RF3 = seq[2::].translate(table=self._translation_table)
-
-            if record.id == "":
-                print("skip entries without id", record.description)
-                continue
-            output_handle.write("%s\n%s\n" % ('>' + record.id + '_RF1', RF1))
-            output_handle.write("%s\n%s\n" % ('>' + record.id + '_RF2', RF2))
-            output_handle.write("%s\n%s\n" % ('>' + record.id + '_RF3', RF3))
-
-    @staticmethod
-    def get_multiple_options(options_str: str):
-        """
+    for record in SeqIO.parse(input_handle, 'fasta'):
+      seq = record.seq
+      RF1 = seq.translate(table=self._translation_table)
+      RF2 = seq[1::].translate(table=self._translation_table)
+      RF3 = seq[2::].translate(table=self._translation_table)
+
+      if record.id == "":
+        print("skip entries without id", record.description)
+        continue
+      output_handle.write("%s\n%s\n" % ('>' + record.id + '_RF1', RF1))
+      output_handle.write("%s\n%s\n" % ('>' + record.id + '_RF2', RF2))
+      output_handle.write("%s\n%s\n" % ('>' + record.id + '_RF3', RF3))
+
+  @staticmethod
+  def get_multiple_options(options_str: str):
+    """
         This method takes an String like option1, option2, ... and produce and array [option1, option2,... ]
         :param options_str:
         :return: Array
         """
-        return list(map(lambda x: x.strip(), options_str.split(",")))
+    return list(map(lambda x: x.strip(), options_str.split(",")))
 
-    @staticmethod
-    def check_overlap(var_start, var_end, features_info=[[0, 1, 'type']]):
-        """
+  @staticmethod
+  def check_overlap(var_start, var_end, features_info=None):
+    """
         This function returns true when the variant overlaps any of the features
         :param var_start: Start location
         :param var_end: End location
-        :param features_info: Feature information
+        :param features_info: Feature information (default = [[0, 1, 'type']])
         :return:
         """
-        if var_start == -1:
-            return True
-        # check if the var overlaps any of the features
-        for feature_pos in features_info:
-            pep_start = feature_pos[0]
-            pep_end = feature_pos[1]
-            if var_start <= pep_start <= var_end:  # fully contained or partial overlap from the end
-                return True
-            elif var_start <= pep_end <= var_end:  # partial overlap in the begining
-                return True
-            elif pep_start <= var_start and pep_end >= var_end:  # fully covered
-                return True
-        return False
-
-    @staticmethod
-    def get_altseq(ref_seq, ref_allele, var_allele, var_pos, strand, features_info, cds_info=[]):
-        """
-        the given sequence in the fasta file represents all exons of the transcript combined.
-        for protein coding genes, the CDS is specified therefore the sequence position has to be
-        calculated based on the CDS's positions
-        However, for non-protein coding genes, the whole sequence is used
-        """
-        alt_seq = ""
-        if len(cds_info) == 2:
-            start_coding_index = cds_info[0] - 1  # it should be index not pos
-            stop_coding_index = cds_info[1]  # get end position of the  last cds
-        else:
-            start_coding_index = 0
-            total_len = 0
-            for x in features_info:
-                total_len += x[1] - x[0] + 1
-            stop_coding_index = total_len  # the features are sorted by end therefroe the end pos of the last item is the last coding nc
-
-        if strand == '-':  # ge the correct orientation, because exons are oredered based on their position
-            ref_seq = ref_seq[
-                      ::-1]  # in order to calculate from the first base of the first feature (sorted by genomic coordinates)
-            ref_allele = ref_allele.complement()  # the reverse will be done on return
-            var_allele = var_allele.complement()  # the reverse will be done on return
-
-        ref_seq = ref_seq[
-                  start_coding_index:stop_coding_index]  # just keep the coding regions (mostly effective in case of protein-coding genes)
-        nc_index = 0
-        if len(ref_allele) == len(var_allele) or ref_allele[0] == var_allele[0]:
-            for feature in features_info:  # for every exon, cds or stop codon
-                if var_pos in range(feature[0], feature[
-                                                    1] + 1):  # get index of the var relative to the position of the overlapping feature in the coding region
-                    var_index_in_cds = nc_index + (var_pos - feature[0])
-                    # modify the coding reference sequence accoding to the var_allele
-                    c = len(ref_allele)
-                    alt_seq = ref_seq[0:var_index_in_cds] + var_allele + ref_seq[
-                                                                         var_index_in_cds + c::]  # variant and ref strand??
-                    if strand == '-':
-                        return ref_seq[::-1], alt_seq[::-1]
-                    else:
-                        return ref_seq, alt_seq
-
-                nc_index += (feature[1] - feature[0] + 1)
-
-        return ref_seq, alt_seq
-
-    @staticmethod
-    def parse_gtf(gene_annotations_gtf, gtf_db_file):
-        """
+    if features_info is None:
+      features_info = [[0, 1, 'type']]
+    if var_start == -1:
+      return True
+    # check if the var overlaps any of the features
+    for feature_pos in features_info:
+      pep_start = feature_pos[0]
+      pep_end = feature_pos[1]
+      if var_start <= pep_start <= var_end:  # fully contained or partial overlap from the end
+        return True
+      elif var_start <= pep_end <= var_end:  # partial overlap in the begining
+        return True
+      elif pep_start <= var_start and pep_end >= var_end:  # fully covered
+        return True
+    return False
+
+  @staticmethod
+  def get_altseq(ref_seq, ref_allele, var_allele, var_pos, strand, features_info, cds_info=None):
+    """
+    The given sequence in the fasta file represents all exons of the transcript combined.
+    for protein coding genes, the CDS is specified therefore the sequence position has to be
+    calculated based on the CDS's positions
+    However, for non-protein coding genes, the whole sequence is used
+    :param ref_seq:
+    :param ref_allele:
+    :param var_allele:
+    :param var_pos:
+    :param strand:
+    :param features_info:
+    :param cds_info:
+    :return:
+    """
+    if cds_info is None:
+      cds_info = []
+    alt_seq = ""
+    if len(cds_info) == 2:
+      start_coding_index = cds_info[0] - 1  # it should be index not pos
+      stop_coding_index = cds_info[1]  # get end position of the  last cds
+    else:
+      start_coding_index = 0
+      total_len = 0
+      for x in features_info:
+        total_len += x[1] - x[0] + 1
+      stop_coding_index = total_len  # the features are sorted by end therefroe the end pos of the last item is the last coding nc
+
+    if strand == '-':  # ge the correct orientation, because exons are oredered based on their position
+      ref_seq = ref_seq[
+                ::-1]  # in order to calculate from the first base of the first feature (sorted by genomic coordinates)
+      ref_allele = ref_allele.complement()  # the reverse will be done on return
+      var_allele = var_allele.complement()  # the reverse will be done on return
+
+    ref_seq = ref_seq[
+              start_coding_index:stop_coding_index]  # just keep the coding regions (mostly effective in case of protein-coding genes)
+    nc_index = 0
+    if len(ref_allele) == len(var_allele) or ref_allele[0] == var_allele[0]:
+      for feature in features_info:  # for every exon, cds or stop codon
+        if var_pos in range(feature[0], feature[
+                                          1] + 1):  # get index of the var relative to the position of the overlapping feature in the coding region
+          var_index_in_cds = nc_index + (var_pos - feature[0])
+          # modify the coding reference sequence accoding to the var_allele
+          c = len(ref_allele)
+          alt_seq = ref_seq[0:var_index_in_cds] + var_allele + ref_seq[
+                                                               var_index_in_cds + c::]  # variant and ref strand??
+          if strand == '-':
+            return ref_seq[::-1], alt_seq[::-1]
+          else:
+            return ref_seq, alt_seq
+
+        nc_index += (feature[1] - feature[0] + 1)
+
+    return ref_seq, alt_seq
+
+  @staticmethod
+  def parse_gtf(gene_annotations_gtf, gtf_db_file):
+    """
         Convert GTF file into a FeatureDB
         :param gene_annotations_gtf:
         :param gtf_db_file:
         :return:
         """
-        try:
-            gffutils.create_db(gene_annotations_gtf, gtf_db_file, merge_strategy="create_unique",
-                               keep_order=True, disable_infer_transcripts=True, disable_infer_genes=True,
-                               verbose=True,
-                               force=False)
-        except:  # already exists
-            print("already exists", gtf_db_file)
-            pass
-
-        db = gffutils.FeatureDB(gtf_db_file)
-        return db
-
-    @staticmethod
-    def get_features(db, feature_id, biotype_str, feature_types=['exon']):
-        """
+    try:
+      gffutils.create_db(gene_annotations_gtf, gtf_db_file, merge_strategy="create_unique",
+                         keep_order=True, disable_infer_transcripts=True, disable_infer_genes=True,
+                         verbose=True,
+                         force=False)
+    except Exception as e:  # already exists
+      print("Databae already exists" + str(e), gtf_db_file)
+
+    db = gffutils.FeatureDB(gtf_db_file)
+    return db
+
+  @staticmethod
+  def get_features(db, feature_id, biotype_str, feature_types=None):
+    """
         Get chr, genomic positions, strand and biotype for feature_id
         also genomic positions for all its elements (exons/cds&start_codon)
         :param db:
         :param feature_id:
         :param biotype_str:
         :param feature_types:
         :return:
         """
-        try:
-            feature = db[feature_id]
-        except gffutils.exceptions.FeatureNotFoundError: #remove version number from the ID
-            try:
-                feature = db[feature_id.split('.')[0]]
-            except gffutils.exceptions.FeatureNotFoundError:
-                print("""Feature {} found in fasta file but not in gtf file. Check that the fasta file and the gtf files match.
-                        A common issue is when the fasta file have chromosome patches but not the gtf""".format(feature_id))
-                return None, None, None, None
-        coding_features = []
-        features = db.children(feature, featuretype=feature_types, order_by='end')
-        for f in features:
-            f_type = f.featuretype
-            coding_features.append([f.start, f.end, f_type])
-        return feature.chrom, feature.strand, coding_features, feature.attributes[biotype_str][0]
-
-    @staticmethod
-    def get_orfs_vcf(ref_seq: str, alt_seq: str, translation_table: int, num_orfs=1):
-        """
+    if feature_types is None:
+      feature_types = ['exon']
+    try:
+      feature = db[feature_id]
+    except gffutils.exceptions.FeatureNotFoundError:  # remove version number from the ID
+      try:
+        feature = db[feature_id.split('.')[0]]
+      except gffutils.exceptions.FeatureNotFoundError:
+        print("""Feature {} found in fasta file but not in gtf file. Check that the fasta file and the gtf files match.
+                        A common issue is when the fasta file have chromosome patches but not the gtf""".format(
+          feature_id))
+        return None, None, None, None
+    coding_features = []
+    features = db.children(feature, featuretype=feature_types, order_by='end')
+    for f in features:
+      f_type = f.featuretype
+      coding_features.append([f.start, f.end, f_type])
+    return feature.chrom, feature.strand, coding_features, feature.attributes[biotype_str][0]
+
+  @staticmethod
+  def get_orfs_vcf(ref_seq: str, alt_seq: str, translation_table: int, num_orfs=1):
+    """
         Translate the coding_ref and the coding_alt into ORFs
         :param ref_seq:
         :param alt_seq:
         :param translation_table:
         :param num_orfs:
         :return:
         """
 
-        ref_orfs = []
-        alt_orfs = []
-        for n in range(0, num_orfs):
-            ref_orfs.append(ref_seq[n::].translate(translation_table))
-            alt_orfs.append(alt_seq[n::].translate(translation_table))
-
-        return ref_orfs, alt_orfs
-
-    @staticmethod
-    def get_orfs_dna(ref_seq: str, translation_table: int, num_orfs: int, num_orfs_complement: int, to_stop: bool):
-        """translate the coding_ref into ORFs"""
-
-        ref_orfs = []
-        for n in range(0, num_orfs):
-            ref_orfs.append(ref_seq[n::].translate(translation_table, to_stop=to_stop))
+    ref_orfs = []
+    alt_orfs = []
+    for n in range(0, num_orfs):
+      ref_orfs.append(ref_seq[n::].translate(translation_table))
+      alt_orfs.append(alt_seq[n::].translate(translation_table))
+
+    return ref_orfs, alt_orfs
+
+  @staticmethod
+  def get_orfs_dna(ref_seq: str, translation_table: int, num_orfs: int, num_orfs_complement: int, to_stop: bool):
+    """translate the coding_ref into ORFs"""
+
+    ref_orfs = []
+    for n in range(0, num_orfs):
+      ref_orfs.append(ref_seq[n::].translate(translation_table, to_stop=to_stop))
+
+    rev_ref_seq = ref_seq.reverse_complement()
+    for n in range(0, num_orfs_complement):
+      ref_orfs.append(rev_ref_seq[n::].translate(translation_table, to_stop=to_stop))
 
-        rev_ref_seq = ref_seq.reverse_complement()
-        for n in range(0, num_orfs_complement):
-            ref_orfs.append(rev_ref_seq[n::].translate(translation_table, to_stop=to_stop))
+    return ref_orfs
 
-        return ref_orfs
-
-    def dnaseq_to_proteindb(self, input_fasta):
-        """
+  def dnaseq_to_proteindb(self, input_fasta):
+    """
         translates DNA sequences to protein sequences
         :param input_fasta:
         :return:
         """
 
-        seq_dict = SeqIO.index(input_fasta, "fasta")
+    seq_dict = SeqIO.index(input_fasta, "fasta")
 
-        with open(self._proteindb_output, 'w') as prots_fn:
-            for record_id in seq_dict.keys():
+    with open(self._proteindb_output, 'w') as prots_fn:
+      for record_id in seq_dict.keys():
 
-                ref_seq = seq_dict[
-                    record_id].seq  # get the seq and desc for the record from the fasta of the gtf
-                desc = str(seq_dict[record_id].description)
-
-                key_values = {}  # extract key=value in the desc into a dict
-                sep = ' '
-                if '|' in desc:
-                    sep = '|'
-                for value in desc.split(sep):
-                    if value.split('=')[0]=='cds' or value.split(':')[0]=='cds':
-                        value.replace('cds', 'CDS')
-                    if '=' in value:
-                        key_values[value.split('=')[0]] = value.split('=')[1]
-                    elif ':' in value:
-                        key_values[value.split(':')[0]] = value.split(':')[1]
-                    elif value.split('=')[0]=='CDS': #when only it is specified to be a CDS, it means the whole sequence to be used
-                        key_values[value.split('=')[0]] = '{}-{}'.format(1, len(ref_seq))
-
-                feature_biotype = ""
-                if self._biotype_str:
-                    try:
-                        feature_biotype = key_values[self._biotype_str]
-                    except KeyError:
-                        msg = "Biotype info was not found in the header using {} for record {} {}".format(self._biotype_str, record_id, desc)
-                        self.get_logger().debug(msg)
-
-                # only include features that have the specified biotypes or they have CDSs info
-                if 'CDS' in key_values.keys() and (
-                        not self._skip_including_all_cds or 'altORFs' in self._include_biotypes):
-                    pass
-                elif self._biotype_str and (feature_biotype == "" or (feature_biotype in self._exclude_biotypes or
-                                               (
-                                                       feature_biotype not in self._include_biotypes and self._include_biotypes != [
-                                                   'all']))):
-                    continue
-
-                # check wether to filter on expression and if it passes
-                if self._expression_str:
-                    try:
-                        if float(key_values[self._expression_str]) < self._expression_thresh:
-                            continue
-                    except KeyError:
-                        msg = "Expression information not found in the fasta header with expression_str: {} for record {} {}".format(self._expression_str, record_id, desc)
-                        self.get_logger().debug(msg)
-                        continue
-                    except TypeError:
-                        msg = "Expression value is not of valid type (float) at record: {} {}".format(record_id, key_values[self._expression_str])
-                        self.get_logger().debug(msg)
-                        continue
-
-                # translate the whole sequences (3 ORFs) for non CDS sequences and not take alt_ORFs for CDSs
-                if 'CDS' not in key_values.keys() or ('CDS' in key_values.keys() and
-                                                      ('altORFs' in self._include_biotypes or
-                                                       self._include_biotypes == ['all'])):
-                    ref_orfs = self.get_orfs_dna(ref_seq, self._translation_table, self._num_orfs,
-                                                 self._num_orfs_complement, to_stop=False)
-                    print(self._header_var_prefix)
-                    self.write_output(seq_id=self._header_var_prefix+record_id, desc=desc, seqs=ref_orfs, prots_fn=prots_fn)
-
-                # also allow for direct translation of the CDS, when the cds info exists in the fasta header skip_including_all_cds is false
-                if 'CDS' in key_values.keys() and not self._skip_including_all_cds:
-                    try:
-                        cds_info = [int(x) for x in key_values['CDS'].split('-')]
-                        ref_seq = ref_seq[cds_info[0] - 1:cds_info[1]]
-                        ref_orfs = self.get_orfs_dna(ref_seq, self._translation_table, 1, 0, to_stop=True)
-                        self.write_output(seq_id=record_id, desc=desc, seqs=ref_orfs, prots_fn=prots_fn)
-                    except (ValueError, IndexError, KeyError):
-                        print("Could not extra cds position from fasta header for: ", record_id, desc)
-
-        return self._proteindb_output
-
-    @staticmethod
-    def get_key(fasta_header):
-        return fasta_header.split('|')[0].split(' ')[0]
+        ref_seq = seq_dict[record_id].seq  # get the seq and desc for the record from the fasta of the gtf
+        desc = str(seq_dict[record_id].description)
 
-    def vcf_to_proteindb(self, vcf_file, input_fasta, gene_annotations_gtf):
-        """
+        key_values = {}  # extract key=value in the desc into a dict
+        sep = ' '
+        if '|' in desc:
+          sep = '|'
+        for value in desc.split(sep):
+          if value.split('=')[0] == 'cds' or value.split(':')[0] == 'cds':
+            value.replace('cds', 'CDS')
+          if '=' in value:
+            key_values[value.split('=')[0]] = value.split('=')[1]
+          elif ':' in value:
+            key_values[value.split(':')[0]] = value.split(':')[1]
+          elif value.split('=')[
+            0] == 'CDS':  # when only it is specified to be a CDS, it means the whole sequence to be used
+            key_values[value.split('=')[0]] = '{}-{}'.format(1, len(ref_seq))
+
+        feature_biotype = ""
+        if self._biotype_str:
+          try:
+            feature_biotype = key_values[self._biotype_str]
+          except KeyError:
+            msg = "Biotype info was not found in the header using {} for record {} {}".format(self._biotype_str,
+                                                                                              record_id, desc)
+            self.get_logger().debug(msg)
+
+        # only include features that have the specified biotypes or they have CDSs info
+        if 'CDS' in key_values.keys() and (
+          not self._skip_including_all_cds or 'altORFs' in self._include_biotypes):
+          pass
+        elif self._biotype_str and (feature_biotype == "" or (feature_biotype in self._exclude_biotypes or
+                                                              (
+                                                                feature_biotype not in self._include_biotypes and self._include_biotypes != [
+                                                                'all']))):
+          continue
+
+        # check wether to filter on expression and if it passes
+        if self._expression_str:
+          try:
+            if float(key_values[self._expression_str]) < self._expression_thresh:
+              continue
+          except KeyError:
+            msg = "Expression information not found in the fasta header with expression_str: {} for record {} {}".format(
+              self._expression_str, record_id, desc)
+            self.get_logger().debug(msg)
+            continue
+          except TypeError:
+            msg = "Expression value is not of valid type (float) at record: {} {}".format(record_id, key_values[
+              self._expression_str])
+            self.get_logger().debug(msg)
+            continue
+
+        # translate the whole sequences (3 ORFs) for non CDS sequences and not take alt_ORFs for CDSs
+        if 'CDS' not in key_values.keys() or ('CDS' in key_values.keys() and
+                                              ('altORFs' in self._include_biotypes or
+                                               self._include_biotypes == ['all'])):
+          ref_orfs = self.get_orfs_dna(ref_seq, self._translation_table, self._num_orfs,
+                                       self._num_orfs_complement, to_stop=False)
+          print(self._header_var_prefix)
+          self.write_output(seq_id=self._header_var_prefix + record_id, desc=desc, seqs=ref_orfs, prots_fn=prots_fn)
+
+        # also allow for direct translation of the CDS, when the cds info exists in the fasta header skip_including_all_cds is false
+        if 'CDS' in key_values.keys() and not self._skip_including_all_cds:
+          try:
+            cds_info = [int(x) for x in key_values['CDS'].split('-')]
+            ref_seq = ref_seq[cds_info[0] - 1:cds_info[1]]
+            ref_orfs = self.get_orfs_dna(ref_seq, self._translation_table, 1, 0, to_stop=True)
+            self.write_output(seq_id=record_id, desc=desc, seqs=ref_orfs, prots_fn=prots_fn)
+          except (ValueError, IndexError, KeyError):
+            print("Could not extra cds position from fasta header for: ", record_id, desc)
+
+    return self._proteindb_output
+
+  @staticmethod
+  def get_key(fasta_header):
+    return fasta_header.split('|')[0].split(' ')[0]
+
+  def vcf_to_proteindb(self, vcf_file, input_fasta, gene_annotations_gtf):
+    """
         Generate peps for variants by modifying sequences of affected transcripts (VCF - VEP annotated).
         It only considers variants within potential coding regions of the transcript
         (CDSs & stop codons for protein-coding genes, exons for non-protein coding genes).
         :param vcf_file:
         :param input_fasta:
         :param gene_annotations_gtf:
         :return:
         """
 
-        db = self.parse_gtf(gene_annotations_gtf, gene_annotations_gtf.replace('.gtf', '.db'))
+    db = self.parse_gtf(gene_annotations_gtf, gene_annotations_gtf.replace('.gtf', '.db'))
 
-        transcripts_dict = SeqIO.index(input_fasta, "fasta", key_function=self.get_key)
-        # handle cases where the transcript has version in the GTF but not in the VCF
-        transcript_id_mapping = {k.split('.')[0]: k for k in transcripts_dict.keys()}
-        with open(self._proteindb_output, 'w') as prots_fn:
-            vcf_reader = vcf.Reader(open(vcf_file, 'r'))
-
-            for record in vcf_reader:
-                if record.ALT==[None] or record.REF==[None]:
-                    msg = "Invalid VCF record, skipping: {}".format(record)
-                    self.get_logger().debug(msg)
-                    continue
-                if not self._ignore_filters:
-                    if record.FILTER:  # if not PASS: None and empty means PASS
-                        if not (set(record.FILTER[0].split(',')) <= set(self._accepted_filters)):
-                            continue
-
-                # only process variants above a given allele frequency threshold if the AF string is not empty
-                if self._af_field:
-                    # get AF from the INFO field
-                    try:
-                        af = float(record.INFO[self._af_field])
-                    except TypeError:
-                        af = float(record.INFO[self._af_field][0])
-                    except KeyError:
-                        continue
-
-                    # check if the AF passed the threshold
-                    if af < self._af_threshold:
-                        continue
-
-                trans_table = self._translation_table
-                consequences = []
-                if str(record.CHROM).lstrip('chr').upper() in ['M', 'MT']:
-                    trans_table = self._mito_translation_table
-
-                processed_transcript_allele = []
-
-                for transcript_record in record.INFO[self._annotation_field_name]:
-                    transcript_info = transcript_record.split('|')
-                    try:
-                        consequence = transcript_info[self._consequence_index]
-                    except IndexError:
-                        msg = "Give a valid index for the consequence in the INFO field for: {}".format(transcript_record)
-                        self.get_logger().debug(msg)
-                        continue
-                    consequences.append(consequence)
-                    try:
-                        transcript_id = transcript_info[self._transcript_index]
-                    except IndexError:
-                        msg = "Give a valid index for the Transcript ID in the INFO field for: {}".format(transcript_record)
-                        self.get_logger().debug(msg)
-                        continue
-                    if transcript_id == "":
-                        continue
-
-                    try:
-                        transcript_id_v = transcript_id_mapping[transcript_id]
-                    except KeyError:
-                        transcript_id_v = transcript_id
-
-                    try:
-                        row = transcripts_dict[transcript_id_v]
-                        ref_seq = row.seq  # get the seq and desc for the transcript from the fasta of the gtf
-                        desc = str(row.description)
-                    except KeyError:
-                        msg = "Transcript {} not found in fasta of the GTF file {}".format(transcript_id_v, record)
-                        self.get_logger().debug(msg)
-                        continue
-
-                    feature_types = ['exon']
-                    # check if cds info exists in the fasta header otherwise translate all exons
-                    cds_info = []
-                    num_orfs = 3
-                    if 'CDS=' in desc:
-                        try:
-                            cds_info = [int(x) for x in desc.split(' ')[1].split('=')[1].split('-')]
-                            feature_types = ['CDS', 'stop_codon']
-                            num_orfs = 1
-                        except (ValueError, IndexError):
-                            msg = "Could not extra cds position from fasta header for: {}".format(desc)
-                            self.get_logger().debug(msg)
-                            pass
-                    chrom, strand, features_info, feature_biotype = self.get_features(db, transcript_id_v,
-                                                                                      self._biotype_str,
-                                                                                      feature_types)
-                    if chrom == None: #the record info was not found
-                        continue
-                    # skip transcripts with unwanted consequences
-                    if (consequence in self._exclude_consequences or
-                            (consequence not in self._include_consequences and
-                             self._include_consequences != ['all'])):
-                        continue
-
-                    # only include features that have the specified biotypes or they have CDSs info
-                    if 'CDS' in feature_types and not self._skip_including_all_cds:
-                        pass
-                    elif (feature_biotype in self._exclude_biotypes or
-                          (feature_biotype not in self._include_biotypes and
-                           self._include_biotypes != ['all'])):
-                        continue
-                    for alt in record.ALT:  # in cases of multiple alternative alleles consider all
-                        if alt is None:
-                            continue
-                        if transcript_id + str(record.REF) + str(
-                                alt) in processed_transcript_allele:  # because VEP reports affected transcripts per alt allele
-                            continue
-
-                        processed_transcript_allele.append(transcript_id + str(record.REF) + str(alt))
-                        "for non-CDSs, only consider the exon that actually overlaps the variant"
-
-                        try:
-                            overlap_flag = self.check_overlap(record.POS, record.POS + len(alt), features_info)
-                        except TypeError:
-                            msg = "Wrong VCF record in {}".format(record)
-                            self.get_logger().debug(msg)
-                            continue
-
-                        if (chrom.lstrip("chr") == str(record.CHROM).lstrip("chr") and
-                                overlap_flag):
-                            coding_ref_seq, coding_alt_seq = self.get_altseq(ref_seq, Seq(str(record.REF)),
-                                                                             Seq(str(alt)), int(record.POS), strand,
-                                                                             features_info, cds_info)
-                            if coding_alt_seq != "":
-                                ref_orfs, alt_orfs = self.get_orfs_vcf(coding_ref_seq, coding_alt_seq, trans_table,
-                                                                       num_orfs)
-                                record_id = ""
-                                if record.ID:
-                                    record_id = '_' + str(record.ID)
-                                self.write_output(seq_id='_'.join([self._header_var_prefix + str(record_id),
-                                                                   '.'.join([str(record.CHROM), str(record.POS),
-                                                                             str(record.REF), str(alt)]),
-                                                                   transcript_id_v]),
-                                                  desc=feature_biotype + ":" + consequence,
-                                                  seqs=alt_orfs,
-                                                  prots_fn=prots_fn)
-
-                                if self._report_reference_seq:
-                                    self.write_output(seq_id=transcript_id_v,
-                                                      desc=feature_biotype,
-                                                      seqs=ref_orfs,
-                                                      prots_fn=prots_fn)
-
-        return self._proteindb_output
-
-    def check_proteindb(self, input_fasta : str = None, num_aa: str = 6):
-
-      input_handle = open(input_fasta, 'r')
-      output_handle = open(self._proteindb_output, 'w')
-      proteins = []
-      pcount = 0
-      stop_count = 0
-      gap_count = 0
-      no_met = 0
-      less = 0
-
-      for record in SeqIO.parse(input_handle, 'fasta'):
-
-        seq = str(record.seq)
-        pcount += 1
-
-
-        # parse the description string into a dictionary
-        new_desc_string = record.description
-        new_desc_string = new_desc_string[new_desc_string.find(' ') + 1:]
-        # test for odd amino acids, stop codons, gaps
-        if not seq.startswith('M'):
-          no_met += 1
-        if seq.endswith('*'):
-          seq = seq[:-1]
-        if '*' in seq:
-          stop_count += 1
+    transcripts_dict = SeqIO.index(input_fasta, "fasta", key_function=self.get_key)
+    # handle cases where the transcript has version in the GTF but not in the VCF
+    transcript_id_mapping = {k.split('.')[0]: k for k in transcripts_dict.keys()}
+    with open(self._proteindb_output, 'w') as prots_fn:
+      vcf_reader = vcf.Reader(open(vcf_file, 'r'))
+
+      for record in vcf_reader:
+        if record.ALT == [None] or record.REF == [None]:
+          msg = "Invalid VCF record, skipping: {}".format(record)
+          self.get_logger().debug(msg)
+          continue
+        if not self._ignore_filters:
+          if record.FILTER:  # if not PASS: None and empty means PASS
+            if not (set(record.FILTER[0].split(',')) <= set(self._accepted_filters)):
+              continue
+
+        # only process variants above a given allele frequency threshold if the AF string is not empty
+        if self._af_field:
+          # get AF from the INFO field
+          try:
+            af = float(record.INFO[self._af_field])
+          except TypeError:
+            af = float(record.INFO[self._af_field][0])
+          except KeyError:
+            continue
+
+          # check if the AF passed the threshold
+          if af < self._af_threshold:
+            continue
+
+        trans_table = self._translation_table
+        consequences = []
+        if str(record.CHROM).lstrip('chr').upper() in ['M', 'MT']:
+          trans_table = self._mito_translation_table
+
+        processed_transcript_allele = []
+
+        for transcript_record in record.INFO[self._annotation_field_name]:
+          transcript_info = transcript_record.split('|')
+          try:
+            consequence = transcript_info[self._consequence_index]
+          except IndexError:
+            msg = "Give a valid index for the consequence in the INFO field for: {}".format(transcript_record)
+            self.get_logger().debug(msg)
+            continue
+          consequences.append(consequence)
+          try:
+            transcript_id = transcript_info[self._transcript_index]
+          except IndexError:
+            msg = "Give a valid index for the Transcript ID in the INFO field for: {}".format(transcript_record)
+            self.get_logger().debug(msg)
+            continue
+          if transcript_id == "":
+            continue
+
+          try:
+            transcript_id_v = transcript_id_mapping[transcript_id]
+          except KeyError:
+            transcript_id_v = transcript_id
+
+          try:
+            row = transcripts_dict[transcript_id_v]
+            ref_seq = row.seq  # get the seq and desc for the transcript from the fasta of the gtf
+            desc = str(row.description)
+          except KeyError:
+            msg = "Transcript {} not found in fasta of the GTF file {}".format(transcript_id_v, record)
+            self.get_logger().debug(msg)
+            continue
+
+          feature_types = ['exon']
+          # check if cds info exists in the fasta header otherwise translate all exons
+          cds_info = []
+          num_orfs = 3
+          if 'CDS=' in desc:
+            try:
+              cds_info = [int(x) for x in desc.split(' ')[1].split('=')[1].split('-')]
+              feature_types = ['CDS', 'stop_codon']
+              num_orfs = 1
+            except (ValueError, IndexError):
+              msg = "Could not extra cds position from fasta header for: {}".format(desc)
+              self.get_logger().debug(msg)
+
+          chrom, strand, features_info, feature_biotype = self.get_features(db, transcript_id_v,
+                                                                            self._biotype_str,
+                                                                            feature_types)
+          if chrom is None:  # the record info was not found
+            continue
+          # skip transcripts with unwanted consequences
+          if (consequence in self._exclude_consequences or
+            (consequence not in self._include_consequences and
+             self._include_consequences != ['all'])):
+            continue
+
+          # only include features that have the specified biotypes or they have CDSs info
+          if 'CDS' in feature_types and not self._skip_including_all_cds:
+            pass
+          elif (feature_biotype in self._exclude_biotypes or
+                (feature_biotype not in self._include_biotypes and
+                 self._include_biotypes != ['all'])):
+            continue
+          for alt in record.ALT:  # in cases of multiple alternative alleles consider all
+            if alt is None:
+              continue
+            if transcript_id + str(record.REF) + str(
+              alt) in processed_transcript_allele:  # because VEP reports affected transcripts per alt allele
+              continue
+
+            processed_transcript_allele.append(transcript_id + str(record.REF) + str(alt))
+            # for non-CDSs, only consider the exon that actually overlaps the variant
+
+            try:
+              overlap_flag = self.check_overlap(record.POS, record.POS + len(alt), features_info)
+            except TypeError:
+              msg = "Wrong VCF record in {}".format(record)
+              self.get_logger().debug(msg)
+              continue
+
+            if (chrom.lstrip("chr") == str(record.CHROM).lstrip("chr") and
+              overlap_flag):
+              coding_ref_seq, coding_alt_seq = self.get_altseq(ref_seq, Seq(str(record.REF)),
+                                                               Seq(str(alt)), int(record.POS), strand,
+                                                               features_info, cds_info)
+              if coding_alt_seq != "":
+                ref_orfs, alt_orfs = self.get_orfs_vcf(coding_ref_seq, coding_alt_seq, trans_table,
+                                                       num_orfs)
+                record_id = ""
+                if record.ID:
+                  record_id = '_' + str(record.ID)
+                self.write_output(seq_id='_'.join([self._header_var_prefix + str(record_id),
+                                                   '.'.join([str(record.CHROM), str(record.POS),
+                                                             str(record.REF), str(alt)]),
+                                                   transcript_id_v]),
+                                  desc=feature_biotype + ":" + consequence,
+                                  seqs=alt_orfs,
+                                  prots_fn=prots_fn)
+
+                if self._report_reference_seq:
+                  self.write_output(seq_id=transcript_id_v,
+                                    desc=feature_biotype,
+                                    seqs=ref_orfs,
+                                    prots_fn=prots_fn)
+
+    return self._proteindb_output
+
+  @staticmethod
+  def add_protein_to_map(seq: str, new_desc_string: str, protein_id: str, proteins, output_handle):
+    protein = {'description': new_desc_string, 'sequence': seq, 'accession': protein_id}
+    proteins.append(protein)
+    output_handle.write(">{}\t{}\n{}\n".format(protein_id, new_desc_string, seq))
+    return proteins
+
+  def check_proteindb(self, input_fasta: str = None, add_stop_codon: bool = False, num_aa: int = 6):
+
+    input_handle = open(input_fasta, 'r')
+    output_handle = open(self._proteindb_output, 'w')
+    proteins = []
+    pcount = 0
+    stop_count = 0
+    gap_count = 0
+    no_met = 0
+    less = 0
+
+    for record in SeqIO.parse(input_handle, 'fasta'):
+
+      seq = str(record.seq)
+      pcount += 1
+
+      # parse the description string into a dictionary
+      new_desc_string = record.description
+      new_desc_string = new_desc_string[new_desc_string.find(' ') + 1:]
+      # test for odd amino acids, stop codons, gaps
+      if not seq.startswith('M'):
+        no_met += 1
+      if seq.endswith('*'):
+        seq = seq[:-1]
+      if '-' in seq:
+        gap_count += 1
+        new_desc_string = new_desc_string + ' (Contains gaps)'
+      if '*' in seq:
+        stop_count += 1
+        if add_stop_codon:
+          seq_list = seq.split("*")
+          codon_index = 1
+          for codon in seq_list:
+            new_desc_string = new_desc_string + ' codon ' + str(codon_index)
+            protein_id = record.id + '_codon_' + str(codon_index)
+            seq = codon
+            if len(seq) > num_aa:
+              proteins = self.add_protein_to_map(seq, new_desc_string, protein_id, proteins, output_handle)
+            codon_index = codon_index + 1
+        else:
           cut = seq.index('*')
           string = ' (Premature stop %s/%s)' % (cut, len(seq))
           new_desc_string = new_desc_string + string
           seq = seq[:cut]
-        if '-' in seq:
-          gap_count += 1
-          new_desc_string = new_desc_string + ' (Contains gaps)'
-
-        # save the protein in list
-
+          # save the protein in list
+          if len(seq) > num_aa:
+            protein_id = record.id
+            proteins = self.add_protein_to_map(seq, new_desc_string, protein_id, proteins, output_handle)
+          else:
+            less += 1
+      else:
         if len(seq) > num_aa:
-          protein = {}
-          protein['description'] = new_desc_string
-          protein['sequence'] = seq
-          protein['accession'] = record.id
-          proteins.append(protein)
-
-          output_handle.write(">{}\t{}\n{}\n".format(record.id, new_desc_string, seq))
+          protein_id = record.id
+          proteins = self.add_protein_to_map(seq, new_desc_string, protein_id, proteins, output_handle)
         else:
           less += 1
 
-      print("   translations that do not start with Met:", no_met)
-      print("   translations that have premature stop codons:", stop_count)
-      print("   translations that contain gaps:", gap_count)
-      print("   total number of input sequences was:", pcount)
-      print("   total number of sequences written was:", len(proteins))
-      print("   total number of proteins less than {} aminoacids: {}".format(num_aa, less))
-
-
-    def write_output(self, seq_id, desc, seqs, prots_fn):
-        """write the orfs to the output file"""
-        write_i = False
-        if len(seqs) > 1:  # only add _num when multiple ORFs are generated (e.g in 3 ORF)
-            write_i = True
-
-        for i, orf in enumerate(seqs):
-            if write_i:  # only add _num when multiple ORFs are generated (e.g in 3 ORF)
-                prots_fn.write('>{} {}\n{}\n'.format(seq_id + "_" + str(i + 1), desc, orf))
-            else:
-                prots_fn.write('>{} {}\n{}\n'.format(seq_id, desc, orf))
+    print("   translations that do not start with Met:", no_met)
+    print("   translations that have premature stop codons:", stop_count)
+    print("   translations that contain gaps:", gap_count)
+    print("   total number of input sequences was:", pcount)
+    print("   total number of sequences written was:", len(proteins))
+    print("   total number of proteins less than {} aminoacids: {}".format(num_aa, less))
+
+  @staticmethod
+  def write_output(seq_id, desc, seqs, prots_fn):
+    """
+    write the orfs to the output file
+    :param seq_id: Sequence Accession
+    :param desc: Sequence Description
+    :param seqs: Sequence
+    :param prots_fn:
+    :return:
+    """
+    write_i = False
+    if len(seqs) > 1:  # only add _num when multiple ORFs are generated (e.g in 3 ORF)
+      write_i = True
+
+    for i, orf in enumerate(seqs):
+      if write_i:  # only add _num when multiple ORFs are generated (e.g in 3 ORF)
+        prots_fn.write('>{} {}\n{}\n'.format(seq_id + "_" + str(i + 1), desc, orf))
+      else:
+        prots_fn.write('>{} {}\n{}\n'.format(seq_id, desc, orf))
 
 
 if __name__ == '__main__':
-    print("ERROR: This script is part of a pipeline collection and it is not meant to be run in stand alone mode")
+  print("ERROR: This script is part of a pipeline collection and it is not meant to be run in stand alone mode")
```

### Comparing `pypgatk-0.0.8/pypgatk/ensembl/models.py` & `pypgatk-0.0.9/pypgatk/ensembl/models.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk/proteomics/db/decoy_pyrat.py` & `pypgatk-0.0.9/pypgatk/proteomics/db/decoy_pyrat.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,28 +203,28 @@
         outfa = open(self._temp_file, 'w')
 
         # Open FASTA file using first cmd line argument
         fasta = SeqIO.parse(self._input_fasta, 'fasta')
         # loop each seq in the file
         for record in fasta:
                 seq = str(record.seq)
-                dcount+=1	
+                dcount+=1
                 #make sequence isobaric (check args for switch off)
-                if self._isobaric == False:
+                if not self._isobaric:
                         seq = seq.replace('I', 'L')
 
                 #digest sequence add peptides to set
                 upeps.update(ProteinDBService.digest(seq, self._cleavage_sites, self._cleavage_position,
                                                          self._anti_cleavage_sites, self._peptide_length))
 
                 #reverse and switch protein sequence
                 decoyseq = ProteinDBService.revswitch(seq, self._no_switch, self._cleavage_sites)
 
                 #do not store decoy peptide set in reduced memory mode
-                if self._memory_save == False:
+                if not self._memory_save:
                         #update decoy peptide set
                         dpeps.update( ProteinDBService.digest(decoyseq, self._cleavage_sites, self._cleavage_position,
                                                              self._anti_cleavage_sites, self._peptide_length))
 
                 #write decoy protein accession and sequence to file
                 outfa.write('>' + self._decoy_prefix + record.id + '\n')
                 outfa.write(decoyseq + '\n')
```

### Comparing `pypgatk-0.0.8/pypgatk/pypgatk_cli.py` & `pypgatk-0.0.9/pypgatk/pypgatk_cli.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk/tests/pypgatk_tests.py` & `pypgatk-0.0.9/pypgatk/tests/pypgatk_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,32 +184,56 @@
         """
     runner = CliRunner()
     result = runner.invoke(cli,
                            ['ensembl-downloader', '--config_file', 'config/ensembl_downloader_config.yaml',
                             '--taxonomy', '9103', '--output_directory', 'testdata'])
     assert result.exit_code == 0
 
+
+def download_ensembl_data_37():
+  """
+      Test downloading ensembl data for species with taxonomy identifier = 9606
+      :return:
+      """
+  runner = CliRunner()
+  result = runner.invoke(cli,
+                         ['ensembl-downloader', '--config_file', 'config/ensembl_downloader_config.yaml',
+                          '--taxonomy', '9606', '--output_directory', 'testdata', '--grch37'])
+  assert result.exit_code == 0
+
 def download_cbioportal_data():
     """
         Test downloading cbioportal data for study id: paac_jhu_2014
         :return:
         """
     runner = CliRunner()
     result = runner.invoke(cli,
                            ['cbioportal-downloader', '--config_file', 'config/cbioportal_config.yaml',
                             '--download_study', 'paac_jhu_2014', '--output_directory', 'testdata'])
     assert result.exit_code == 0
 
+
+def check_ensembl_database():
+  runner = CliRunner()
+  result = runner.invoke(cli,
+                         ['ensembl-check', '--config_file', 'config/ensembl_config.yaml',
+                          '--input_fasta', 'testdata/proteindb_from_ENSEMBL_VCF.fa', '--output', 'testdata/proteindb_from_ENSEMBL_VCF-clean.fa', '--add_stop_codons', '--num_aa', '6'])
+  assert result.exit_code == 0
+
+
+
 if __name__ == '__main__':
     vcf_to_proteindb()
     vcf_gnomad_to_proteindb()
     dnaseq_to_proteindb()
     dnaseq_ncrnas_to_proteindb()
     dnaseq_lncrnas_to_proteindb()
     dnaseq_sncrnas_to_proteindb()
     dnaseq_pseudogenes_to_proteindb()
     dnaseq_altorfs_to_proteindb()
     cbioportal_to_proteindb()
     generate_decoy_database()
     cosmic_to_proteindb()
     download_ensembl_data()
+    download_ensembl_data_37()
     download_cbioportal_data()
+    check_ensembl_database()
```

### Comparing `pypgatk-0.0.8/pypgatk/toolbox/exceptions.py` & `pypgatk-0.0.9/pypgatk/toolbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk/toolbox/general.py` & `pypgatk-0.0.9/pypgatk/toolbox/general.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk/toolbox/rest.py` & `pypgatk-0.0.9/pypgatk/toolbox/rest.py`

 * *Files identical despite different names*

### Comparing `pypgatk-0.0.8/pypgatk.egg-info/PKG-INFO` & `pypgatk-0.0.9/pypgatk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pypgatk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python tools for proteogenomics
 Home-page: http://github.com/bigbio/py-pgatk
 Author: PgAtk Team
 Author-email: ypriverol@gmail.com
 License: LICENSE.txt
 Description: # Python tools for ProteoGenomics Analysis Toolkit
         
         
         ![Python application](https://github.com/bigbio/py-pgatk/workflows/Python%20application/badge.svg)
         [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pypgatk/README.html)
-        
+        [![Codacy Badge](https://app.codacy.com/project/badge/Grade/f6d030fd7d69413987f7265a01193324)](https://www.codacy.com/gh/bigbio/py-pgatk/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bigbio/py-pgatk&amp;utm_campaign=Badge_Grade)
+        [![PyPI version](https://badge.fury.io/py/pypgatk.svg)](https://badge.fury.io/py/pypgatk)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dm/pypgatk)
         
         **pypgatk** is a Python library part of the [ProteoGenomics Analysis Toolkit](https://pgatk.readthedocs.io/en/latest). It provides different bioinformatics tools for proteogenomics data analysis.
         
         # Requirements:
         
         This package requirements vary depending on the way that you want to install it (all three are independent, you don't need all these requirements):
         
@@ -103,11 +105,13 @@
           vcf-to-proteindb         Generate peptides based on DNA variants from
                                    ENSEMBL VEP VCF files
         
         ```
         
         The library provides multiple commands to download, translate and generate protein sequence databases from reference and mutation genome databases.
         
-        ### Please read full docs here: <https://pgatk.readthedocs.io/en/latest/pypgatk.html>
+        # Full Documentation
+        
+        [https://pgatk.readthedocs.io/en/latest/pypgatk.html](https://pgatk.readthedocs.io/en/latest/pypgatk.html)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pypgatk-0.0.8/pypgatk.egg-info/SOURCES.txt` & `pypgatk-0.0.9/pypgatk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,12 +35,13 @@
 pypgatk/ensembl/ensembl.py
 pypgatk/ensembl/exceptions.py
 pypgatk/ensembl/models.py
 pypgatk/proteomics/__init__.py
 pypgatk/proteomics/db/__init__.py
 pypgatk/proteomics/db/decoy_pyrat.py
 pypgatk/tests/__init__.py
+pypgatk/tests/ensembl_tests.py
 pypgatk/tests/pypgatk_tests.py
 pypgatk/toolbox/__init__.py
 pypgatk/toolbox/exceptions.py
 pypgatk/toolbox/general.py
 pypgatk/toolbox/rest.py
```

### Comparing `pypgatk-0.0.8/setup.py` & `pypgatk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='pypgatk',
-      version='0.0.8',
+      version='0.0.9',
       description='Python tools for proteogenomics',
       url='http://github.com/bigbio/py-pgatk',
       long_description=readme(),
       long_description_content_type='text/markdown',
       author='PgAtk Team',
       author_email='ypriverol@gmail.com',
       license='LICENSE.txt',
```

