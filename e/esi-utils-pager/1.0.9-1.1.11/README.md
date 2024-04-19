# Comparing `tmp/esi-utils-pager-1.0.9.tar.gz` & `tmp/esi_utils_pager-1.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi-utils-pager-1.0.9.tar", last modified: Fri Feb  9 19:42:00 2024, max compression
+gzip compressed data, was "esi_utils_pager-1.1.11.tar", last modified: Fri Apr 19 22:27:41 2024, max compression
```

## Comparing `esi-utils-pager-1.0.9.tar` & `esi_utils_pager-1.1.11.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.944348 esi-utils-pager-1.0.9/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/LICENSE.md
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7121 2024-02-09 19:42:00.940348 esi-utils-pager-1.0.9/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3982 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-02-09 19:42:00.944348 esi-utils-pager-1.0.9/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.916347 esi-utils-pager-1.0.9/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.924347 esi-utils-pager-1.0.9/src/esi_utils_pager/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:40:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.928347 esi-utils-pager-1.0.9/src/esi_utils_pager/bin/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4454 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/bin/pagerlite.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7859 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/calc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/country.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.940348 esi-utils-pager-1.0.9/src/esi_utils_pager/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/countries.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/econexposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    22938 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/emploss.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/exposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/growth.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/pandas_container.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2468 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-02-09 18:25:33.000000 esi-utils-pager-1.0.9/src/esi_utils_pager/semimodel.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-09 19:42:00.940348 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7121 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1363 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-02-09 19:42:00.000000 esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.103234 esi_utils_pager-1.1.11/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/LICENSE.md
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7837 2024-04-19 22:27:41.103234 esi_utils_pager-1.1.11/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4697 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-19 22:27:41.103234 esi_utils_pager-1.1.11/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.087235 esi_utils_pager-1.1.11/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.091235 esi_utils_pager-1.1.11/src/esi_utils_pager/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:26:33.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.091235 esi_utils_pager-1.1.11/src/esi_utils_pager/bin/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5872 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/bin/pagerlite.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8250 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/calc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/country.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.099234 esi_utils_pager-1.1.11/src/esi_utils_pager/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/countries.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/economic.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/econexposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/emploss.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/exposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/growth.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/pandas_container.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/semimodel.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.099234 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7837 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/top_level.txt
```

### Comparing `esi-utils-pager-1.0.9/LICENSE.md` & `esi_utils_pager-1.1.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/PKG-INFO` & `esi_utils_pager-1.1.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.0.9
+Version: 1.1.11
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -164,14 +164,34 @@
 There are three input modes for pagerlite:
 
  - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
  - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
  - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
     (these files can be in sub-directories).
 
+## Examples
+
+To run the PAGER empirical models *only* on a ShakeMap grid.xml file in the current directory and write the results to an Excel file:
+
+`pagerlite -g grid.xml -o output.xlsx`
+
+To run the PAGER empirical models *only* on a directory containing (potentially) many sub-directories with 
+files ending in "grid.xml":
+
+`pagerlite -f /data/shakemap_output/ -o output.xlsx`
+
+To run the PAGER empirical models *only* on a ComCat event ID (this will download the authoritative 
+ShakeMap grid.xml file from ComCat):
+
+`pagerlite -e us7000lz23 -o output.xlsx`
+
+To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
+
+`pagerlite -e us7000lz23 -s -o output.xlsx`
+
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi-utils-pager-1.0.9/README.md` & `esi_utils_pager-1.1.11/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -80,14 +80,34 @@
 There are three input modes for pagerlite:
 
  - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
  - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
  - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
     (these files can be in sub-directories).
 
