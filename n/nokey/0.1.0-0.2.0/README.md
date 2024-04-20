# Comparing `tmp/nokey-0.1.0.tar.gz` & `tmp/nokey-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.1.0.tar", last modified: Sun Apr 14 00:33:39 2024, max compression
+gzip compressed data, was "nokey-0.2.0.tar", last modified: Sat Apr 20 15:25:31 2024, max compression
```

## Comparing `nokey-0.1.0.tar` & `nokey-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,76 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.425000 nokey-0.1.0/
--rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2962 2024-04-14 00:33:39.421000 nokey-0.1.0/PKG-INFO
--rw-------   0 root         (0) root         (0)     2441 2024-04-14 00:25:34.000000 nokey-0.1.0/README.md
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.221000 nokey-0.1.0/nokey/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/__init__.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.245000 nokey-0.1.0/nokey/animals/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/animals/__init__.py
--rw-------   0 root         (0) root         (0)     2615 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/animals/dog_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.257000 nokey-0.1.0/nokey/country_info/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/country_info/__init__.py
--rw-------   0 root         (0) root         (0)     4631 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/country_info/rest_country.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.265000 nokey-0.1.0/nokey/developer_tools/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/developer_tools/__init__.py
--rw-------   0 root         (0) root         (0)     1489 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/developer_tools/url_shortener.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.273000 nokey-0.1.0/nokey/education/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/education/__init__.py
--rw-------   0 root         (0) root         (0)     2215 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/education/university_names_and_domains.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.285000 nokey-0.1.0/nokey/finance/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/finance/__init__.py
--rw-------   0 root         (0) root         (0)      977 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/finance/wall_street_bets.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.293000 nokey-0.1.0/nokey/food/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/food/__init__.py
--rw-------   0 root         (0) root         (0)     3044 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/food/fruityvice.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.305000 nokey-0.1.0/nokey/games/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/games/__init__.py
--rw-------   0 root         (0) root         (0)     6369 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/games/free_to_game.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.321000 nokey-0.1.0/nokey/geolocation/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/geolocation/__init__.py
--rw-------   0 root         (0) root         (0)      916 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/geolocation/ip_api.py
--rw-------   0 root         (0) root         (0)     1692 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/geolocation/zippopotamus.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.341000 nokey-0.1.0/nokey/helperFuncs/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/__init__.py
--rw-------   0 root         (0) root         (0)      822 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/get_api_list.py
--rw-------   0 root         (0) root         (0)     1393 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/make_request.py
--rw-------   0 root         (0) root         (0)      576 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/nokey_apis.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.353000 nokey-0.1.0/nokey/inspiration/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/inspiration/__init__.py
--rw-------   0 root         (0) root         (0)     5764 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/inspiration/dictum.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.361000 nokey-0.1.0/nokey/jokes/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/jokes/__init__.py
--rw-------   0 root         (0) root         (0)     2700 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/jokes/joke_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.369000 nokey-0.1.0/nokey/language/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/language/__init__.py
--rw-------   0 root         (0) root         (0)     1013 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/language/free_dictionary.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.381000 nokey-0.1.0/nokey/random/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/random/__init__.py
--rw-------   0 root         (0) root         (0)      932 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/random/random_user.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.389000 nokey-0.1.0/nokey/science/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/science/__init__.py
--rw-------   0 root         (0) root         (0)     2802 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/science/nobel_prize.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.401000 nokey-0.1.0/nokey/spaceflight/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/spaceflight/__init__.py
--rw-------   0 root         (0) root         (0)     8565 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/spaceflight/spaceflight_news.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.409000 nokey-0.1.0/nokey/weather/
--rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/weather/__init__.py
--rw-------   0 root         (0) root         (0)    25903 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/weather/national_weather_service.py
-drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.417000 nokey-0.1.0/nokey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2962 2024-04-14 00:33:38.000000 nokey-0.1.0/nokey.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)     1225 2024-04-14 00:33:39.000000 nokey-0.1.0/nokey.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-14 00:33:38.000000 nokey-0.1.0/nokey.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        6 2024-04-14 00:33:39.000000 nokey-0.1.0/nokey.egg-info/top_level.txt
--rw-rw----   0 root         (0) root         (0)      503 2024-04-14 00:28:11.000000 nokey-0.1.0/pyproject.toml
--rw-------   0 root         (0) root         (0)       38 2024-04-14 00:33:39.425000 nokey-0.1.0/setup.cfg
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.120087 nokey-0.2.0/
+-rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3516 2024-04-20 15:25:31.116087 nokey-0.2.0/PKG-INFO
+-rw-------   0 root         (0) root         (0)     2995 2024-04-20 15:20:37.000000 nokey-0.2.0/README.md
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.872087 nokey-0.2.0/nokey/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/__init__.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.892087 nokey-0.2.0/nokey/activities/
+-rw-------   0 root         (0) root         (0)     5116 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/activities/bored_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.900087 nokey-0.2.0/nokey/animals/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/animals/__init__.py
+-rw-------   0 root         (0) root         (0)     2754 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/animals/dog_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.912087 nokey-0.2.0/nokey/calendar/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/calendar/__init__.py
+-rw-------   0 root         (0) root         (0)     4848 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/calendar/nager_date.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.920087 nokey-0.2.0/nokey/country_info/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/country_info/__init__.py
+-rw-------   0 root         (0) root         (0)     4824 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/country_info/rest_country.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.948087 nokey-0.2.0/nokey/developer_tools/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/__init__.py
+-rw-------   0 root         (0) root         (0)     3945 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/apis_guru.py
+-rw-------   0 root         (0) root         (0)     2578 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/microlink.py
+-rw-------   0 root         (0) root         (0)     7314 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/url_haus.py
+-rw-------   0 root         (0) root         (0)     1621 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/url_shortener.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.960087 nokey-0.2.0/nokey/education/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/education/__init__.py
+-rw-------   0 root         (0) root         (0)     2348 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/education/university_domains_and_names.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.968087 nokey-0.2.0/nokey/finance/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/finance/__init__.py
+-rw-------   0 root         (0) root         (0)     1127 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/finance/wall_street_bets.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.980087 nokey-0.2.0/nokey/food/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/food/__init__.py
+-rw-------   0 root         (0) root         (0)     3198 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/food/fruityvice.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.996087 nokey-0.2.0/nokey/games/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/games/__init__.py
+-rw-------   0 root         (0) root         (0)     6542 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/games/free_to_game.py
+-rw-------   0 root         (0) root         (0)     5382 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/games/open_trivia_db.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.008087 nokey-0.2.0/nokey/geolocation/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/geolocation/__init__.py
+-rw-------   0 root         (0) root         (0)     1045 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/geolocation/ip_api.py
+-rw-------   0 root         (0) root         (0)     1874 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/geolocation/zippopotamus.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.020087 nokey-0.2.0/nokey/government/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/government/__init__.py
+-rw-------   0 root         (0) root         (0)    10654 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/government/federal_register.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.040087 nokey-0.2.0/nokey/helperFuncs/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/__init__.py
+-rw-------   0 root         (0) root         (0)      822 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/get_api_list.py
+-rw-------   0 root         (0) root         (0)     2337 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/make_request.py
+-rw-------   0 root         (0) root         (0)      741 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/nokey_apis.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.048087 nokey-0.2.0/nokey/inspiration/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/inspiration/__init__.py
+-rw-------   0 root         (0) root         (0)     5925 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/inspiration/dictum.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.060087 nokey-0.2.0/nokey/jokes/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/jokes/__init__.py
+-rw-------   0 root         (0) root         (0)     3004 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/jokes/joke_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.068087 nokey-0.2.0/nokey/language/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/language/__init__.py
+-rw-------   0 root         (0) root         (0)     1185 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/language/free_dictionary.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.080087 nokey-0.2.0/nokey/random/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/random/__init__.py
+-rw-------   0 root         (0) root         (0)     1119 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/random/random_user.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.088087 nokey-0.2.0/nokey/science/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/science/__init__.py
+-rw-------   0 root         (0) root         (0)     2948 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/science/nobel_prize.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.096087 nokey-0.2.0/nokey/spaceflight/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/spaceflight/__init__.py
+-rw-------   0 root         (0) root         (0)     8784 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/spaceflight/spaceflight_news.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.108087 nokey-0.2.0/nokey/weather/
+-rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/weather/__init__.py
+-rw-------   0 root         (0) root         (0)    26115 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/weather/national_weather_service.py
+drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.112087 nokey-0.2.0/nokey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3516 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1511 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        6 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)      503 2024-04-20 15:23:04.000000 nokey-0.2.0/pyproject.toml
+-rw-------   0 root         (0) root         (0)       38 2024-04-20 15:25:31.120087 nokey-0.2.0/setup.cfg
```

### Comparing `nokey-0.1.0/LICENSE` & `nokey-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.1.0/PKG-INFO` & `nokey-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: nokey
-Version: 0.1.0
-Summary: A python package for accessing APIs that require no key.
-Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
-Project-URL: Homepage, https://github.com/SpyderRex/nokey
-Project-URL: Issues, https://github.com/Spyder/nokey/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
 
 ## Features
 
 - Access a growing collection of keyless APIs conveniently from one place.
