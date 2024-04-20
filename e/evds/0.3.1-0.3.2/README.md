# Comparing `tmp/evds-0.3.1.tar.gz` & `tmp/evds-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evds-0.3.1.tar", last modified: Sun Jul  9 14:00:50 2023, max compression
+gzip compressed data, was "evds-0.3.2.tar", last modified: Sat Apr 20 07:14:38 2024, max compression
```

## Comparing `evds-0.3.1.tar` & `evds-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 14:00:50.711154 evds-0.3.1/
--rw-r--r--   0 ege       (1000) ege       (1000)     1071 2023-07-09 13:53:18.000000 evds-0.3.1/LICENCE
--rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 14:00:50.711154 evds-0.3.1/PKG-INFO
--rw-r--r--   0 ege       (1000) ege       (1000)    10356 2023-07-09 13:53:18.000000 evds-0.3.1/README.md
-drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 14:00:50.711154 evds-0.3.1/evds/
--rw-r--r--   0 ege       (1000) ege       (1000)    10194 2023-07-09 13:59:50.000000 evds-0.3.1/evds/__init__.py
-drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 14:00:50.711154 evds-0.3.1/evds.egg-info/
--rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/PKG-INFO
--rw-r--r--   0 ege       (1000) ege       (1000)      182 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/SOURCES.txt
--rw-r--r--   0 ege       (1000) ege       (1000)        1 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/dependency_links.txt
--rw-r--r--   0 ege       (1000) ege       (1000)       24 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/requires.txt
--rw-r--r--   0 ege       (1000) ege       (1000)        5 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/top_level.txt
--rw-r--r--   0 ege       (1000) ege       (1000)       38 2023-07-09 14:00:50.711154 evds-0.3.1/setup.cfg
--rw-r--r--   0 ege       (1000) ege       (1000)      709 2023-07-09 13:59:50.000000 evds-0.3.1/setup.py
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2024-04-20 07:14:38.645390 evds-0.3.2/
+-rw-r--r--   0 ege       (1000) ege       (1000)     1071 2024-04-20 07:07:19.000000 evds-0.3.2/LICENCE
+-rw-r--r--   0 ege       (1000) ege       (1000)    10831 2024-04-20 07:14:38.645390 evds-0.3.2/PKG-INFO
+-rw-r--r--   0 ege       (1000) ege       (1000)    10356 2024-04-20 07:07:19.000000 evds-0.3.2/README.md
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2024-04-20 07:14:38.645390 evds-0.3.2/evds/
+-rw-r--r--   0 ege       (1000) ege       (1000)    10028 2024-04-20 07:07:19.000000 evds-0.3.2/evds/__init__.py
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2024-04-20 07:14:38.645390 evds-0.3.2/evds.egg-info/
+-rw-r--r--   0 ege       (1000) ege       (1000)    10831 2024-04-20 07:14:38.000000 evds-0.3.2/evds.egg-info/PKG-INFO
+-rw-r--r--   0 ege       (1000) ege       (1000)      182 2024-04-20 07:14:38.000000 evds-0.3.2/evds.egg-info/SOURCES.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)        1 2024-04-20 07:14:38.000000 evds-0.3.2/evds.egg-info/dependency_links.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)       24 2024-04-20 07:14:38.000000 evds-0.3.2/evds.egg-info/requires.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)        5 2024-04-20 07:14:38.000000 evds-0.3.2/evds.egg-info/top_level.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)       38 2024-04-20 07:14:38.645390 evds-0.3.2/setup.cfg
+-rw-r--r--   0 ege       (1000) ege       (1000)      709 2024-04-20 07:10:29.000000 evds-0.3.2/setup.py
```

### Comparing `evds-0.3.1/LICENCE` & `evds-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `evds-0.3.1/PKG-INFO` & `evds-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: evds
-Version: 0.3.1
+Version: 0.3.2
 Summary: EVDS python wrapper
 Home-page: https://github.com/fatihmete/evds
 Author: Fatih Mete
 Author-email: fatihmete@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 # EVDS
 
 [English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
 
 EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
```

### Comparing `evds-0.3.1/README.md` & `evds-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `evds-0.3.1/evds/__init__.py` & `evds-0.3.2/evds/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             self.session.verify = self.httpsVerify
 
     def __get_main_categories(self):
         """
         Function returns main categories dataframe.
         """
         main_categories = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/categories/',