+## Examples
+
+To run the PAGER empirical models *only* on a ShakeMap grid.xml file in the current directory and write the results to an Excel file:
+
+`pagerlite -g grid.xml -o output.xlsx`
+
+To run the PAGER empirical models *only* on a directory containing (potentially) many sub-directories with 
+files ending in "grid.xml":
+
+`pagerlite -f /data/shakemap_output/ -o output.xlsx`
+
+To run the PAGER empirical models *only* on a ComCat event ID (this will download the authoritative 
+ShakeMap grid.xml file from ComCat):
+
+`pagerlite -e us7000lz23 -o output.xlsx`
+
+To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
+
+`pagerlite -e us7000lz23 -s -o output.xlsx`
+
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi-utils-pager-1.0.9/pyproject.toml` & `esi_utils_pager-1.1.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/calc.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/calc.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,28 +73,35 @@
             continue
         maxmmi_col = mmi_idx[mmi_idx].index[-1]
         maxmmi_array.append(headers.index(maxmmi_col) + 1)
     expframe["MaxMMI1000"] = maxmmi_array
     return (expframe, exposure)
 
 
-def get_fatalities(expframe, exposure):
-    fatmodel = EmpiricalLoss.fromDefaultFatality()
+def get_fatalities(expframe, exposure, fatality_file):
+    if fatality_file is None:
+        fatmodel = EmpiricalLoss.fromDefaultFatality()
+    else:
+        fatmodel = EmpiricalLoss.fromExcel(fatality_file)
+
     fatdict = fatmodel.getLosses(exposure)
     fatdict["Total"] = fatdict.pop("TotalFatalities")
     fatframe = expframe.copy()
     fatframe["Fatalities"] = 0
     for key, value in fatdict.items():
         fatframe.loc[fatframe["CountryCode"] == key, "Fatalities"] = value
     return fatframe
 
 
-def get_econ_losses(fatframe, popfile, popyear, isofile, gridfile):
+def get_econ_losses(fatframe, popfile, popyear, isofile, gridfile, economic_file):
+    if economic_file is None:
+        ecomodel = EmpiricalLoss.fromDefaultEconomic()
+    else:
+        ecomodel = EmpiricalLoss.fromExcel(economic_file)
     econexpmodel = EconExposure(popfile, popyear, isofile)
-    ecomodel = EmpiricalLoss.fromDefaultEconomic()
     econexposure = econexpmodel.calcExposure(gridfile)
     rows = []
     for key, value in econexposure.items():
         if key != "TotalEconomicExposure" and len(key) != 2:
             continue
         row = {}
         ccode = key
@@ -130,15 +137,15 @@
     #         1) Total number of fatalities
     #         2) Dictionary of residential fatalities per building type, per country.
     #         3) Dictionary of non-residential fatalities per building type, per country.
     semifat, resfat, nonresfat = semimodel.getLosses(gridfile)
     return (semifat, resfat, nonresfat)
 
 