@@ -48,57 +34,88 @@
 ```
 
 Also, to print out a list of the APIs supported by nokey, simply run the following script:
 
 ```python
 from nokey.helperFuncs import get_api_list
 
-api_list = get_api_list()
+api_list = get_api_list.get_api_list()
 
-prrint(api_list)
+print(api_list)
 ```
 
+Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
+
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
-Supported APIs
-## Country Info
+# Supported APIs
+## country_info
 RestCountries
-## Finance
+
+## finance
 Wallstreet Bets
-## Geolocation
+
+## geolocation
 IP API
 Zippopotomus
-## Spaceflight
+
+## spaceflight
 Spaceflight News
-## Education
-University Names and Domains
-## Food
+
+## education
+University Domains and Names
+
+## food
 Fruityvice
-## Random
+
+## random
 RandomUserGenerator
-## Jokes
+
+##jokes
 JokeAPI
-## Animals
+
+## animals
 DogAPI
-## Science
+
+## science
 Nobel Prize API
-## Weather
+
+## weather
 National Weather Service API
-## Inspiration
+
+## developer_tools
+URL Shortener
+URLHaus
+APIsGuru
+Microlink
+
+## inspiration
 Dictum
-## Games
-Free To Game
-## Language
+
+## language
 Free Dictionary
-Developer Tools
-URl Shortener ...
-... and many more on the way.
+
+## games
+Free To Game
+Open Trivia Database
+
+## activities
+Bored API
+
+## calendar
+Nager.Date
+
+## government
+Federal Register
 
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
-Check out the [docs](https://nokey.readthedocs.io/en/latest/)
+Check out the [docs](https://nokey.readthedocs.io/en/latest/).
+
+# Disclaimer:
+Be sure to read the API documentation if you plan to use any of the APIs for development. This package is for accessing keyless, free, open source APIs and I am not responsible for the content of the APIs themselves.
```