-                                              params={'key': self.key, 'type': 'json'})
+                                              params={'type': 'json'})
         try:
             main_categories_raw = json.loads(main_categories)
             main_categories_df = pd.DataFrame(main_categories_raw)[
                 ["CATEGORY_ID", "TOPIC_TITLE_" + self.lang]]
             main_categories_df["CATEGORY_ID"] = main_categories_df["CATEGORY_ID"].astype(
                 "int")
             return main_categories_df[~main_categories_df.CATEGORY_ID.isin(self.not_available_categories)]
@@ -78,28 +78,26 @@
         If main_category,
             - Not defined, returns all subcategories,
             - Defined as an integer, returns subcategories which main category id match this value,
             - Defined as a string, depending on self.lang value, search in main category name and 
               returns matched the main category' subcategories
         """
         if main_category == "":
-            params = {'key': self.key, 'mode': 0, 'code': '', 'type': 'json'}
+            params = {'mode': 0, 'code': '', 'type': 'json'}
 
         elif isinstance(main_category, (int, float)):
             if main_category in self.main_categories["CATEGORY_ID"].to_list():
-                params = {'key': self.key, 'mode': 2,
-                          'code': main_category, 'type': 'json'}
+                params = {'mode': 2, 'code': main_category, 'type': 'json'}
             else:
                 raise CategoryNotFoundError("Category not found.")
         else:
             try:
                 code = self.main_categories[self.main_categories["TOPIC_TITLE_" +
                                                                  self.lang].str.contains(main_category)]["CATEGORY_ID"].values[0]
-                params = {'key': self.key, 'mode': 2,
-                          'code': code, 'type': 'json'}
+                params = {'mode': 2, 'code': code, 'type': 'json'}
             except:
                 raise CategoryNotFoundError("Category not found.")
 
         sub_categories = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/datagroups/',
                                              params=params)
         sub_categories = json.loads(sub_categories)
         if raw:
@@ -114,15 +112,15 @@
 
     def get_series(self, datagroup_code, detail=False, raw=False):
         """
         The function returns dataframe of series which belongs to given data group.
         Because of default detail parameter is False, only return "SERIE_CODE", "SERIE_NAME" and "START_DATE" value.
         """
         series = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/serieList/',
-                                     params={'key': self.key, 'type': 'json', 'code': datagroup_code})
+                                     params={'type': 'json', 'code': datagroup_code})
         series = json.loads(series)
         if raw:
             return series
         df = pd.DataFrame(series)
         if detail == False:
             return df[["SERIE_CODE",
                        "SERIE_NAME" + ("_ENG" if self.lang == "ENG" else ""),
@@ -195,15 +193,14 @@
 
         data = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/',
                                    params={
                                        'series': "-".join(series),
                                        'startDate': startdate,
                                        'endDate': enddate,
                                        'type': 'json',
-                                       'key': self.key,
                                        'formulas': formula_param,
                                        'frequency': str(frequency),
                                        'aggregationTypes': aggregation_type_param,
                                    })
         data = json.loads(data)["items"]
         # If raw is true return only json results.
         if raw:
@@ -218,15 +215,15 @@
 
         if "UNIXTIME" in df.columns:
             df.drop(columns=["UNIXTIME"], inplace=True)
         return df
 
     def __make_request(self, url, params={}):
         params = self.__param_generator(params)
-        request = self.session.get(url + params)
+        request = self.session.get(url + params, headers={'key': self.key})
         self.session.close()
         print(request.url) if self.DEBUG == True else None
         if request.status_code == 200:
             return request.content
         else:
             raise EVDSConnectionError(
                 "Connection error, please check your API Key or request. Url:{}".format(request.url))
```

### Comparing `evds-0.3.1/evds.egg-info/PKG-INFO` & `evds-0.3.2/evds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: evds
-Version: 0.3.1
+Version: 0.3.2
 Summary: EVDS python wrapper
 Home-page: https://github.com/fatihmete/evds
 Author: Fatih Mete
 Author-email: fatihmete@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 # EVDS
 
 [English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
 
 EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
```

### Comparing `evds-0.3.1/setup.py` & `evds-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="evds",
-    version="0.3.1",
+    version="0.3.2",
     author="Fatih Mete",
     author_email="fatihmete@live.com",
     description="EVDS python wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fatihmete/evds",
     packages=setuptools.find_packages(),
```