-def calc_pager_event(gridfile, config, run_semi):
+def calc_pager_event(gridfile, config, run_semi, fatality_file, economic_file):
     # get all the basic event information and print it, if requested
     shake_tuple = getHeaderData(gridfile)
     local_time = get_local_time(
         shake_tuple[1]["event_timestamp"],
         config["model_data"]["timezones_file"],
         shake_tuple[1]["lat"],
         shake_tuple[1]["lon"],
@@ -158,16 +165,18 @@
     with rasterio.open(isofile, "r") as dataset:
         xy = [(shake_tuple[1]["lon"], shake_tuple[1]["lat"])]
         isocode = list(sample_gen(dataset, xy))[0][0]
         ccode = country.getCountry(isocode)["ISO2"]
     master_row["EpicentralCountryCode"] = ccode
     pop_year, popfile = get_pop_year(config, event_year)
     expframe, exposure = get_exposure(master_row, isofile, popfile, pop_year, gridfile)
-    fatframe = get_fatalities(expframe, exposure)
-    ecoframe = get_econ_losses(fatframe, popfile, pop_year, isofile, gridfile)
+    fatframe = get_fatalities(expframe, exposure, fatality_file)
+    ecoframe = get_econ_losses(
+        fatframe, popfile, pop_year, isofile, gridfile, economic_file
+    )
 
     if run_semi:
         urbanfile = config["model_data"]["urban_rural_grid"]
         semifat, resfat, nonresfat = get_semi_losses(
             gridfile, popfile, pop_year, isofile, urbanfile
         )
         resframe = pd.DataFrame(resfat).transpose()
@@ -181,29 +190,31 @@
             btotal = final_frame.sum(axis="columns")
             final_frame["TotalSemiFatalities"] = btotal
             ecoframe = ecoframe.join(final_frame, on=["CountryCode"])
 
     return ecoframe
 
 
-def calc_pager_events(gridfolder, verbose, run_semi):
+def calc_pager_events(gridfolder, verbose, run_semi, fatality_file, economic_file):
     gridfolder = pathlib.Path(gridfolder)
     # read config file
     config = read_config()
     # Make sure grid.xml file exists
     if not gridfolder.is_dir():
         print(f"ShakeMap Grid folder {gridfolder} does not exist.")
         sys.exit(1)
 
     gridfiles = gridfolder.glob("**/*grid.xml")
     dataframes = []
     for gridfile in gridfiles:
         if verbose:
             logging.info(f"Parsing {gridfile}...")
-        dataframe = calc_pager_event(gridfile, config, run_semi)
+        dataframe = calc_pager_event(
+            gridfile, config, run_semi, fatality_file, economic_file
+        )
         dataframes.append(dataframe)
 
     dataframe = pd.concat(dataframes)
     if run_semi:
         # make TotalSemiFatalities column the last one, if it exists
         fatcol = dataframe.pop("TotalSemiFatalities")
         ncols = len(dataframe.columns)
```

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/config.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/config.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/country.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/country.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/countries.xlsx` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/countries.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/economy.xml` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/economy.xml`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/fatality.xml` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.hdf` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_casualty.xlsx` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.hdf` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_collapse_mmi.xlsx` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.hdf` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_inventory.xlsx` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.hdf` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.hdf`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/data/semi_workforce.xlsx` & `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.xlsx`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/econexposure.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/econexposure.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/emploss.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/emploss.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # stdlib imports
 import pathlib
 from collections import OrderedDict
 from xml.dom import minidom
 
 # third party imports
 import numpy as np
+import pandas as pd
 import shapely
 from mapio.grid2d import Grid2D
 from scipy.special import erfc
 
 # local imports
 from esi_utils_pager.country import Country
 from esi_utils_pager.probs import calcEmpiricalProbFromRange
@@ -321,22 +322,22 @@
             return self._model_dict[ccode]
         else:
             return default
 
     @classmethod
     def fromDefaultFatality(cls):
         homedir = pathlib.Path(__file__).parent  # where is this module?
-        fatxml = homedir / "data" / "fatality.xml"
-        return cls.fromXML(fatxml)
+        fatexcel = homedir / "data" / "fatality.xlsx"
+        return cls.fromExcel(fatexcel)
 
     @classmethod
     def fromDefaultEconomic(cls):
         homedir = pathlib.Path(__file__).parent  # where is this module?
-        econxml = homedir / "data" / "economy.xml"
-        return cls.fromXML(econxml)
+        econexcel = homedir / "data" / "economic.xlsx"
+        return cls.fromExcel(econexcel)
 
     @classmethod
     def fromXML(cls, xmlfile):
         """Load country-specific models from an XML file of the form:
           <?xml version="1.0" encoding="US-ASCII" standalone="yes"?>
 
           <models vstr="2.2" type="fatality">
@@ -375,14 +376,50 @@
             else:
                 alpha = 1.0  # what is the appropriate default value for this?
             model_list.append(LognormalModel(key, theta, beta, l2g, alpha=alpha))
         root.unlink()
 
         return cls(model_list, losstype)
 
+    @classmethod
+    def fromExcel(cls, excelfile):
+        """Load country-specific models from an Excel file containing columns:
+          (for fatality model)
+          - ccode Two letter ISO country code
+          - theta Lognormal theta parameter
+          - beta Lognormal beta parameter
+          - gnormvalue The G norm value used to determine model uncertainties.
+          (for economic model)
+          - ccode Two letter ISO country code
+          - alpha Lognormal theta parameter
+          - beta Lognormal beta parameter
+          - gnormvalue The G norm value used to determine model uncertainties.
+
+        :param xmlfile:
+          XML file containing model parameters (see above).
+        :returns:
+          EmpiricalLoss instance.
+        """
+        dataframe = pd.read_excel(excelfile)
+        losstype = "fatality"
+        if "alpha" in dataframe.columns:
+            losstype = "economic"
+        model_list = []
+        for idx, row in dataframe.iterrows():
+            key = row["ccode"]
+            theta = row["theta"]
+            beta = row["beta"]
+            l2g = row["gnormvalue"]
+            if losstype == "economic":
+                alpha = row["alpha"]
+            else:
+                alpha = 1.0
+            model_list.append(LognormalModel(key, theta, beta, l2g, alpha=alpha))
+        return cls(model_list, losstype)
+
     def getLossRates(self, ccode, mmirange):
         """Return loss rates for given country country code model at input MMI values.
 
         :param ccode:
           Country code (usually two letter ISO code).
         :param mmirange:
           Array-like range of MMI values at which loss rates will be calculated.
```

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/exposure.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/exposure.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/growth.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/growth.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/probs.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/probs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import numpy as np
 import math
+
+import numpy as np
 from scipy.special import erfc, erfcinv
 
 
 def phi(input):
     """Phi function.
 
     :param input:
@@ -70,15 +71,15 @@
     :param drange:
       Two-element sequence, containing range of losses over which probability should be calculated.
     :returns:
       Probability that losses will occur in input range.
     """
     e = e + 0.00001
     if e < 1:
-        # e = 0.1
+        e = 0.1
         if G > 1.7:
             G = 1.7613
     if len(drange) == 2:
         if (e - 0) < 0.001:
             e = 0.5
         fmin = drange[0] + 0.00001
         fmax = drange[1] + 0.00001
```

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager/semimodel.py` & `esi_utils_pager-1.1.11/src/esi_utils_pager/semimodel.py`

 * *Files identical despite different names*

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/PKG-INFO` & `esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.0.9
+Version: 1.1.11
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -164,14 +164,34 @@
 There are three input modes for pagerlite:
 
  - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
  - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
  - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
     (these files can be in sub-directories).
 
+## Examples
+
+To run the PAGER empirical models *only* on a ShakeMap grid.xml file in the current directory and write the results to an Excel file:
+
+`pagerlite -g grid.xml -o output.xlsx`
+
+To run the PAGER empirical models *only* on a directory containing (potentially) many sub-directories with 
+files ending in "grid.xml":
+
+`pagerlite -f /data/shakemap_output/ -o output.xlsx`
+
+To run the PAGER empirical models *only* on a ComCat event ID (this will download the authoritative 
+ShakeMap grid.xml file from ComCat):
+
+`pagerlite -e us7000lz23 -o output.xlsx`
+
+To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
+
+`pagerlite -e us7000lz23 -s -o output.xlsx`
+
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi-utils-pager-1.0.9/src/esi_utils_pager.egg-info/SOURCES.txt` & `esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 src/esi_utils_pager.egg-info/requires.txt
 src/esi_utils_pager.egg-info/top_level.txt
 src/esi_utils_pager/bin/pagerlite.py
 src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
 src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
 src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
 src/esi_utils_pager/data/countries.xlsx
+src/esi_utils_pager/data/economic.xlsx
 src/esi_utils_pager/data/economy.xml
+src/esi_utils_pager/data/fatality.xlsx
 src/esi_utils_pager/data/fatality.xml
 src/esi_utils_pager/data/semi_casualty.hdf
 src/esi_utils_pager/data/semi_casualty.xlsx
 src/esi_utils_pager/data/semi_collapse_mmi.hdf
 src/esi_utils_pager/data/semi_collapse_mmi.xlsx
 src/esi_utils_pager/data/semi_inventory.hdf
 src/esi_utils_pager/data/semi_inventory.xlsx
```