### Comparing `nokey-0.1.0/README.md` & `nokey-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: nokey
+Version: 0.2.0
+Summary: A python package for accessing APIs that require no key.
+Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
+Project-URL: Homepage, https://github.com/SpyderRex/nokey
+Project-URL: Issues, https://github.com/Spyder/nokey/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
 
 ## Features
 
 - Access a growing collection of keyless APIs conveniently from one place.
@@ -34,57 +48,88 @@
 ```
 
 Also, to print out a list of the APIs supported by nokey, simply run the following script:
 
 ```python
 from nokey.helperFuncs import get_api_list
 
-api_list = get_api_list()
+api_list = get_api_list.get_api_list()
 
-prrint(api_list)
+print(api_list)
 ```
 
+Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
+
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
-Supported APIs
-## Country Info
+# Supported APIs
+## country_info
 RestCountries
-## Finance
+
+## finance
 Wallstreet Bets
-## Geolocation
+
+## geolocation
 IP API
 Zippopotomus
-## Spaceflight
+
+## spaceflight
 Spaceflight News
-## Education
-University Names and Domains
-## Food
+
+## education
+University Domains and Names
+
+## food
 Fruityvice
-## Random
+
+## random
 RandomUserGenerator
-## Jokes
+
+##jokes
 JokeAPI
-## Animals
+
+## animals
 DogAPI
-## Science
+
+## science
 Nobel Prize API
-## Weather
+
+## weather
 National Weather Service API
-## Inspiration
+
+## developer_tools
+URL Shortener
+URLHaus
+APIsGuru
+Microlink
+
+## inspiration
 Dictum
-## Games
-Free To Game
-## Language
+
+## language
 Free Dictionary
-Developer Tools
-URl Shortener ...
-... and many more on the way.
+
+## games
+Free To Game
+Open Trivia Database
+
+## activities
+Bored API
+
+## calendar
+Nager.Date
+
+## government
+Federal Register
 
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
-Check out the [docs](https://nokey.readthedocs.io/en/latest/)
+Check out the [docs](https://nokey.readthedocs.io/en/latest/).
+
+# Disclaimer:
+Be sure to read the API documentation if you plan to use any of the APIs for development. This package is for accessing keyless, free, open source APIs and I am not responsible for the content of the APIs themselves.
```

### Comparing `nokey-0.1.0/nokey/animals/dog_api.py` & `nokey-0.2.0/nokey/animals/dog_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class DogAPI:
     """
     A class to interact with the Dog API.
     
     Attributes:
     - base_url: The base URL for the API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://dog.ceo/api/"
+        self.about = "The Dog API returns URLs for dog images, either at random or by breed."
         
     def get_docs_url(self):
         """
         Returns the URL for the Dog API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/country_info/rest_country.py` & `nokey-0.2.0/nokey/country_info/rest_country.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 class RestCountries:
     """
     A class to interact with the RestCountries API.
     
     Attributes:
     - base_url: The base URL of the RestCountries API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://restcountries.com/v3.1/"
+        self.about = "REST Countries API is a simple REST API from RapidAPI that provides information about countries in the world In JSON format."
         
     def get_docs_url(self):
         """
         Returns url for API docs.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/developer_tools/url_shortener.py` & `nokey-0.2.0/nokey/developer_tools/url_shortener.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class UrlShortener:
     """
     A class for interacting with the URL Shortener API.
     
     Attributes:
     - base_url: The base URL of the URL Shortener API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://is.gd/create.php?"
+        self.about = "This URL Shortener API (from is.gd) is a URL shortener service."
         
     def get_docs_url(self):
         """
         Returns the URL for the URL Shortener API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/education/university_names_and_domains.py` & `nokey-0.2.0/nokey/education/university_domains_and_names.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .. helperFuncs import make_request as mr
 
-class UniversityNamesAndDomains:
+class UniversityDomainsAndNames:
     """
-    A class to interact with the University Names and Domains API.
+    A class to interact with the University Domains and Names API.
     
     Attributes:
-    - base_url: The base url for the University Names and Domains API.
+    - base_url: The base url for the University Domains and Names API.
+    - about: A short description of the API.
     """
     
     def __init__(self):
         self.base_url = "http://universities.hipolabs.com/search?"
+        self.about = "This API accesses a list of universities and their domain names."
         
     def get_docs_url(self):
         """
-        Returns the url for the University Names and Domains API documentation.
+        Returns the url for the University Domains and Names API documentation.
         
         Args:
         - None
         
         Returns:
         - string: URL for API documentation.
         """
```

### Comparing `nokey-0.1.0/nokey/food/fruityvice.py` & `nokey-0.2.0/nokey/food/fruityvice.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 class Fruityvice:
     """
     A class to interact with the Fruityvice API.
     
     Attributes:
     - base_url: The base url of the Fruityvice API.
+    - about: A short description of the API.
     """
     
     def __init__(self):
         self.base_url = "https://www.fruityvice.com/api/fruit/"
+        self.about = "Fruityvice is an API that provides information on fruits and their nutritional value."
         
     def get_docs_url(self):
         """
         Returns the url for the Fruityvice API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/games/free_to_game.py` & `nokey-0.2.0/nokey/games/free_to_game.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class FreeToGame:
     """
     Class to interact with the Free To Game API.
     
     Attributes:
     - base_url: The base URL of the Free To Game API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://www.freetogame.com/api/"
+        self.about = "The Free To Game API is a way to access programmatically the best free-to-play games and free MMO games."
         
     def get_docs_url(self):
         """
         Returns the URL for the Free To Game API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/geolocation/ip_api.py` & `nokey-0.2.0/nokey/geolocation/ip_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 class IP_API:
     """
     A class to interact with the IP API.
     
     Attributes:
     - base_url: The base URL of IP API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "http://ip-api.com/json/" 
+        self.about = "The IP API is a fast, reliable, and free IP geolocation API."
         
     def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/geolocation/zippopotamus.py` & `nokey-0.2.0/nokey/geolocation/zippopotamus.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class Zippopotomus:
     """
     A class to interact with the Zippopotomus API.
     
     Attributes:
     - base_url: The basee URL of the API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "http://api.zippopotam.us/"
+        self.about = "Zippopotamus is an open source project that is focused on converting zip codes into valid geographical locations."
         
     def get_docs_url(self):
         """
         Returns the URL for the Zippopotomus API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/helperFuncs/get_api_list.py` & `nokey-0.2.0/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.1.0/nokey/helperFuncs/make_request.py` & `nokey-0.2.0/nokey/helperFuncs/make_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,7 +29,35 @@
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
+
+def make_request_with_params(url, params):
+    """
+    Make a request to an API if the API call requires params.
+    
+    Args:
+    - url (str): The base url of the API.
+    - params (dict): The params to be included in the request.
+    
+    Returns:
+    - dict: A dictionary containing either the response data or an error message.
+    """
+    try:
+        response = requests.get(url, params)
+        return response.json()
+    except HTTPError as http_err:
+        # Handle HTTP error
+        return {"error": f"HTTP error occurred: {http_err}"}
+    except Timeout:
+        # Handle timeout error
+        return {"error": "Request timed out."}
+    except RequestException as req_err:
+        # Handle other request exceptions
+        return {"error": f"Request exception occurred: {req_err}"}
+    except Exception as err:
+        # Handle any other unexpected errors
+        return {"error": f"An unexpected error occurred: {err}"}
+
```

### Comparing `nokey-0.1.0/nokey/inspiration/dictum.py` & `nokey-0.2.0/nokey/inspiration/dictum.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class Dictum:
     """
     A class for interacting with the Dictum API.
     
     Attributes:
     - base_url: The base URL of the API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://api.fisenko.net/v1/"
+        self.about = "Dictum API provides a programmatic way to access the most inspiring expressions of humanity."
         
     def get_docs_url(self):
         """
         Returns the URL for the Dictum API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/jokes/joke_api.py` & `nokey-0.2.0/nokey/jokes/joke_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class JokeAPI:
     """
     A class to interact with the JokeAPI API.
     
     Attributes:
     - base_url: Base URL for interacting with the API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://v2.jokeapi.dev/joke/"
+        self.about = "JokeAPI is a REST API that serves uniformly and well formatted jokes. It can be used without any API token, membership, registration or payment. It supports a variety of filters that can be applied to get just the right jokes you need."
         
     def get_docs_url(self):
         """
         Returns the URL for the JokeAPI documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/random/random_user.py` & `nokey-0.2.0/nokey/random/random_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class RandomUserGenerator:
     """
     A class to interact with the Random User Generator API.
     
     Attributes:
     - base_url: The base url of the API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://randomuser.me/api/"
+        self.about = "The Random User Generator API is a free, open-source API for generating random user data, like Lorem Ipsum for people."
         
     def get_docs_url(self):
         """
         Returns the url for the Random User Generator API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/science/nobel_prize.py` & `nokey-0.2.0/nokey/science/nobel_prize.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 class NobelPrizeAPI:
     """
     A class to interact with the Nobel Prize API.
     
     Attributes:
     - base_url: The base url for the Nobel Prize API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://api.nobelprize.org/2.1/"
+        self.about = "The Nobel Prize API returns all information about Laureates and Nobel Prizes."
         
     def get_docs_url(self):
         """
         Returns the URL for the Nobel Prize API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/spaceflight/spaceflight_news.py` & `nokey-0.2.0/nokey/spaceflight/spaceflight_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 class SpaceflightNews:
     
     """
     A class to interact with the Spaceflight News API.
     
     Attributes:
     - base_url: The base URL of the Spaceflight News API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://api.spaceflightnewsapi.net/v4/"
+        self.about = "The Spaceflight News API (SNAPI) is a product by The Space Devs (TSD). It's the most complete and up-to-date spaceflight news API currently available."
         
     def get_docs_url(self):
         """
         Returns the url for the Spaceflight News API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey/weather/national_weather_service.py` & `nokey-0.2.0/nokey/weather/national_weather_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 class NationalWeatherService:
     """
     A class to interact with the National Weather Service API.
     
     Attributes:
     - base_url: The base URL of the National Weather Service API.
+    - about: A short description of the API.
     """
     def __init__(self):
         self.base_url = "https://api.weather.gov/"
+        self.about = "The National Weather Service (NWS) API allows developers access to critical forecasts, alerts, and observations, along with other weather data."
         
     def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
         - None
```

### Comparing `nokey-0.1.0/nokey.egg-info/PKG-INFO` & `nokey-0.2.0/nokey.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,57 +48,88 @@
 ```
 
 Also, to print out a list of the APIs supported by nokey, simply run the following script:
 
 ```python
 from nokey.helperFuncs import get_api_list
 
-api_list = get_api_list()
+api_list = get_api_list.get_api_list()
 
-prrint(api_list)
+print(api_list)
 ```
 
+Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
+
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
-Supported APIs
-## Country Info
+# Supported APIs
+## country_info
 RestCountries
-## Finance
+
+## finance
 Wallstreet Bets
-## Geolocation
+
+## geolocation
 IP API
 Zippopotomus
-## Spaceflight
+
+## spaceflight
 Spaceflight News
-## Education
-University Names and Domains
-## Food
+
+## education
+University Domains and Names
+
+## food
 Fruityvice
-## Random
+
+## random
 RandomUserGenerator
-## Jokes
+
+##jokes
 JokeAPI
-## Animals
+
+## animals
 DogAPI
-## Science
+
+## science
 Nobel Prize API
-## Weather
+
+## weather
 National Weather Service API
-## Inspiration
+
+## developer_tools
+URL Shortener
+URLHaus
+APIsGuru
+Microlink
+
+## inspiration
 Dictum
-## Games
-Free To Game
-## Language
+
+## language
 Free Dictionary
-Developer Tools
-URl Shortener ...
-... and many more on the way.
+
+## games
+Free To Game
+Open Trivia Database
+
+## activities
+Bored API
+
+## calendar
+Nager.Date
+
+## government
+Federal Register
 
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
-Check out the [docs](https://nokey.readthedocs.io/en/latest/)
+Check out the [docs](https://nokey.readthedocs.io/en/latest/).
+
+# Disclaimer:
+Be sure to read the API documentation if you plan to use any of the APIs for development. This package is for accessing keyless, free, open source APIs and I am not responsible for the content of the APIs themselves.
```

### Comparing `nokey-0.1.0/nokey.egg-info/SOURCES.txt` & `nokey-0.2.0/nokey.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 README.md
 pyproject.toml
 nokey/__init__.py
 nokey.egg-info/PKG-INFO
 nokey.egg-info/SOURCES.txt
 nokey.egg-info/dependency_links.txt
 nokey.egg-info/top_level.txt
+nokey/activities/bored_api.py
 nokey/animals/__init__.py
 nokey/animals/dog_api.py
+nokey/calendar/__init__.py
+nokey/calendar/nager_date.py
 nokey/country_info/__init__.py
 nokey/country_info/rest_country.py
 nokey/developer_tools/__init__.py
+nokey/developer_tools/apis_guru.py
+nokey/developer_tools/microlink.py
+nokey/developer_tools/url_haus.py
 nokey/developer_tools/url_shortener.py
 nokey/education/__init__.py
-nokey/education/university_names_and_domains.py
+nokey/education/university_domains_and_names.py
 nokey/finance/__init__.py
 nokey/finance/wall_street_bets.py
 nokey/food/__init__.py
 nokey/food/fruityvice.py
 nokey/games/__init__.py
 nokey/games/free_to_game.py
+nokey/games/open_trivia_db.py
 nokey/geolocation/__init__.py
 nokey/geolocation/ip_api.py
 nokey/geolocation/zippopotamus.py
+nokey/government/__init__.py
+nokey/government/federal_register.py
 nokey/helperFuncs/__init__.py
 nokey/helperFuncs/get_api_list.py
 nokey/helperFuncs/make_request.py
 nokey/helperFuncs/nokey_apis.py
 nokey/inspiration/__init__.py
 nokey/inspiration/dictum.py
 nokey/jokes/__init__.py
```

