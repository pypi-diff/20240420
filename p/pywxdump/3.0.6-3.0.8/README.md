# Comparing `tmp/pywxdump-3.0.6.tar.gz` & `tmp/pywxdump-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywxdump-3.0.6.tar", last modified: Fri Apr 19 11:00:55 2024, max compression
+gzip compressed data, was "pywxdump-3.0.8.tar", last modified: Sat Apr 20 10:42:42 2024, max compression
```

## Comparing `pywxdump-3.0.6.tar` & `pywxdump-3.0.8.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.490700 pywxdump-3.0.6/
--rw-rw-rw-   0        0        0     1147 2024-04-19 10:58:00.000000 pywxdump-3.0.6/LICENSE
--rw-rw-rw-   0        0        0    13955 2024-04-19 11:00:55.490700 pywxdump-3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    13210 2024-04-19 10:58:00.000000 pywxdump-3.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/
--rw-rw-rw-   0        0        0     1341 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/analyzer/
--rw-rw-rw-   0        0        0      645 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/analyzer/__init__.py
--rw-rw-rw-   0        0        0    16241 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/analyzer/chat_analysis.py
--rw-rw-rw-   0        0        0    12514 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/analyzer/db_parsing.py
--rw-rw-rw-   0        0        0    19339 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/analyzer/export_chat.py
--rw-rw-rw-   0        0        0     8690 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/analyzer/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/api/
--rw-rw-rw-   0        0        0      401 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/api/__init__.py
--rw-rw-rw-   0        0        0    26842 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/api/api.py
--rw-rw-rw-   0        0        0     3049 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/api/rjson.py
--rw-rw-rw-   0        0        0     3221 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/api/utils.py
--rw-rw-rw-   0        0        0    23961 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/dbpreprocess/
--rw-rw-rw-   0        0        0     3745 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/__init__.py
--rw-rw-rw-   0        0        0     3288 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/dbbase.py
--rw-rw-rw-   0        0        0    11846 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/parsingMSG.py
--rw-rw-rw-   0        0        0     1037 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/parsingMediaMSG.py
--rw-rw-rw-   0        0        0     6399 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/parsingMicroMsg.py
--rw-rw-rw-   0        0        0     2697 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/parsingOpenIMContact.py
--rw-rw-rw-   0        0        0    12132 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/dbpreprocess/utils.py
--rw-rw-rw-   0        0        0     5094 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/server.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/ui/
--rw-rw-rw-   0        0        0      396 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/ui/templates/
--rw-rw-rw-   0        0        0     2935 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/ui/templates/chat.html
--rw-rw-rw-   0        0        0     8758 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/ui/templates/index.html
--rw-rw-rw-   0        0        0    13425 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/ui/view_chat.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.459450 pywxdump-3.0.6/pywxdump/ui/web/
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.475074 pywxdump-3.0.6/pywxdump/ui/web/assets/
--rw-rw-rw-   0        0        0     8667 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/AboutView-Zw8iwR0j.js
--rw-rw-rw-   0        0        0     2670 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/BiasView-HrnP52sC.js
--rw-rw-rw-   0        0        0    13600 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/ChatView-3ZOUdUTv.css
--rw-rw-rw-   0        0        0    35569 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/ChatView-zX7v9ucw.js
--rw-rw-rw-   0        0        0     1000 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/CleanupView-E355vjQT.js
--rw-rw-rw-   0        0        0      665 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/DateTimeSelect-L-ShBE0O.css
--rw-rw-rw-   0        0        0     2086 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/DecryptView-j3edNkwI.js
--rw-rw-rw-   0        0        0     1010 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/HelpView-8d8K8EDR.js
--rw-rw-rw-   0        0        0      157 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/HomeView-DcUxYQHB.js
--rw-rw-rw-   0        0        0      689 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/HomeView.vue_vue_type_script_setup_true_lang-5w2dEJdv.js
--rw-rw-rw-   0        0        0     1851 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/MergeView-R4wK5Hv8.js
--rw-rw-rw-   0        0        0      501 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/SettingView-7PdMki0v.js
--rw-rw-rw-   0        0        0      856 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/StatisticsView-g0EfwdVR.js
--rw-rw-rw-   0        0        0     2289 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/WxinfoView-dBviDsRz.js
--rw-rw-rw-   0        0        0    29988 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/axios--FnjuHWf.js
--rw-rw-rw-   0        0        0   327609 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/index-55UIhNbb.css
--rw-rw-rw-   0        0        0  2016118 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/assets/index-CtkzF4da.js
--rw-rw-rw-   0        0        0   270398 2024-04-19 10:59:31.000000 pywxdump-3.0.6/pywxdump/ui/web/favicon.ico
--rw-rw-rw-   0        0        0      568 2024-04-19 11:00:50.000000 pywxdump-3.0.6/pywxdump/ui/web/index.html
--rw-rw-rw-   0        0        0     5164 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/version_list.json
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.475074 pywxdump-3.0.6/pywxdump/wx_info/
--rw-rw-rw-   0        0        0      559 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/__init__.py
--rw-rw-rw-   0        0        0     6653 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/decryption.py
--rw-rw-rw-   0        0        0     8257 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/get_bias_addr.py
--rw-rw-rw-   0        0        0    14509 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/get_wx_info.py
--rw-rw-rw-   0        0        0    16574 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/merge_db.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.490700 pywxdump-3.0.6/pywxdump/wx_info/tools/
--rw-rw-rw-   0        0        0  3412992 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/tools/libcrypto-1_1-x64.dll
--rwxrwxrwx   0        0        0  2166272 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/tools/realTime.exe
--rw-rw-rw-   0        0        0     3606 2024-04-19 10:58:00.000000 pywxdump-3.0.6/pywxdump/wx_info/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.490700 pywxdump-3.0.6/pywxdump.egg-info/
--rw-rw-rw-   0        0        0    13955 2024-04-19 11:00:55.000000 pywxdump-3.0.6/pywxdump.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2130 2024-04-19 11:00:55.000000 pywxdump-3.0.6/pywxdump.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 11:00:55.000000 pywxdump-3.0.6/pywxdump.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-19 11:00:55.000000 pywxdump-3.0.6/pywxdump.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      128 2024-04-19 11:00:55.000000 pywxdump-3.0.6/pywxdump.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 11:00:55.000000 pywxdump-3.0.6/pywxdump.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 11:00:55.490700 pywxdump-3.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2179 2024-04-19 10:58:00.000000 pywxdump-3.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:00:55.490700 pywxdump-3.0.6/tests/
--rw-rw-rw-   0        0        0      690 2024-04-19 10:58:00.000000 pywxdump-3.0.6/tests/test_Bias.py
--rw-rw-rw-   0        0        0     1246 2024-04-19 10:58:00.000000 pywxdump-3.0.6/tests/test_dbshow.py
--rw-rw-rw-   0        0        0      590 2024-04-19 10:58:00.000000 pywxdump-3.0.6/tests/test_decrypt.py
--rw-rw-rw-   0        0        0      513 2024-04-19 10:58:00.000000 pywxdump-3.0.6/tests/test_read_info.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.440948 pywxdump-3.0.8/
+-rw-rw-rw-   0        0        0     1147 2024-04-20 10:40:11.000000 pywxdump-3.0.8/LICENSE
+-rw-rw-rw-   0        0        0    13955 2024-04-20 10:42:42.440948 pywxdump-3.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    13210 2024-04-20 10:40:11.000000 pywxdump-3.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.409685 pywxdump-3.0.8/pywxdump/
+-rw-rw-rw-   0        0        0     1341 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.409685 pywxdump-3.0.8/pywxdump/analyzer/
+-rw-rw-rw-   0        0        0      645 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/analyzer/__init__.py
+-rw-rw-rw-   0        0        0    16241 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/analyzer/chat_analysis.py
+-rw-rw-rw-   0        0        0    12514 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/analyzer/db_parsing.py
+-rw-rw-rw-   0        0        0    19339 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/analyzer/export_chat.py
+-rw-rw-rw-   0        0        0     8690 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/analyzer/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.409685 pywxdump-3.0.8/pywxdump/api/
+-rw-rw-rw-   0        0        0      401 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/api/__init__.py
+-rw-rw-rw-   0        0        0    31533 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/api/api.py
+-rw-rw-rw-   0        0        0     3049 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/api/rjson.py
+-rw-rw-rw-   0        0        0     3221 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/api/utils.py
+-rw-rw-rw-   0        0        0    23961 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.425317 pywxdump-3.0.8/pywxdump/dbpreprocess/
+-rw-rw-rw-   0        0        0     3893 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/__init__.py
+-rw-rw-rw-   0        0        0     3288 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/dbbase.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.425317 pywxdump-3.0.8/pywxdump/dbpreprocess/export/
+-rw-rw-rw-   0        0        0      334 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/export/__init__.py
+-rw-rw-rw-   0        0        0     2170 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/export/exportCSV.py
+-rw-rw-rw-   0        0        0     1297 2024-04-20 10:40:11.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/export/exportJSON.py
+-rw-rw-rw-   0        0        0    11962 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/parsingMSG.py
+-rw-rw-rw-   0        0        0     1087 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/parsingMediaMSG.py
+-rw-rw-rw-   0        0        0     6881 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/parsingMicroMsg.py
+-rw-rw-rw-   0        0        0     2746 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/parsingOpenIMContact.py
+-rw-rw-rw-   0        0        0    12132 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/dbpreprocess/utils.py
+-rw-rw-rw-   0        0        0     5094 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/server.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.425317 pywxdump-3.0.8/pywxdump/ui/
+-rw-rw-rw-   0        0        0      396 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.425317 pywxdump-3.0.8/pywxdump/ui/templates/
+-rw-rw-rw-   0        0        0     2935 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/ui/templates/chat.html
+-rw-rw-rw-   0        0        0     8758 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/ui/templates/index.html
+-rw-rw-rw-   0        0        0    13425 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/ui/view_chat.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.425317 pywxdump-3.0.8/pywxdump/ui/web/
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.425317 pywxdump-3.0.8/pywxdump/ui/web/assets/
+-rw-rw-rw-   0        0        0     8667 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/AboutView-YDN8Uqso.js
+-rw-rw-rw-   0        0        0     2670 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/BiasView-8tCrt-Mg.js
+-rw-rw-rw-   0        0        0    13600 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/ChatView-I_cUSrgs.css
+-rw-rw-rw-   0        0        0    36210 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/ChatView-PSmCcQTu.js
+-rw-rw-rw-   0        0        0     1000 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/CleanupView-JwdNAC7i.js
+-rw-rw-rw-   0        0        0      665 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/DateTimeSelect-_xTa7bZL.css
+-rw-rw-rw-   0        0        0     2086 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/DecryptView-emfcQg74.js
+-rw-rw-rw-   0        0        0     1010 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/HelpView-eMRBH9mj.js
+-rw-rw-rw-   0        0        0      157 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/HomeView-oLhVq41M.js
+-rw-rw-rw-   0        0        0      689 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/HomeView.vue_vue_type_script_setup_true_lang-dZI7DIut.js
+-rw-rw-rw-   0        0        0     1851 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/MergeView-pn-ejbod.js
+-rw-rw-rw-   0        0        0      501 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/SettingView-LZJej87E.js
+-rw-rw-rw-   0        0        0      856 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/StatisticsView-sWS8TEdn.js
+-rw-rw-rw-   0        0        0     2289 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/WxinfoView-UlpcKPEi.js
+-rw-rw-rw-   0        0        0    29988 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/axios--FnjuHWf.js
+-rw-rw-rw-   0        0        0   327609 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/index-55UIhNbb.css
+-rw-rw-rw-   0        0        0  2016118 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/assets/index-VdcdRmrH.js
+-rw-rw-rw-   0        0        0   270398 2024-04-20 10:41:26.000000 pywxdump-3.0.8/pywxdump/ui/web/favicon.ico
+-rw-rw-rw-   0        0        0      568 2024-04-20 10:42:37.000000 pywxdump-3.0.8/pywxdump/ui/web/index.html
+-rw-rw-rw-   0        0        0     5164 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/version_list.json
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.440948 pywxdump-3.0.8/pywxdump/wx_info/
+-rw-rw-rw-   0        0        0      559 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/__init__.py
+-rw-rw-rw-   0        0        0     6653 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/decryption.py
+-rw-rw-rw-   0        0        0     8257 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/get_bias_addr.py
+-rw-rw-rw-   0        0        0    14509 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/get_wx_info.py
+-rw-rw-rw-   0        0        0    16605 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/merge_db.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.440948 pywxdump-3.0.8/pywxdump/wx_info/tools/
+-rw-rw-rw-   0        0        0  3412992 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/tools/libcrypto-1_1-x64.dll
+-rwxrwxrwx   0        0        0  2166272 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/tools/realTime.exe
+-rw-rw-rw-   0        0        0     3606 2024-04-20 10:40:12.000000 pywxdump-3.0.8/pywxdump/wx_info/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.440948 pywxdump-3.0.8/pywxdump.egg-info/
+-rw-rw-rw-   0        0        0    13955 2024-04-20 10:42:42.000000 pywxdump-3.0.8/pywxdump.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2024-04-20 10:42:42.000000 pywxdump-3.0.8/pywxdump.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 10:42:42.000000 pywxdump-3.0.8/pywxdump.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-20 10:42:42.000000 pywxdump-3.0.8/pywxdump.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      128 2024-04-20 10:42:42.000000 pywxdump-3.0.8/pywxdump.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 10:42:42.000000 pywxdump-3.0.8/pywxdump.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 10:42:42.440948 pywxdump-3.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2293 2024-04-20 10:40:12.000000 pywxdump-3.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:42:42.440948 pywxdump-3.0.8/tests/
+-rw-rw-rw-   0        0        0      690 2024-04-20 10:40:12.000000 pywxdump-3.0.8/tests/test_Bias.py
+-rw-rw-rw-   0        0        0     1246 2024-04-20 10:40:12.000000 pywxdump-3.0.8/tests/test_dbshow.py
+-rw-rw-rw-   0        0        0      590 2024-04-20 10:40:12.000000 pywxdump-3.0.8/tests/test_decrypt.py
+-rw-rw-rw-   0        0        0      513 2024-04-20 10:40:12.000000 pywxdump-3.0.8/tests/test_read_info.py
```

### Comparing `pywxdump-3.0.6/LICENSE` & `pywxdump-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/PKG-INFO` & `pywxdump-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdump
-Version: 3.0.6
+Version: 3.0.8
 Summary: 微信信息获取工具
 Home-page: https://github.com/xaoyaoo/PyWxDump
 Author: xaoyaoo
 Author-email: xaoyaoo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pywxdump-3.0.6/README.md` & `pywxdump-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/__init__.py` & `pywxdump-3.0.8/pywxdump/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 except:
     VERSION_LIST = {}
     VERSION_LIST_PATH = None
 
 PYWXDUMP_ROOT_PATH = os.path.dirname(__file__)
 db_init = DBPool("DBPOOL_INIT")
 
-__version__ = "3.0.6"
+__version__ = "3.0.8"
```

### Comparing `pywxdump-3.0.6/pywxdump/analyzer/__init__.py` & `pywxdump-3.0.8/pywxdump/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/analyzer/chat_analysis.py` & `pywxdump-3.0.8/pywxdump/analyzer/chat_analysis.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/analyzer/db_parsing.py` & `pywxdump-3.0.8/pywxdump/analyzer/db_parsing.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/analyzer/export_chat.py` & `pywxdump-3.0.8/pywxdump/analyzer/export_chat.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/analyzer/utils.py` & `pywxdump-3.0.8/pywxdump/analyzer/utils.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/api/api.py` & `pywxdump-3.0.8/pywxdump/api/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pywxdump.analyzer.export_chat import get_contact, get_room_user_list
 from pywxdump.api.rjson import ReJson, RqJson
 from pywxdump.api.utils import read_session, get_session_wxids, save_session, error9999, gen_base64, validate_title
 from pywxdump import read_info, VERSION_LIST, batch_decrypt, BiasAddr, merge_db, decrypt_merge, merge_real_time_db
 import pywxdump
 from pywxdump.dbpreprocess import wxid2userinfo, ParsingMSG, get_user_list, get_recent_user_list, ParsingMediaMSG, \
     download_file
+from pywxdump.dbpreprocess import export_csv,export_json
 
 # app = Flask(__name__, static_folder='../ui/web/dist', static_url_path='/')
 
 api = Blueprint('api', __name__, template_folder='../ui/web', static_folder='../ui/web/assets/', )
 api.debug = False
 
 
@@ -131,18 +132,18 @@
         "key": "",
         "my_wxid": my_wxid,
         "is_init": True,
     }
     return ReJson(0, rdata)
 
 
-# END 以上为初始化相关 ****************************************************************************************************
+# END 以上为初始化相关 ***************************************************************************************************
 
 
-# start 以下为聊天联系人相关api ******************************************************************************************
+# start 以下为聊天联系人相关api *******************************************************************************************
 
 @api.route('/api/recent_user_list', methods=["GET", 'POST'])
 @error9999
 def recent_user_list():
     """
     获取联系人列表
     :return:
@@ -433,15 +434,133 @@
     if not os.path.exists(all_file_path):
         return ReJson(5002)
     return send_file(all_file_path)
 
 
 # end 以上为聊天记录相关api *********************************************************************************************
 
-# 导出聊天记录
+# start 导出聊天记录 *****************************************************************************************************
+
+@api.route('/api/export_endb', methods=["GET", 'POST'])
+def get_export_endb():
+    """
+    导出加密数据库
+    :return:
+    """
+    my_wxid = read_session(g.sf, "test", "last")
+    if not my_wxid: return ReJson(1001, body="my_wxid is required")
+    wx_path = read_session(g.sf, my_wxid, "wx_path")
+    wx_path = request.json.get("wx_path", wx_path)
+
+    if not wx_path:
+        return ReJson(1002, body=f"wx_path is required: {wx_path}")
+    if not os.path.exists(wx_path):
+        return ReJson(1001, body=f"wx_path not exists: {wx_path}")
+
+    # 分割wx_path的文件名和父目录
+    code, wxdbpaths = get_core_db(wx_path)
+    if not code:
+        return ReJson(2001, body=wxdbpaths)
+
+    outpath = os.path.join(g.tmp_path, "export", my_wxid, "endb")
+    if not os.path.exists(outpath):
+        os.makedirs(outpath)
+
+    for wxdb in wxdbpaths:
+        # 复制wxdb->outpath, os.path.basename(wxdb)
+        assert isinstance(outpath, str)  # 为了解决pycharm的警告, 无实际意义
+        shutil.copy(wxdb, os.path.join(outpath, os.path.basename(wxdb)))
+    return ReJson(0, body=outpath)
+
+
+@api.route('/api/export_dedb', methods=["GET", "POST"])
+def get_export_dedb():
+    """
+    导出解密数据库
+    :return:
+    """
+    my_wxid = read_session(g.sf, "test", "last")
+    if not my_wxid: return ReJson(1001, body="my_wxid is required")
+
+    key = request.json.get("key", read_session(g.sf, my_wxid, "key"))
+    wx_path = request.json.get("wx_path", read_session(g.sf, my_wxid, "wx_path"))
+
+    if not key:
+        return ReJson(1002, body=f"key is required: {key}")
+    if not wx_path:
+        return ReJson(1002, body=f"wx_path is required: {wx_path}")
+    if not os.path.exists(wx_path):
+        return ReJson(1001, body=f"wx_path not exists: {wx_path}")
+
+    outpath = os.path.join(g.tmp_path, "export", my_wxid, "dedb")
+    if not os.path.exists(outpath):
+        os.makedirs(outpath)
+
+    code, merge_save_path = decrypt_merge(wx_path=wx_path, key=key, outpath=outpath)
+    time.sleep(1)
+    if code:
+        return ReJson(0, body=merge_save_path)
+    else:
+        return ReJson(2001, body=merge_save_path)
+
+
+@api.route('/api/export_csv', methods=["GET", 'POST'])
+def get_export_csv():
+    """
+    导出csv
+    :return:
+    """
+    my_wxid = read_session(g.sf, "test", "last")
+    if not my_wxid: return ReJson(1001, body="my_wxid is required")
+
+    wxid = request.json.get("wxid")
+    # st_ed_time = request.json.get("datetime", [0, 0])
+    if not wxid:
+        return ReJson(1002, body=f"username is required: {wxid}")
+    # if not isinstance(st_ed_time, list) or len(st_ed_time) != 2:
+    #     return ReJson(1002, body=f"datetime is required: {st_ed_time}")
+    # start, end = st_ed_time
+    # if not isinstance(start, int) or not isinstance(end, int) or start >= end:
+    #     return ReJson(1002, body=f"datetime is required: {st_ed_time}")
+
+    outpath = os.path.join(g.tmp_path, "export", my_wxid, "csv", wxid)
+    if not os.path.exists(outpath):
+        os.makedirs(outpath)
+
+    code, ret = export_csv(wxid, outpath, read_session(g.sf, my_wxid, "merge_path"))
+    if code:
+        return ReJson(0, ret)
+    else:
+        return ReJson(2001, body=ret)
+
+
+@api.route('/api/export_json', methods=["GET", 'POST'])
+def get_export_json():
+    """
+    导出json
+    :return:
+    """
+    my_wxid = read_session(g.sf, "test", "last")
+    if not my_wxid: return ReJson(1001, body="my_wxid is required")
+
+    wxid = request.json.get("wxid")
+    if not wxid:
+        return ReJson(1002, body=f"username is required: {wxid}")
+
+    outpath = os.path.join(g.tmp_path, "export", my_wxid, "json", wxid)
+    if not os.path.exists(outpath):
+        os.makedirs(outpath)
+
+    code, ret = export_json(wxid, outpath, read_session(g.sf, my_wxid, "merge_path"))
+    if code:
+        return ReJson(0, ret)
+    else:
+        return ReJson(2001, body=ret)
+
+
 @api.route('/api/export', methods=["GET", 'POST'])
 @error9999
 def export():
     """
     导出聊天记录
     :return:
     """
@@ -617,15 +736,18 @@
         pass
     else:
         return ReJson(1002)
 
     return ReJson(9999, "")
 
 
-# 这部分为专业工具的api
+# end 导出聊天记录 *******************************************************************************************************
+
+# start 这部分为专业工具的api *********************************************************************************************
+
 @api.route('/api/wxinfo', methods=["GET", 'POST'])
 @error9999
 def get_wxinfo():
     """
     获取微信信息
     :return:
     """
@@ -688,17 +810,17 @@
     out_path = request.json.get("outPath")
     if not out_path:
         return ReJson(1002)
     rdata = merge_db(wxdb_path, out_path)
     return ReJson(0, str(rdata))
 
 
-# END 这部分为专业工具的api
+# END 这部分为专业工具的api ***********************************************************************************************
 
-# 关于、帮助、设置
+# 关于、帮助、设置 *******************************************************************************************************
 @api.route('/api/check_update', methods=["GET", 'POST'])
 @error9999
 def check_update():
     """
     检查更新
     :return:
     """
@@ -727,14 +849,14 @@
     """
     版本
     :return:
     """
     return ReJson(0, pywxdump.__version__)
 
 
-# END 关于、帮助、设置
+# END 关于、帮助、设置 ***************************************************************************************************
 
 
 @api.route('/')
 @error9999
 def index():
     return render_template('index.html')
```

### Comparing `pywxdump-3.0.6/pywxdump/api/rjson.py` & `pywxdump-3.0.8/pywxdump/api/rjson.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/api/utils.py` & `pywxdump-3.0.8/pywxdump/api/utils.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/cli.py` & `pywxdump-3.0.8/pywxdump/cli.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/__init__.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 from .parsingMSG import ParsingMSG
 from .parsingMicroMsg import ParsingMicroMsg
 from .parsingMediaMSG import ParsingMediaMSG
 from .parsingOpenIMContact import ParsingOpenIMContact
 from .utils import download_file
 
+from .export.exportCSV import export_csv
+from .export.exportJSON import export_json
+
 
 def get_user_list(MicroMsg_db_path, OpenIMContact_db_path=None, word=None):
     """
     获取联系人列表
     :param MicroMsg_db_path: MicroMsg.db 文件路径
     :return: 联系人列表
     """
@@ -61,15 +64,15 @@
     return users
 
 
 def wxid2userinfo(MicroMsg_db_path, OpenIMContact_db_path, wxid):
     """
     获取联系人信息
     :param MicroMsg_db_path: MicroMsg.db 文件路径
-    :param wxid: 微信id
+    :param wxid: 微信id,可以是单个id，也可以是多个id，使用list传入
     :return: 联系人信息 {wxid: {wxid: wxid, nickname: nickname, remark: remark, account: account, describe: describe, headImgUrl: headImgUrl}}
     """
     # 连接 MicroMsg.db 数据库，并执行查询
     parsing_micromsg = ParsingMicroMsg(MicroMsg_db_path)
     users = parsing_micromsg.wxid2userinfo(wxid)
     # {'wxid_uw8ruinee7zq12': {'wxid': 'wxid_uw8ruinee7zq12', 'nickname': '2021年', 'remark': '于浩', 'account': 'yh13327404424', 'describe': '', 'headImgUrl': 'https://wx.qlogo.cn/mmhead/ver_1/LLibM2qUys7nBt9Hl8uuTQkn9ILFicoImlt2616ZNGoIvRbA8VmJ0Vibhd3V96JFfxQ25Tj1nRWTsXYDdH3z2FAQkQDXSnjS5PBuSraey4ZnoooOkEu2e3DjXbJaJJXKUib1/0'}}
     # 如果有 OpenIMContact.db 文件，获取 OpenIMContact.db 中的联系人信息
```

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/dbbase.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/dbbase.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/parsingMSG.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/parsingMSG.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,22 +46,24 @@
         except Exception as e:
             return None
 
     def msg_count(self, wxid: str = ""):
         """
         获取聊天记录数量,根据wxid获取单个联系人的聊天记录数量，不传wxid则获取所有联系人的聊天记录数量
         :param MSG_db_path: MSG.db 文件路径
-        :return: 聊天记录数量列表
+        :return: 聊天记录数量列表 {wxid: chat_count}
         """
         if wxid:
             sql = f"SELECT StrTalker, COUNT(*) FROM MSG WHERE StrTalker='{wxid}';"
         else:
             sql = f"SELECT StrTalker, COUNT(*) FROM MSG GROUP BY StrTalker ORDER BY COUNT(*) DESC;"
 
         result = self.execute_sql(sql)
+        if not result:
+            return {}
         df = pd.DataFrame(result, columns=["wxid", "msg_count"])
         # # 排序
         df = df.sort_values(by="msg_count", ascending=False)
         # chat_counts ： {wxid: chat_count}
         chat_counts = df.set_index("wxid").to_dict()["msg_count"]
         return chat_counts
 
@@ -253,15 +255,16 @@
                 "ORDER BY CreateTime ASC LIMIT ?,?")
             result1 = self.execute_sql(sql, (wxid, start_index, page_size))
         else:
             sql = (
                 "SELECT localId, IsSender, StrContent, StrTalker, Sequence, Type, SubType,CreateTime,MsgSvrID,DisplayContent,CompressContent,BytesExtra,ROW_NUMBER() OVER (ORDER BY CreateTime ASC) AS id "
                 "FROM MSG ORDER BY CreateTime ASC LIMIT ?,?")
             result1 = self.execute_sql(sql, (start_index, page_size))
-
+        if not result1:
+            return [], []
         data = []
         wxid_list = []
         for row in result1:
             tmpdata = self.msg_detail(row)
             wxid_list.append(tmpdata["talker"])
             data.append(tmpdata)
         wxid_list = list(set(wxid_list))
```

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/parsingMediaMSG.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/parsingMediaMSG.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     _class_name = "MediaMSG"
     def __init__(self, db_path):
         super().__init__(db_path)
 
     def get_audio(self, MsgSvrID, is_play=False, is_wave=False, save_path=None, rate=24000):
         sql = "select Buf from Media where Reserved0=? "
         DBdata = self.execute_sql(sql, (MsgSvrID,))
+        if not DBdata:
+            return False
         if len(DBdata) == 0:
             return False
         data = DBdata[0][0]  # [1:] + b'\xFF\xFF'
         try:
             pcm_data = silk2audio(buf_data=data, is_play=is_play, is_wave=is_wave, save_path=save_path, rate=rate)
             return pcm_data
         except Exception as e:
```

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/parsingMicroMsg.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/parsingMicroMsg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-#
 # -------------------------------------------------------------------------------
 # Name:         parsingMicroMsg.py
 # Description:  
 # Author:       xaoyaoo
 # Date:         2024/04/15
 # -------------------------------------------------------------------------------
+import logging
+
 from .dbbase import DatabaseBase
 from .utils import timestamp2str, bytes2str
 
 import blackboxprotobuf
 
 
 class ParsingMicroMsg(DatabaseBase):
@@ -36,15 +38,15 @@
             return data
         except Exception as e:
             return None
 
     def wxid2userinfo(self, wxid):
         """
         获取单个联系人信息
-        :param wxid: 微信id
+        :param wxid: 微信id,可以是单个id，也可以是id列表
         :return: 联系人信息
         """
         if isinstance(wxid, str):
             wxid = [wxid]
         elif isinstance(wxid, list):
             wxid = wxid
         else:
@@ -84,14 +86,16 @@
                               f"A.UserName LIKE '%{word}%' "
                               f"OR A.NickName LIKE '%{word}%' "
                               f"OR A.Remark LIKE '%{word}%' "
                               f"OR A.Alias LIKE '%{word}%' "
                               # f"OR A.Reserved6 LIKE '%{word}%' "
                               "ORDER BY A.NickName DESC;")
         result = self.execute_sql(sql)
+        if not result:
+            return []
         for row in result:
             # 获取wxid,昵称，备注，描述，头像
             username, nickname, remark, Alias, describe, headImgUrl = row
             users.append(
                 {"wxid": username, "nickname": nickname, "remark": remark, "account": Alias,
                  "describe": describe, "headImgUrl": headImgUrl})
         return users
@@ -103,14 +107,16 @@
         """
         users = []
         sql = (
             "SELECT C.Username, C.LastReadedCreateTime,C.LastReadedSvrId "
             "FROM ChatInfo C "
             "ORDER BY C.LastReadedCreateTime DESC;")
         result = self.execute_sql(sql)
+        if not result:
+            return []
         for row in result:
             # 获取用户名、昵称、备注和聊天记录数量
             username, LastReadedCreateTime, LastReadedSvrId = row
             LastReadedCreateTime = timestamp2str(LastReadedCreateTime / 1000) if LastReadedCreateTime else None
             users.append(
                 {"wxid": username, "LastReadedCreateTime": LastReadedCreateTime, "LastReadedSvrId": LastReadedSvrId})
         return users
@@ -126,29 +132,35 @@
         sql = (
             "SELECT A.ChatRoomName,A.UserNameList, A.DisplayNameList,A.RoomData, B.Announcement,B.AnnouncementEditor "
             "FROM ChatRoom A,ChatRoomInfo B "
             "where A.ChatRoomName==B.ChatRoomName "
             "ORDER BY A.ChatRoomName ASC;")
         if roomwxid:
             sql = sql.replace("ORDER BY A.ChatRoomName ASC;",
-                              f"where A.ChatRoomName LIKE '%{roomwxid}%' "
+                              f"and A.ChatRoomName LIKE '%{roomwxid}%' "
                               "ORDER BY A.ChatRoomName ASC;")
         result = self.execute_sql(sql)
+        if not result:
+            return []
         room_datas = []
         for row in result:
             # 获取用户名、昵称、备注和聊天记录数量
             ChatRoomName, UserNameList, DisplayNameList, RoomData, Announcement, AnnouncementEditor = row
             UserNameList = UserNameList.split("^G")
             DisplayNameList = DisplayNameList.split("^G")
             RoomData = self.ChatRoom_RoomData(RoomData)
-            rd = []
+            wxid2remark = {}
             if RoomData:
+                rd = []
                 for k, v in RoomData.items():
                     if isinstance(v, list):
                         rd += v
-                room_datas.append(rd)
-            else:
-                print(f"ChatRoomName:{ChatRoomName} RoomData is None")
+                for i in rd:
+                    try:
+                        if isinstance(i, dict) and isinstance(i.get('1'),str) and i.get('2'):
+                            wxid2remark[i['1']] = i["2"]
+                    except Exception as e:
+                        logging.error(f"wxid2remark: ChatRoomName:{ChatRoomName}, {i} error:{e}")
             rooms.append(
                 {"ChatRoomName": ChatRoomName, "UserNameList": UserNameList, "DisplayNameList": DisplayNameList,
-                 "Announcement": Announcement, "AnnouncementEditor": AnnouncementEditor})
+                 "Announcement": Announcement, "AnnouncementEditor": AnnouncementEditor, "wxid2remark": wxid2remark})
         return rooms
```

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/parsingOpenIMContact.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/parsingOpenIMContact.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,25 +47,28 @@
 
     def user_list(self, word=None):
         """
         获取联系人列表
         :param MicroMsg_db_path: MicroMsg.db 文件路径
         :return: 联系人列表
         """
-        users = []
         sql = ("SELECT A.UserName, A.NickName, A.Remark,A.BigHeadImgUrl FROM OpenIMContact A "
                "ORDER BY NickName ASC;")
         if word:
             sql = sql.replace("ORDER BY NickName ASC;",
                               f"where "
                               f"UserName LIKE '%{word}%' "
                               f"OR NickName LIKE '%{word}%' "
                               f"OR Remark LIKE '%{word}%' "
                               "ORDER BY NickName ASC;")
         result = self.execute_sql(sql)
+        if not result:
+            return []
+
+        users = []
         for row in result:
             # 获取用户名、昵称、备注和聊天记录数量
             username, nickname, remark, headImgUrl = row
             users.append(
                 {"wxid": username, "nickname": nickname, "remark": remark, "account": "", "describe": "",
                  "headImgUrl": headImgUrl})
         return users
```

### Comparing `pywxdump-3.0.6/pywxdump/dbpreprocess/utils.py` & `pywxdump-3.0.8/pywxdump/dbpreprocess/utils.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/server.py` & `pywxdump-3.0.8/pywxdump/server.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/templates/chat.html` & `pywxdump-3.0.8/pywxdump/ui/templates/chat.html`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/templates/index.html` & `pywxdump-3.0.8/pywxdump/ui/templates/index.html`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/view_chat.py` & `pywxdump-3.0.8/pywxdump/ui/view_chat.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/AboutView-Zw8iwR0j.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/AboutView-YDN8Uqso.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,18 +2,18 @@
     d as h,
     b as u,
     c as r,
     e as o,
     h as y,
     f as c,
     u as x,
-    s as n,
-    q as d,
+    z as n,
+    y as d,
     M as g
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 import {
     h as b
 } from "./axios--FnjuHWf.js";
 const l = {
         class: "about"
     },
     w = o("h1", null, null, -1),
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/BiasView-HrnP52sC.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/BiasView-8tCrt-Mg.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     b as f,
     c as V,
     e,
     f as o,
     g as w,
     a as m,
     h as x
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const g = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
         }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/ChatView-3ZOUdUTv.css` & `pywxdump-3.0.8/pywxdump/ui/web/assets/ChatView-I_cUSrgs.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-.chat-content[data-v-d930be9e]{width:100%;padding:20px}.chat-content .word[data-v-d930be9e]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-d930be9e]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-d930be9e]{margin-left:10px}.chat-content .word .info .time[data-v-d930be9e]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-d930be9e]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px;display:inline-block}.chat-content .word .info .info-content[data-v-d930be9e]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-d930be9e]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-d930be9e]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-d930be9e]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-d930be9e]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-d930be9e]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left;display:inline-block}.chat-content .word-my .info .info-content[data-v-d930be9e]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content[data-v-24d6aaa0]{width:100%;padding:20px}.chat-content .word[data-v-24d6aaa0]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-24d6aaa0]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-24d6aaa0]{margin-left:10px}.chat-content .word .info .time[data-v-24d6aaa0]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-24d6aaa0]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-24d6aaa0]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-24d6aaa0]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-24d6aaa0]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-24d6aaa0]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-24d6aaa0]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-24d6aaa0]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-24d6aaa0]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-24d6aaa0]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-24d6aaa0]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-24d6aaa0],.demo-image__error .image-slot .el-icon[data-v-24d6aaa0]{font-size:30px}.demo-image__error .el-image[data-v-24d6aaa0]{width:100%;height:200px}.chat-content[data-v-5aa79515]{width:100%;padding:20px}.chat-content .word[data-v-5aa79515]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-5aa79515]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-5aa79515]{margin-left:10px}.chat-content .word .info .time[data-v-5aa79515]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-5aa79515]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-5aa79515]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-5aa79515]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-5aa79515]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-5aa79515]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-5aa79515]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-5aa79515]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-5aa79515]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-5aa79515]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-5aa79515]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-5aa79515],.demo-image__error .image-slot .el-icon[data-v-5aa79515]{font-size:30px}.demo-image__error .el-image[data-v-5aa79515]{width:100%;height:200px}.demo-video__preview[data-v-5aa79515]{padding-left:5px;padding-right:5px}.chat-content[data-v-0d0f2cd4]{width:100%;padding:20px}.chat-content .word[data-v-0d0f2cd4]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-0d0f2cd4]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-0d0f2cd4]{margin-left:10px}.chat-content .word .info .time[data-v-0d0f2cd4]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-0d0f2cd4]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-0d0f2cd4]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-0d0f2cd4]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-0d0f2cd4]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-0d0f2cd4]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-0d0f2cd4]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-0d0f2cd4]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-0d0f2cd4]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left;display:inline-block}.chat-content .word-my .info .chat_img[data-v-0d0f2cd4]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-0d0f2cd4]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-0d0f2cd4],.demo-image__error .image-slot .el-icon[data-v-0d0f2cd4]{font-size:30px}.demo-image__error .el-image[data-v-0d0f2cd4]{width:100%;height:200px}.chat-content[data-v-e797f204]{width:100%;padding:20px}.chat-content .word[data-v-e797f204]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-e797f204]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-e797f204]{margin-left:10px}.chat-content .word .info .time[data-v-e797f204]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-e797f204]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-e797f204]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-e797f204]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-e797f204]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-e797f204]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-e797f204]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-e797f204]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-e797f204]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-e797f204]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-e797f204]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-e797f204],.demo-image__error .image-slot .el-icon[data-v-e797f204]{font-size:30px}.demo-image__error .el-image[data-v-e797f204]{width:100%;height:200px}.demo-video__preview[data-v-e797f204]{padding-left:5px;padding-right:5px}.chat-content[data-v-ad34c109]{width:100%;padding:20px}.chat-content .word[data-v-ad34c109]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-ad34c109]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-ad34c109]{margin-left:10px}.chat-content .word .info .time[data-v-ad34c109]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-ad34c109]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-ad34c109]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-ad34c109]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-ad34c109]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-ad34c109]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-ad34c109]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-ad34c109]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-ad34c109]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-ad34c109]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-ad34c109]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-ad34c109],.demo-image__error .image-slot .el-icon[data-v-ad34c109]{font-size:30px}.demo-image__error .el-image[data-v-ad34c109]{width:100%;height:200px}.chat-content[data-v-e529325a]{width:100%;padding:20px}.chat-content .word[data-v-e529325a]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-e529325a]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-e529325a]{margin-left:10px}.chat-content .word .info .time[data-v-e529325a]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-e529325a]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px;display:inline-block}.chat-content .word .info .info-content[data-v-e529325a]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-e529325a]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-e529325a]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-e529325a]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-e529325a]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-e529325a]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left;display:inline-block}.chat-content .word-my .info .info-content[data-v-e529325a]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}#chat[data-v-09ca318b]{position:relative;width:100%;height:100%;background-color:#f5f5f5;display:flex;flex-direction:column}#chat[data-v-09ca318b] .chat_body[data-v-09ca318b]{flex:1;overflow-y:hidden;overflow-x:hidden}#chat[data-v-09ca318b] .chat_body[data-v-09ca318b] .chat_window[data-v-09ca318b]{height:100%;overflow-y:scroll;width:calc(100% + 17px);padding:0;margin:0}#chat[data-v-09ca318b] .chat_body[data-v-09ca318b] .chat_window[data-v-09ca318b]>.message[data-v-09ca318b]:last-of-type{margin-bottom:8px}
+.chat-content[data-v-d930be9e]{width:100%;padding:20px}.chat-content .word[data-v-d930be9e]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-d930be9e]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-d930be9e]{margin-left:10px}.chat-content .word .info .time[data-v-d930be9e]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-d930be9e]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px;display:inline-block}.chat-content .word .info .info-content[data-v-d930be9e]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-d930be9e]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-d930be9e]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-d930be9e]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-d930be9e]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-d930be9e]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left;display:inline-block}.chat-content .word-my .info .info-content[data-v-d930be9e]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content[data-v-24d6aaa0]{width:100%;padding:20px}.chat-content .word[data-v-24d6aaa0]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-24d6aaa0]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-24d6aaa0]{margin-left:10px}.chat-content .word .info .time[data-v-24d6aaa0]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-24d6aaa0]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-24d6aaa0]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-24d6aaa0]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-24d6aaa0]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-24d6aaa0]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-24d6aaa0]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-24d6aaa0]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-24d6aaa0]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-24d6aaa0]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-24d6aaa0]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-24d6aaa0],.demo-image__error .image-slot .el-icon[data-v-24d6aaa0]{font-size:30px}.demo-image__error .el-image[data-v-24d6aaa0]{width:100%;height:200px}.chat-content[data-v-5aa79515]{width:100%;padding:20px}.chat-content .word[data-v-5aa79515]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-5aa79515]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-5aa79515]{margin-left:10px}.chat-content .word .info .time[data-v-5aa79515]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-5aa79515]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-5aa79515]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-5aa79515]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-5aa79515]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-5aa79515]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-5aa79515]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-5aa79515]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-5aa79515]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-5aa79515]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-5aa79515]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-5aa79515],.demo-image__error .image-slot .el-icon[data-v-5aa79515]{font-size:30px}.demo-image__error .el-image[data-v-5aa79515]{width:100%;height:200px}.demo-video__preview[data-v-5aa79515]{padding-left:5px;padding-right:5px}.chat-content[data-v-0d0f2cd4]{width:100%;padding:20px}.chat-content .word[data-v-0d0f2cd4]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-0d0f2cd4]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-0d0f2cd4]{margin-left:10px}.chat-content .word .info .time[data-v-0d0f2cd4]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-0d0f2cd4]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-0d0f2cd4]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-0d0f2cd4]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-0d0f2cd4]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-0d0f2cd4]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-0d0f2cd4]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-0d0f2cd4]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-0d0f2cd4]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left;display:inline-block}.chat-content .word-my .info .chat_img[data-v-0d0f2cd4]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-0d0f2cd4]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-0d0f2cd4],.demo-image__error .image-slot .el-icon[data-v-0d0f2cd4]{font-size:30px}.demo-image__error .el-image[data-v-0d0f2cd4]{width:100%;height:200px}.chat-content[data-v-e797f204]{width:100%;padding:20px}.chat-content .word[data-v-e797f204]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-e797f204]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-e797f204]{margin-left:10px}.chat-content .word .info .time[data-v-e797f204]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-e797f204]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-e797f204]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-e797f204]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-e797f204]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-e797f204]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-e797f204]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-e797f204]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-e797f204]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-e797f204]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-e797f204]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-e797f204],.demo-image__error .image-slot .el-icon[data-v-e797f204]{font-size:30px}.demo-image__error .el-image[data-v-e797f204]{width:100%;height:200px}.demo-video__preview[data-v-e797f204]{padding-left:5px;padding-right:5px}.chat-content[data-v-ad34c109]{width:100%;padding:20px}.chat-content .word[data-v-ad34c109]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-ad34c109]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-ad34c109]{margin-left:10px}.chat-content .word .info .time[data-v-ad34c109]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-ad34c109]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px}.chat-content .word .info .chat_img[data-v-ad34c109]{width:200px;height:200px;border-radius:5px}.chat-content .word .info .info-content[data-v-ad34c109]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-ad34c109]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-ad34c109]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-ad34c109]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-ad34c109]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-ad34c109]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left}.chat-content .word-my .info .chat_img[data-v-ad34c109]{width:200px;height:200px;border-radius:5px}.chat-content .word-my .info .info-content[data-v-ad34c109]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}.demo-image__error .image-slot[data-v-ad34c109],.demo-image__error .image-slot .el-icon[data-v-ad34c109]{font-size:30px}.demo-image__error .el-image[data-v-ad34c109]{width:100%;height:200px}.chat-content[data-v-e529325a]{width:100%;padding:20px}.chat-content .word[data-v-e529325a]{display:flex;margin-bottom:20px}.chat-content .word img[data-v-e529325a]{width:40px;height:40px;border-radius:50%}.chat-content .word .info[data-v-e529325a]{margin-left:10px}.chat-content .word .info .time[data-v-e529325a]{font-size:12px;color:#333c;margin:-5px 0 0;height:20px;line-height:20px}.chat-content .word .info .info-content[data-v-e529325a]{max-width:80%;padding:10px;font-size:14px;background:#fff;position:relative;margin-top:8px;display:inline-block}.chat-content .word .info .info-content[data-v-e529325a]:before{position:absolute;left:-8px;top:8px;content:"";border-right:10px solid #FFF;border-top:8px solid transparent;border-bottom:8px solid transparent}.chat-content .word-my[data-v-e529325a]{display:flex;justify-content:flex-end;margin-bottom:20px}.chat-content .word-my img[data-v-e529325a]{width:40px;height:40px;border-radius:50%}.chat-content .word-my .info[data-v-e529325a]{width:90%;margin-left:10px;text-align:right}.chat-content .word-my .info .time[data-v-e529325a]{font-size:12px;color:#333c;margin:-5px 10px 0 0;height:20px;line-height:20px}.chat-content .word-my .info .info-content[data-v-e529325a]{max-width:80%;padding:10px;font-size:14px;float:right;margin-right:10px;position:relative;margin-top:8px;background:#95ec69;text-align:left;display:inline-block}.chat-content .word-my .info .info-content[data-v-e529325a]:after{position:absolute;right:-8px;top:8px;content:"";border-left:10px solid #95EC69;border-top:8px solid transparent;border-bottom:8px solid transparent}#chat[data-v-49e80cb1]{position:relative;width:100%;height:100%;background-color:#f5f5f5;display:flex;flex-direction:column}#chat[data-v-49e80cb1] .chat_body[data-v-49e80cb1]{flex:1;overflow-y:hidden;overflow-x:hidden}#chat[data-v-49e80cb1] .chat_body[data-v-49e80cb1] .chat_window[data-v-49e80cb1]{height:100%;overflow-y:scroll;width:calc(100% + 17px);padding:0;margin:0}#chat[data-v-49e80cb1] .chat_body[data-v-49e80cb1] .chat_window[data-v-49e80cb1]>.message[data-v-49e80cb1]:last-of-type{margin-bottom:8px}
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/ChatView-zX7v9ucw.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/ChatView-PSmCcQTu.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,424 +1,437 @@
 import {
-    d as j,
+    d as M,
     r as m,
-    o as Z,
-    a as k,
-    b as l,
-    c as u,
+    o as Y,
+    a as x,
+    b as o,
+    c,
     e,
-    f as a,
-    w as de,
-    g as o,
-    h as c,
-    i as E,
-    t as x,
-    j as R,
-    F as K,
-    E as ae,
-    _ as L,
-    u as F,
-    k as se,
-    l as ue,
-    m as J,
-    n as X,
-    p as G,
-    q as W,
+    f as n,
+    w as te,
+    g as _,
+    h,
+    i as U,
+    t as k,
+    j as E,
+    F as G,
+    E as J,
+    _ as O,
+    u as L,
+    k as X,
+    l as le,
+    m as I,
+    n as Z,
+    p as A,
+    q as N,
     s as ne,
     v as B,
-    x as _e,
-    y as A,
-    z as Y
-} from "./index-CtkzF4da.js";
+    x as F,
+    y as K,
+    z as oe
+} from "./index-VdcdRmrH.js";
 import {
-    h as O
+    h as T
 } from "./axios--FnjuHWf.js"; /* empty css                                                                       */
 import {
-    _ as he
-} from "./HomeView.vue_vue_type_script_setup_true_lang-5w2dEJdv.js";
-const me = {
+    _ as se
+} from "./HomeView.vue_vue_type_script_setup_true_lang-dZI7DIut.js";
+const ae = {
         style: {
             padding: "10px 10px"
         }
     },
-    fe = {
+    ie = {
         key: 0
     },
-    pe = {
+    re = {
         key: 1
     },
-    ve = e("br", null, null, -1),
-    ye = {
+    ce = e("br", null, null, -1),
+    de = {
         key: 2,
         style: {
             color: "#909399",
             "font-size": "12px"
         }
     },
-    we = j({
+    ue = M({
         __name: "ContactsList",
         emits: ["wxid"],
         setup(t, {
-            emit: v
+            emit: i
         }) {
-            const i = m([]),
-                r = async () => {
+            const l = m([]),
+                a = async () => {
                     try {
-                        return await O.post("/api/recent_user_list", {})
-                    } catch (w) {
-                        return console.error("Error fetching data:", w), []
+                        return await T.post("/api/recent_user_list", {})
+                    } catch (d) {
+                        return console.error("Error fetching data:", d), []
                     }
-                }, h = async (w = "") => {
+                }, s = async (d = "") => {
                     try {
-                        return await O.post("/api/user_list", {
-                            word: w
+                        return await T.post("/api/user_list", {
+                            word: d
                         })
-                    } catch (D) {
-                        return console.error("Error fetching data:", D), []
+                    } catch (g) {
+                        return console.error("Error fetching data:", g), []
                     }
                 };
-            Z(async () => {
+            Y(async () => {
                 try {
-                    i.value = await r()
-                } catch (w) {
-                    return console.error("Error fetching data:", w), []
+                    l.value = await a()
+                } catch (d) {
+                    return console.error("Error fetching data:", d), []
                 }
             });
-            const _ = m(""),
-                s = async () => {
+            const p = m(""),
+                u = async () => {
                     try {
-                        if (_.value === "") {
-                            i.value = await r();
+                        if (p.value === "") {
+                            l.value = await a();
                             return
                         }
-                        i.value = await h(_.value)
-                    } catch (w) {
-                        return console.error("Error fetching data:", w), []
+                        l.value = await s(p.value)
+                    } catch (d) {
+                        return console.error("Error fetching data:", d), []
                     }
-                }, d = v, b = w => {
-                    w !== void 0 && d("wxid", w.wxid)
+                }, v = i, w = d => {
+                    d !== void 0 && v("wxid", d.wxid)
                 };
-            return (w, D) => {
-                const z = k("el-input"),
-                    p = k("el-button"),
-                    U = k("el-avatar"),
-                    H = k("el-table-column"),
-                    I = k("el-table");
-                return l(), u("div", null, [e("div", me, [a(z, {
+            return (d, g) => {
+                const D = x("el-input"),
+                    y = x("el-button"),
+                    q = x("el-avatar"),
+                    j = x("el-table-column"),
+                    H = x("el-table");
+                return o(), c("div", null, [e("div", ae, [n(D, {
                     placeholder: "请输入关键字",
-                    modelValue: _.value,
-                    "onUpdate:modelValue": D[0] || (D[0] = S => _.value = S),
-                    onKeyup: de(s, ["enter"]),
+                    modelValue: p.value,
+                    "onUpdate:modelValue": g[0] || (g[0] = V => p.value = V),
+                    onKeyup: te(u, ["enter"]),
                     style: {
                         width: "170px",
                         "margin-left": "15px"
                     }
-                }, null, 8, ["modelValue"]), a(p, {
+                }, null, 8, ["modelValue"]), n(y, {
                     type: "primary",
-                    onClick: s,
+                    onClick: u,
                     style: {
                         width: "50px"
                     }
                 }, {
-                    default: o(() => [c("搜索")]),
+                    default: _(() => [h("搜索")]),
                     _: 1
-                })]), a(I, {
-                    data: i.value,
+                })]), n(H, {
+                    data: l.value,
                     stripe: "",
                     style: {
                         width: "100%"
                     },
                     "max-height": "100%",
                     height: "100%",
                     "highlight-current-row": "",
-                    onCurrentChange: b
+                    onCurrentChange: w
                 }, {
-                    default: o(() => [a(H, {
+                    default: _(() => [n(j, {
                         width: "57"
                     }, {
-                        default: o(({
-                            row: S
-                        }) => [S.headImgUrl !== "" ? (l(), E(U, {
+                        default: _(({
+                            row: V
+                        }) => [V.headImgUrl !== "" ? (o(), U(q, {
                             key: 0,
                             size: 33,
-                            src: "/api/imgsrc/" + S.headImgUrl
-                        }, null, 8, ["src"])) : (l(), E(U, {
+                            src: "/api/imgsrc/" + V.headImgUrl
+                        }, null, 8, ["src"])) : (o(), U(q, {
                             key: 1,
                             size: 33
                         }, {
-                            default: o(() => [c(" 群聊 ")]),
+                            default: _(() => [h(" 群聊 ")]),
                             _: 1
                         }))]),
                         _: 1
-                    }), a(H, {
+                    }), n(j, {
                         width: "190"
                     }, {
-                        default: o(({
-                            row: S
-                        }) => [S.remark !== null && S.remark !== "" ? (l(), u("span", fe, x(S.remark), 1)) : (l(), u("span", pe, x(S.nickname), 1)), ve, S.LastReadedCreateTime !== void 0 && S.LastReadedCreateTime !== null ? (l(), u("span", ye, x(S.LastReadedCreateTime), 1)) : R("", !0)]),
+                        default: _(({
+                            row: V
+                        }) => [V.remark !== null && V.remark !== "" ? (o(), c("span", ie, k(V.remark), 1)) : (o(), c("span", re, k(V.nickname), 1)), ce, V.LastReadedCreateTime !== void 0 && V.LastReadedCreateTime !== null ? (o(), c("span", de, k(V.LastReadedCreateTime), 1)) : E("", !0)]),
                         _: 1
                     })]),
                     _: 1
                 }, 8, ["data"])])
             }
         }
     }),
-    ge = j({
+    _e = M({
         __name: "ChatRecprdsHeader",
         props: {
             userData: {
                 type: Object,
                 required: !0
             }
         },
         emits: ["exporting"],
         setup(t, {
-            emit: v
+            emit: i
         }) {
-            const i = m(!1),
-                r = async () => {
-                    if (i.value) {
+            const l = m(!1),
+                a = async () => {
+                    if (l.value) {
                         console.log("正在获取实时消息，请稍后再试!");
                         return
                     }
-                    i.value = !0;
+                    l.value = !0;
                     try {
-                        const _ = await O.post("/api/realtimemsg", {});
-                        return i.value = !1, ae({
+                        const v = await T.post("/api/realtimemsg", {});
+                        return l.value = !1, J({
                             title: "Success",
                             message: "获取实时消息成功!",
                             type: "success"
-                        }), _
-                    } catch (_) {
-                        return i.value = !1, ae({
+                        }), v
+                    } catch (v) {
+                        return l.value = !1, J({
                             title: "Error",
                             message: "获取实时消息失败!",
                             type: "error"
-                        }), console.error("Error fetching data:", _), []
+                        }), console.error("Error fetching data:", v), []
                     }
-                }, h = v, $ = () => {
-                    h("exporting", !0)
+                }, s = m(!1), r = i, p = () => {
+                    r("exporting", !0), s.value = !0
+                }, u = () => {
+                    r("exporting", !1), s.value = !1
                 };
-            return (_, s) => {
-                const d = k("el-text"),
-                    b = k("el-col"),
-                    w = k("el-row");
-                return l(), u(K, null, [a(w, {
+            return (v, w) => {
+                const d = x("el-text"),
+                    g = x("el-col"),
+                    D = x("el-row");
+                return o(), c(G, null, [n(D, {
                     gutter: 5,
                     style: {
                         width: "100%"
                     }
                 }, {
-                    default: o(() => [a(b, {
+                    default: _(() => [n(g, {
                         span: 6,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "label_color mx-1",
                             truncated: ""
                         }, {
-                            default: o(() => [c("wxid:")]),
+                            default: _(() => [h("wxid:")]),
                             _: 1
-                        }), c("  "), a(d, {
+                        }), h("  "), n(d, {
                             class: "data_color mx-1",
                             truncated: "",
                             title: t.userData.wxid
                         }, {
-                            default: o(() => [c(x(t.userData.wxid), 1)]),
+                            default: _(() => [h(k(t.userData.wxid), 1)]),
                             _: 1
                         }, 8, ["title"])]),
                         _: 1
-                    }), a(b, {
+                    }), n(g, {
                         span: 6,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "label_color mx-1",
                             truncated: ""
                         }, {
-                            default: o(() => [c("账号:")]),
+                            default: _(() => [h("账号:")]),
                             _: 1
-                        }), c("  "), a(d, {
+                        }), h("  "), n(d, {
                             class: "data_color mx-1",
                             truncated: "",
                             title: t.userData.account
                         }, {
-                            default: o(() => [c(x(t.userData.account), 1)]),
+                            default: _(() => [h(k(t.userData.account), 1)]),
                             _: 1
                         }, 8, ["title"])]),
                         _: 1
-                    }), a(b, {
+                    }), n(g, {
                         span: 6,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "label_color mx-1",
                             truncated: ""
                         }, {
-                            default: o(() => [c("昵称:")]),
+                            default: _(() => [h("昵称:")]),
                             _: 1
-                        }), c("  "), a(d, {
+                        }), h("  "), n(d, {
                             class: "data_color mx-1",
                             truncated: "",
                             title: t.userData.nickname
                         }, {
-                            default: o(() => [c(x(t.userData.nickname), 1)]),
+                            default: _(() => [h(k(t.userData.nickname), 1)]),
                             _: 1
                         }, 8, ["title"])]),
                         _: 1
-                    }), a(b, {
+                    }), n(g, {
                         span: 6,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "label_color mx-1",
                             truncated: ""
                         }, {
-                            default: o(() => [c("备注:")]),
+                            default: _(() => [h("备注:")]),
                             _: 1
-                        }), c("  "), a(d, {
+                        }), h("  "), n(d, {
                             class: "data_color mx-1",
                             truncated: "",
                             title: t.userData.remark
                         }, {
-                            default: o(() => [c(x(t.userData.remark), 1)]),
+                            default: _(() => [h(k(t.userData.remark), 1)]),
                             _: 1
                         }, 8, ["title"])]),
                         _: 1
                     })]),
                     _: 1
-                }), a(w, {
+                }), n(D, {
                     gutter: 5,
                     style: {
                         width: "100%"
                     }
                 }, {
-                    default: o(() => [a(b, {
+                    default: _(() => [n(g, {
                         span: 3,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "label_color mx-1",
                             truncated: ""
                         }, {
-                            default: o(() => [c("数量:")]),
+                            default: _(() => [h("数量:")]),
                             _: 1
-                        }), c("  "), a(d, {
+                        }), h("  "), n(d, {
                             class: "data_color mx-1",
                             truncated: "",
                             title: t.userData.msg_count
                         }, {
-                            default: o(() => [c(x(t.userData.msg_count), 1)]),
+                            default: _(() => [h(k(t.userData.msg_count), 1)]),
                             _: 1
                         }, 8, ["title"])]),
                         _: 1
-                    }), a(b, {
+                    }), n(g, {
                         span: 15,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "label_color mx-1",
                             truncated: ""
                         }, {
-                            default: o(() => [c("描述:")]),
+                            default: _(() => [h("描述:")]),
                             _: 1
-                        }), c("  "), a(d, {
+                        }), h("  "), n(d, {
                             class: "data_color mx-1",
                             truncated: "",
                             title: t.userData.describe
                         }, {
-                            default: o(() => [c(x(t.userData.describe), 1)]),
+                            default: _(() => [h(k(t.userData.describe), 1)]),
                             _: 1
                         }, 8, ["title"])]),
                         _: 1
-                    }), a(b, {
+                    }), n(g, {
                         span: 3,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [n(d, {
                             class: "button_color mx-1 underline",
                             truncated: "",
-                            onClick: s[0] || (s[0] = D => {
-                                r()
+                            onClick: w[0] || (w[0] = y => {
+                                a()
                             })
                         }, {
-                            default: o(() => [c("实时消息 "), i.value ? (l(), u(K, {
+                            default: _(() => [h("实时消息 "), l.value ? (o(), c(G, {
                                 key: 0
-                            }, [c("(获取中)")], 64)) : R("", !0)]),
+                            }, [h("(获取中)")], 64)) : E("", !0)]),
                             _: 1
                         })]),
                         _: 1
-                    }), a(b, {
+                    }), n(g, {
                         span: 3,
                         style: {
                             "white-space": "nowrap"
                         }
                     }, {
-                        default: o(() => [a(d, {
+                        default: _(() => [s.value ? E("", !0) : (o(), U(d, {
+                            key: 0,
                             class: "button_color mx-1 underline",
                             truncated: "",
-                            onClick: s[1] || (s[1] = D => {
-                                $()
+                            onClick: w[1] || (w[1] = y => {
+                                p()
                             })
                         }, {
-                            default: o(() => [c("导出")]),
+                            default: _(() => [h("导出备份")]),
                             _: 1
-                        })]),
+                        })), s.value ? (o(), U(d, {
+                            key: 1,
+                            class: "button_color mx-1 underline",
+                            truncated: "",
+                            onClick: w[2] || (w[2] = y => {
+                                u()
+                            })
+                        }, {
+                            default: _(() => [h("聊天查看")]),
+                            _: 1
+                        })) : E("", !0)]),
                         _: 1
                     })]),
                     _: 1
                 })], 64)
             }
         }
     }),
-    xe = L(ge, [
-        ["__scopeId", "data-v-7bc26671"]
+    pe = O(_e, [
+        ["__scopeId", "data-v-0c9eea5d"]
     ]),
-    be = {
+    ve = {
         class: "chat-content"
     },
-    ke = {
+    he = {
         key: 0,
         class: "word"
     },
-    $e = ["src"],
-    Se = {
+    me = ["src"],
+    fe = {
         class: "info"
     },
-    De = {
+    ye = {
         class: "time"
     },
-    Te = ["innerHTML"],
-    Ue = {
+    xe = ["innerHTML"],
+    we = {
         key: 1,
         class: "word-my"
     },
-    Me = {
+    ge = {
         class: "info"
     },
-    Ve = {
+    be = {
         class: "time"
     },
-    Ce = ["innerHTML"],
-    Ee = ["src"],
-    ze = j({
+    $e = ["innerHTML"],
+    ke = ["src"],
+    Se = M({
         __name: "MessageText",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             content: {
@@ -431,63 +444,63 @@
             },
             direction: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            const v = i => (i = i.replace(/\n/g, "<br>"), new DOMParser().parseFromString(i, "text/html").body.innerHTML);
-            return (i, r) => (l(), u("div", be, [t.is_sender ? (l(), u("div", Ue, [e("div", Me, [e("p", Ve, x(t.direction), 1), e("div", {
+            const i = l => (l = l.replace(/\n/g, "<br>"), new DOMParser().parseFromString(l, "text/html").body.innerHTML);
+            return (l, a) => (o(), c("div", ve, [t.is_sender ? (o(), c("div", we, [e("div", ge, [e("p", be, k(t.direction), 1), e("div", {
                 class: "info-content",
-                innerHTML: v(t.content)
-            }, null, 8, Ce)]), e("img", {
+                innerHTML: i(t.content)
+            }, null, 8, $e)]), e("img", {
                 src: t.headUrl
-            }, null, 8, Ee)])) : (l(), u("div", ke, [e("img", {
+            }, null, 8, ke)])) : (o(), c("div", he, [e("img", {
                 src: t.headUrl
-            }, null, 8, $e), e("div", Se, [e("p", De, x(t.direction), 1), e("div", {
+            }, null, 8, me), e("div", fe, [e("p", ye, k(t.direction), 1), e("div", {
                 class: "info-content",
-                innerHTML: v(t.content)
-            }, null, 8, Te)])]))]))
+                innerHTML: i(t.content)
+            }, null, 8, xe)])]))]))
         }
     }),
-    He = L(ze, [
+    Ve = O(Se, [
         ["__scopeId", "data-v-d930be9e"]
     ]),
-    Ie = {
+    Ue = {
         class: "chat-content"
     },
-    Re = {
+    Me = {
         key: 0,
         class: "word"
     },
-    je = ["src"],
-    Oe = {
+    Ee = ["src"],
+    Ce = {
         class: "info"
     },
-    qe = {
+    Te = {
         class: "time"
     },
-    Le = {
+    De = {
         class: "demo-image__preview"
     },
-    Pe = {
+    qe = {
         key: 1,
         class: "word-my"
     },
-    Fe = {
+    ze = {
         class: "info"
     },
-    Ne = {
+    Re = {
         class: "time"
     },
-    Be = {
+    je = {
         class: "demo-image__preview"
     },
-    Ae = ["src"],
-    Ye = j({
+    He = ["src"],
+    Ie = M({
         __name: "MessageImg",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             content: {
@@ -504,33 +517,33 @@
             },
             src: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            return (v, i) => {
-                const r = k("el-image");
-                return l(), u("div", Ie, [t.is_sender ? (l(), u("div", Pe, [e("div", Fe, [e("p", Ne, x(t.direction), 1), e("div", Be, [a(r, {
+            return (i, l) => {
+                const a = x("el-image");
+                return o(), c("div", Ue, [t.is_sender ? (o(), c("div", qe, [e("div", ze, [e("p", Re, k(t.direction), 1), e("div", je, [n(a, {
                     style: {
                         "max-width": "150px",
                         "max-height": "150px"
                     },
                     src: t.src,
                     "zoom-rate": 1.2,
                     "max-scale": 7,
                     "min-scale": .2,
                     "preview-src-list": [t.src],
                     "initial-index": 4,
                     fit: "cover"
                 }, null, 8, ["src", "preview-src-list"])])]), e("img", {
                     src: t.headUrl
-                }, null, 8, Ae)])) : (l(), u("div", Re, [e("img", {
+                }, null, 8, He)])) : (o(), c("div", Me, [e("img", {
                     src: t.headUrl
-                }, null, 8, je), e("div", Oe, [e("p", qe, x(t.direction), 1), e("div", Le, [a(r, {
+                }, null, 8, Ee), e("div", Ce, [e("p", Te, k(t.direction), 1), e("div", De, [n(a, {
                     style: {
                         "max-width": "150px",
                         "max-height": "150px"
                     },
                     src: t.src,
                     "zoom-rate": 1.2,
                     "max-scale": 7,
@@ -538,59 +551,59 @@
                     "preview-src-list": [t.src],
                     "initial-index": 4,
                     fit: "cover"
                 }, null, 8, ["src", "preview-src-list"])])])]))])
             }
         }
     }),
-    We = L(Ye, [
+    Oe = O(Ie, [
         ["__scopeId", "data-v-24d6aaa0"]
     ]),
-    Ge = {
+    Le = {
         class: "chat-content"
     },
-    Ke = {
+    Ne = {
         key: 0,
         class: "word"
     },
-    Je = ["src"],
-    Qe = {
+    Be = ["src"],
+    Fe = {
         class: "info"
     },
-    Xe = {
+    Ae = {
         class: "time"
     },
-    Ze = {
+    Pe = {
         class: "demo-video__preview"
     },
-    et = {
+    We = {
         controls: "",
         width: "30%"
     },
-    tt = ["src"],
-    at = {
+    Ke = ["src"],
+    Ge = {
         key: 1,
         class: "word-my"
     },
-    st = {
+    Ye = {
         class: "info"
     },
-    lt = {
+    Je = {
         class: "time"
     },
-    nt = {
+    Xe = {
         class: "demo-video__preview"
     },
-    ot = {
+    Qe = {
         controls: "",
         width: "50%"
     },
-    it = ["src"],
-    rt = ["src"],
-    ct = j({
+    Ze = ["src"],
+    et = ["src"],
+    tt = M({
         __name: "MessageVideo",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             content: {
@@ -607,70 +620,70 @@
             },
             src: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            return (v, i) => (l(), u("div", Ge, [t.is_sender ? (l(), u("div", at, [e("div", st, [e("p", lt, x(t.direction), 1), e("div", nt, [e("video", ot, [e("source", {
+            return (i, l) => (o(), c("div", Le, [t.is_sender ? (o(), c("div", Ge, [e("div", Ye, [e("p", Je, k(t.direction), 1), e("div", Xe, [e("video", Qe, [e("source", {
                 src: t.src,
                 type: "video/mp4"
-            }, null, 8, it)])])]), e("img", {
+            }, null, 8, Ze)])])]), e("img", {
                 src: t.headUrl
-            }, null, 8, rt)])) : (l(), u("div", Ke, [e("img", {
+            }, null, 8, et)])) : (o(), c("div", Ne, [e("img", {
                 src: t.headUrl
-            }, null, 8, Je), e("div", Qe, [e("p", Xe, x(t.direction), 1), e("div", Ze, [e("video", et, [e("source", {
+            }, null, 8, Be), e("div", Fe, [e("p", Ae, k(t.direction), 1), e("div", Pe, [e("video", We, [e("source", {
                 src: t.src,
                 type: "video/mp4"
-            }, null, 8, tt)])])])]))]))
+            }, null, 8, Ke)])])])]))]))
         }
     }),
-    dt = L(ct, [
+    lt = O(tt, [
         ["__scopeId", "data-v-5aa79515"]
     ]),
-    ut = {
+    nt = {
         class: "chat-content"
     },
-    _t = {
+    ot = {
         key: 0,
         class: "word"
     },
-    ht = ["src"],
-    mt = {
+    st = ["src"],
+    at = {
         class: "info"
     },
-    ft = {
+    it = {
         class: "time"
     },
-    pt = {
+    rt = {
         controls: "",
         style: {
             "background-color": "#fff"
         }
     },
-    vt = ["src"],
-    yt = {
+    ct = ["src"],
+    dt = {
         key: 1,
         class: "word-my"
     },
-    wt = {
+    ut = {
         class: "info"
     },
-    gt = {
+    _t = {
         class: "time"
     },
-    xt = {
+    pt = {
         controls: "",
         style: {
             "background-color": "#95EC69"
         }
     },
-    bt = ["src"],
-    kt = ["src"],
-    $t = j({
+    vt = ["src"],
+    ht = ["src"],
+    mt = M({
         __name: "MessageAudio",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             headUrl: {
@@ -687,82 +700,82 @@
             },
             msg: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            return (v, i) => (l(), u("div", ut, [t.is_sender ? (l(), u("div", yt, [e("div", wt, [e("p", gt, x(t.direction), 1), e("audio", xt, [e("source", {
+            return (i, l) => (o(), c("div", nt, [t.is_sender ? (o(), c("div", dt, [e("div", ut, [e("p", _t, k(t.direction), 1), e("audio", pt, [e("source", {
                 src: t.src,
                 type: "audio/wav"
-            }, null, 8, bt)]), a(F(se), {
+            }, null, 8, vt)]), n(L(X), {
                 rows: 1,
                 readonly: !0,
                 value: t.msg,
                 style: {
                     width: "100%"
                 }
             }, null, 8, ["value"])]), e("img", {
                 src: t.headUrl
-            }, null, 8, kt)])) : (l(), u("div", _t, [e("img", {
+            }, null, 8, ht)])) : (o(), c("div", ot, [e("img", {
                 src: t.headUrl
-            }, null, 8, ht), e("div", mt, [e("p", ft, x(t.direction), 1), e("audio", pt, [e("source", {
+            }, null, 8, st), e("div", at, [e("p", it, k(t.direction), 1), e("audio", rt, [e("source", {
                 src: t.src,
                 type: "audio/wav"
-            }, null, 8, vt)]), a(F(se), {
+            }, null, 8, ct)]), n(L(X), {
                 rows: 1,
                 readonly: !0,
                 value: t.msg,
                 style: {
                     width: "100%"
                 }
             }, null, 8, ["value"])])]))]))
         }
     }),
-    St = L($t, [
+    ft = O(mt, [
         ["__scopeId", "data-v-0d0f2cd4"]
     ]),
-    Dt = {
+    yt = {
         class: "chat-content"
     },
-    Tt = {
+    xt = {
         key: 0,
         class: "word"
     },
-    Ut = ["src"],
-    Mt = {
+    wt = ["src"],
+    gt = {
         class: "info"
     },
-    Vt = {
+    bt = {
         class: "time"
     },
-    Ct = {
+    $t = {
         style: {
             float: "left"
         }
     },
-    Et = ["href"],
-    zt = {
+    kt = ["href"],
+    St = {
         key: 1,
         class: "word-my"
     },
-    Ht = {
+    Vt = {
         class: "info"
     },
-    It = {
+    Ut = {
         class: "time"
     },
-    Rt = {
+    Mt = {
         style: {
             float: "right"
         }
     },
-    jt = ["href"],
-    Ot = ["src"],
-    qt = j({
+    Et = ["href"],
+    Ct = ["src"],
+    Tt = M({
         __name: "MessageFile",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             content: {
@@ -779,102 +792,102 @@
             },
             src: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            const v = t,
-                i = m(""),
-                r = ue({
+            const i = t,
+                l = m(""),
+                a = le({
                     file_name: String,
                     file_size: Number,
                     file_size_unit: String
                 });
-            Z(async () => {
+            Y(async () => {
                 console.log("文件加载中");
-                const $ = await h(v.src);
-                r.file_name = $.file_name, r.file_size = Number($.file_size) / 1024, r.file_size < 1024 ? r.file_size_unit = "kb" : (r.file_size = r.file_size / 1024, r.file_size_unit = "mb"), r.file_size = Number($.file_size) / 1024, i.value = `/api/file/${v.src}`
+                const r = await s(i.src);
+                a.file_name = r.file_name, a.file_size = Number(r.file_size) / 1024, a.file_size < 1024 ? a.file_size_unit = "kb" : (a.file_size = a.file_size / 1024, a.file_size_unit = "mb"), a.file_size = Number(r.file_size) / 1024, l.value = `/api/file/${i.src}`
             });
-            const h = async $ => {
+            const s = async r => {
                 try {
-                    return await O.post("/api/file_info", {
-                        file_path: $
+                    return await T.post("/api/file_info", {
+                        file_path: r
                     })
-                } catch (_) {
-                    return console.error("Error fetching file_info:", _), ""
+                } catch (p) {
+                    return console.error("Error fetching file_info:", p), ""
                 }
             };
-            return ($, _) => {
-                const s = k("el-card");
-                return l(), u("div", Dt, [t.is_sender ? (l(), u("div", zt, [e("div", Ht, [e("p", It, x(t.direction), 1), e("div", Rt, [a(s, {
+            return (r, p) => {
+                const u = x("el-card");
+                return o(), c("div", yt, [t.is_sender ? (o(), c("div", St, [e("div", Vt, [e("p", Ut, k(t.direction), 1), e("div", Mt, [n(u, {
                     shadow: "hover",
                     style: {
                         width: "fit-content"
                     }
                 }, {
-                    default: o(() => [c("文件 ： "), e("a", {
-                        href: i.value,
+                    default: _(() => [h("文件 ： "), e("a", {
+                        href: l.value,
                         download: ""
-                    }, x(r.file_name), 9, jt), e("div", null, [c(" 文件大小："), e("span", null, x(r.file_size) + x(r.file_size_unit), 1)])]),
+                    }, k(a.file_name), 9, Et), e("div", null, [h(" 文件大小："), e("span", null, k(a.file_size) + k(a.file_size_unit), 1)])]),
                     _: 1
                 })])]), e("img", {
                     src: t.headUrl
-                }, null, 8, Ot)])) : (l(), u("div", Tt, [e("img", {
+                }, null, 8, Ct)])) : (o(), c("div", xt, [e("img", {
                     src: t.headUrl
-                }, null, 8, Ut), e("div", Mt, [e("p", Vt, x(t.direction), 1), e("div", Ct, [a(s, {
+                }, null, 8, wt), e("div", gt, [e("p", bt, k(t.direction), 1), e("div", $t, [n(u, {
                     shadow: "hover",
                     style: {
                         width: "fit-content"
                     }
                 }, {
-                    default: o(() => [c("文件 ： "), e("a", {
-                        href: i.value,
+                    default: _(() => [h("文件 ： "), e("a", {
+                        href: l.value,
                         download: ""
-                    }, x(r.file_name), 9, Et), e("div", null, [c(" 文件大小："), e("span", null, x(r.file_size) + x(r.file_size_unit), 1)])]),
+                    }, k(a.file_name), 9, kt), e("div", null, [h(" 文件大小："), e("span", null, k(a.file_size) + k(a.file_size_unit), 1)])]),
                     _: 1
                 })])])]))])
             }
         }
     }),
-    Lt = L(qt, [
+    Dt = O(Tt, [
         ["__scopeId", "data-v-e797f204"]
     ]),
-    Pt = {
+    qt = {
         class: "chat-content"
     },
-    Ft = {
+    zt = {
         key: 0,
         class: "word"
     },
-    Nt = ["src"],
-    Bt = {
+    Rt = ["src"],
+    jt = {
         class: "info"
     },
-    At = {
+    Ht = {
         class: "time"
     },
-    Yt = {
+    It = {
         class: "demo-image__preview"
     },
-    Wt = {
+    Ot = {
         key: 1,
         class: "word-my"
     },
-    Gt = {
+    Lt = {
         class: "info"
     },
-    Kt = {
+    Nt = {
         class: "time"
     },
-    Jt = {
+    Bt = {
         class: "demo-image__preview"
     },
-    Qt = ["src"],
-    Xt = j({
+    Ft = ["src"],
+    At = M({
         __name: "MessageEmoji",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             content: {
@@ -891,33 +904,33 @@
             },
             src: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            return (v, i) => {
-                const r = k("el-image");
-                return l(), u("div", Pt, [t.is_sender ? (l(), u("div", Wt, [e("div", Gt, [e("p", Kt, x(t.direction), 1), e("div", Jt, [a(r, {
+            return (i, l) => {
+                const a = x("el-image");
+                return o(), c("div", qt, [t.is_sender ? (o(), c("div", Ot, [e("div", Lt, [e("p", Nt, k(t.direction), 1), e("div", Bt, [n(a, {
                     style: {
                         "max-width": "150px",
                         "max-height": "150px"
                     },
                     src: t.src,
                     "zoom-rate": 1.2,
                     "max-scale": 7,
                     "min-scale": .2,
                     "preview-src-list": [t.src],
                     "initial-index": 4,
                     fit: "cover"
                 }, null, 8, ["src", "preview-src-list"])])]), e("img", {
                     src: t.headUrl
-                }, null, 8, Qt)])) : (l(), u("div", Ft, [e("img", {
+                }, null, 8, Ft)])) : (o(), c("div", zt, [e("img", {
                     src: t.headUrl
-                }, null, 8, Nt), e("div", Bt, [e("p", At, x(t.direction), 1), e("div", Yt, [a(r, {
+                }, null, 8, Rt), e("div", jt, [e("p", Ht, k(t.direction), 1), e("div", It, [n(a, {
                     style: {
                         "max-width": "150px",
                         "max-height": "150px"
                     },
                     src: t.src,
                     "zoom-rate": 1.2,
                     "max-scale": 7,
@@ -925,45 +938,45 @@
                     "preview-src-list": [t.src],
                     "initial-index": 4,
                     fit: "cover"
                 }, null, 8, ["src", "preview-src-list"])])])]))])
             }
         }
     }),
-    Zt = L(Xt, [
+    Pt = O(At, [
         ["__scopeId", "data-v-ad34c109"]
     ]),
-    ea = {
+    Wt = {
         class: "chat-content"
     },
-    ta = {
+    Kt = {
         key: 0,
         class: "word"
     },
-    aa = ["src"],
-    sa = {
+    Gt = ["src"],
+    Yt = {
         class: "info"
     },
-    la = {
+    Jt = {
         class: "time"
     },
-    na = ["innerHTML"],
-    oa = {
+    Xt = ["innerHTML"],
+    Qt = {
         key: 1,
         class: "word-my"
     },
-    ia = {
+    Zt = {
         class: "info"
     },
-    ra = {
+    el = {
         class: "time"
     },
-    ca = ["innerHTML"],
-    da = ["src"],
-    ua = j({
+    tl = ["innerHTML"],
+    ll = ["src"],
+    nl = M({
         __name: "MessageOther",
         props: {
             is_sender: {
                 type: Number,
                 default: 0
             },
             content: {
@@ -976,52 +989,52 @@
             },
             direction: {
                 type: String,
                 default: ""
             }
         },
         setup(t) {
-            const v = i => (i = i.replace(/\n/g, "<br>"), new DOMParser().parseFromString(i, "text/html").body.innerHTML);
-            return (i, r) => (l(), u("div", ea, [t.is_sender ? (l(), u("div", oa, [e("div", ia, [e("p", ra, x(t.direction), 1), e("div", {
+            const i = l => (l = l.replace(/\n/g, "<br>"), new DOMParser().parseFromString(l, "text/html").body.innerHTML);
+            return (l, a) => (o(), c("div", Wt, [t.is_sender ? (o(), c("div", Qt, [e("div", Zt, [e("p", el, k(t.direction), 1), e("div", {
                 class: "info-content",
-                innerHTML: v(t.content)
-            }, null, 8, ca)]), e("img", {
+                innerHTML: i(t.content)
+            }, null, 8, tl)]), e("img", {
                 src: t.headUrl
-            }, null, 8, da)])) : (l(), u("div", ta, [e("img", {
+            }, null, 8, ll)])) : (o(), c("div", Kt, [e("img", {
                 src: t.headUrl
-            }, null, 8, aa), e("div", sa, [e("p", la, x(t.direction), 1), e("div", {
+            }, null, 8, Gt), e("div", Yt, [e("p", Jt, k(t.direction), 1), e("div", {
                 class: "info-content",
-                innerHTML: v(t.content)
-            }, null, 8, na)])]))]))
+                innerHTML: i(t.content)
+            }, null, 8, Xt)])]))]))
         }
     }),
-    _a = L(ua, [
+    ol = O(nl, [
         ["__scopeId", "data-v-e529325a"]
     ]),
-    ha = {
+    sl = {
         id: "chat"
     },
-    ma = {
+    al = {
         class: "chat_body"
     },
-    fa = {
+    il = {
         class: "chat_window",
         ref: "chatWindow"
     },
-    pa = {
+    rl = {
         key: 0,
         class: "load_more",
         style: {
             display: "flex",
             "justify-content": "center",
             "margin-top": "10px",
             "margin-bottom": "10px"
         }
     },
-    va = j({
+    cl = M({
         __name: "ChatRecordsMain",
         props: {
             userData: {
                 type: Object,
                 required: !0
             },
             setScrollTop: {
@@ -1030,254 +1043,532 @@
             },
             updateScrollTop: {
                 type: Function,
                 required: !0
             }
         },
         setup(t, {
-            expose: v
+            expose: i
         }) {
-            const i = t,
-                r = m([]),
-                h = m({}),
-                $ = m(!1),
-                _ = m(""),
-                s = m(0),
-                d = m(100),
-                b = m(0),
-                w = m(!1),
-                D = async (g, V, T) => {
-                    if ($.value) {
+            const l = t,
+                a = m([]),
+                s = m({}),
+                r = m(!1),
+                p = m(""),
+                u = m(0),
+                v = m(100),
+                w = m(0),
+                d = m(!1),
+                g = async ($, z, C) => {
+                    if (r.value) {
                         console.log("正在获取消息，请稍后再试!");
                         return
                     }
-                    if (T == "") {
+                    if (C == "") {
                         console.log("wxid 为空, 请检查!");
                         return
                     }
                     try {
-                        $.value = !0, g < 0 && (g = 0);
-                        const n = await O.post("/api/msgs", {
-                            start: g,
-                            limit: V,
-                            wxid: T
+                        r.value = !0, $ < 0 && ($ = 0);
+                        const f = await T.post("/api/msgs", {
+                            start: $,
+                            limit: z,
+                            wxid: C
                         });
-                        return r.value = n.msg_list, h.value = Object.assign(h.value, n.user_list), $.value = !1, n
-                    } catch (n) {
-                        return $.value = !1, console.error("Error fetching data:", n), []
+                        return a.value = f.msg_list, s.value = Object.assign(s.value, f.user_list), r.value = !1, f
+                    } catch (f) {
+                        return r.value = !1, console.error("Error fetching data:", f), []
                     }
-                }, z = async g => {
+                }, D = async $ => {
                     try {
-                        return (await O.post("/api/msg_count", {
-                            wxid: g
-                        }))[g]
-                    } catch (V) {
-                        return console.error("Error fetching data msg_count:", V), []
+                        return (await T.post("/api/msg_count", {
+                            wxid: $
+                        }))[$]
+                    } catch (z) {
+                        return console.error("Error fetching data msg_count:", z), []
                     }
-                }, p = async () => {
+                }, y = async () => {
                     try {
-                        return (await O.get("/api/mywxid")).my_wxid
-                    } catch (g) {
-                        return console.error("Error fetching data my_wxid:", g), []
+                        return (await T.get("/api/mywxid")).my_wxid
+                    } catch ($) {
+                        return console.error("Error fetching data my_wxid:", $), []
                     }
-                }, U = async () => {
+                }, q = async () => {
                     try {
-                        _.value = await p(), b.value = await z(i.userData.wxid), s.value = b.value - d.value, s.value < 0 && (s.value = 0), await D(s.value, d.value, i.userData.wxid), w.value || await G(() => {
-                            i.setScrollTop(), w.value = !1
+                        p.value = await y(), w.value = await D(l.userData.wxid), u.value = w.value - v.value, u.value < 0 && (u.value = 0), await g(u.value, v.value, l.userData.wxid), d.value || await A(() => {
+                            l.setScrollTop(), d.value = !1
                         })
-                    } catch (g) {
-                        return console.error("Error fetching data:", g), []
+                    } catch ($) {
+                        return console.error("Error fetching data:", $), []
                     }
                 };
-            J(() => i.userData.wxid, (g, V) => {
-                console.log("username changed： ", V, g), r.value = [], h.value = {}, w.value = !1, b.value = 0, s.value = 0, U()
+            I(() => l.userData.wxid, ($, z) => {
+                console.log("username changed： ", z, $), a.value = [], s.value = {}, d.value = !1, w.value = 0, u.value = 0, q()
             });
-            const H = async () => {
-                _.value = await p(), b.value = await z(i.userData.wxid);
-                let g = d.value,
-                    V = s.value - g;
-                const T = await D(V, g, i.userData.wxid);
-                s.value = V, console.log("loadMore", V, s.value, g, i.userData.wxid), r.value = T.msg_list.concat(r.value), r.value.sort((n, f) => n.id - f.id), r.value = r.value.filter((n, f, y) => f === 0 || n.id !== y[f - 1].id), h.value = Object.assign(h.value, T.user_list), await G(() => {
-                    i.updateScrollTop()
+            const j = async () => {
+                p.value = await y(), w.value = await D(l.userData.wxid);
+                let $ = v.value,
+                    z = u.value - $;
+                z < 0 && (z = 0);
+                const C = await g(z, $, l.userData.wxid);
+                u.value = z, console.log("loadMore", z, u.value, $, l.userData.wxid), a.value = C.msg_list.concat(a.value), a.value.sort((f, S) => f.id - S.id), a.value = a.value.filter((f, S, b) => S === 0 || f.id !== b[S - 1].id), s.value = Object.assign(s.value, C.user_list), await A(() => {
+                    l.updateScrollTop()
                 })
             };
-            v({
-                loadMore: H
+            i({
+                loadMore: j
             });
-            const I = g => (g.talker == "我" && (g.talker = _.value), `${(T=>h.value.hasOwnProperty(T.talker)?h.value[T.talker].remark?h.value[T.talker].remark:h.value[T.talker].nickname?h.value[T.talker].nickname:h.value[T.talker].account?h.value[T.talker].account:T.talker:T.talker)(g)} [${g.type_name}] ${g.CreateTime}`),
-                S = g => (g.talker == "我" && (g.talker = _.value), h.value.hasOwnProperty(g.talker) ? "/api/imgsrc/" + h.value[g.talker].headImgUrl : "");
-            return (g, V) => {
-                const T = k("el-button");
-                return l(), u("div", ha, [e("div", ma, [e("div", fa, [r.value.length < b.value ? (l(), u("div", pa, [a(T, {
+            const H = $ => ($.talker == "我" && ($.talker = p.value), `${(C=>s.value.hasOwnProperty(C.talker)?s.value[C.talker].remark?s.value[C.talker].remark:s.value[C.talker].nickname?s.value[C.talker].nickname:s.value[C.talker].account?s.value[C.talker].account:C.talker:C.talker)($)} [${$.type_name}] ${$.CreateTime}`),
+                V = $ => ($.talker == "我" && ($.talker = p.value), s.value.hasOwnProperty($.talker) ? "/api/imgsrc/" + s.value[$.talker].headImgUrl : "");
+            return ($, z) => {
+                const C = x("el-button");
+                return o(), c("div", sl, [e("div", al, [e("div", il, [a.value.length < w.value ? (o(), c("div", rl, [n(C, {
                     type: "primary",
-                    onClick: H
+                    onClick: j
                 }, {
-                    default: o(() => [c("查看更多消息")]),
+                    default: _(() => [h("查看更多消息")]),
                     _: 1
-                })])) : R("", !0), (l(!0), u(K, null, X(r.value, (n, f) => (l(), u("div", {
+                })])) : E("", !0), (o(!0), c(G, null, Z(a.value, (f, S) => (o(), c("div", {
                     class: "message",
-                    key: f
-                }, [n.type_name == "文本" ? (l(), E(He, {
+                    key: S
+                }, [f.type_name == "文本" ? (o(), U(Ve, {
                     key: 0,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    content: n.content.msg
-                }, null, 8, ["is_sender", "direction", "headUrl", "content"])) : n.type_name == "图片" ? (l(), E(We, {
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    content: f.content.msg
+                }, null, 8, ["is_sender", "direction", "headUrl", "content"])) : f.type_name == "图片" ? (o(), U(Oe, {
                     key: 1,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    src: "/api/img/" + n.content.src
-                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : n.type_name == "动画表情" ? (l(), E(Zt, {
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    src: "/api/img/" + f.content.src
+                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : f.type_name == "动画表情" ? (o(), U(Pt, {
                     key: 2,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    src: "/api/imgsrc/" + n.content.src
-                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : n.type_name == "视频" ? (l(), E(dt, {
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    src: "/api/imgsrc/" + f.content.src
+                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : f.type_name == "视频" ? (o(), U(lt, {
                     key: 3,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    src: "/api/video/" + n.content.src
-                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : n.type_name == "文件" ? (l(), E(Lt, {
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    src: "/api/video/" + f.content.src
+                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : f.type_name == "文件" ? (o(), U(Dt, {
                     key: 4,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    src: n.content.src
-                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : n.type_name == "语音" ? (l(), E(St, {
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    src: f.content.src
+                }, null, 8, ["is_sender", "direction", "headUrl", "src"])) : f.type_name == "语音" ? (o(), U(ft, {
                     key: 5,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    src: "/api/" + n.content.src,
-                    msg: n.content.msg
-                }, null, 8, ["is_sender", "direction", "headUrl", "src", "msg"])) : (l(), E(_a, {
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    src: "/api/" + f.content.src,
+                    msg: f.content.msg
+                }, null, 8, ["is_sender", "direction", "headUrl", "src", "msg"])) : (o(), U(ol, {
                     key: 6,
-                    is_sender: n.is_sender,
-                    direction: I(n),
-                    headUrl: S(n),
-                    content: n.content.msg
+                    is_sender: f.is_sender,
+                    direction: H(f),
+                    headUrl: V(f),
+                    content: f.content.msg
                 }, null, 8, ["is_sender", "direction", "headUrl", "content"]))]))), 128))], 512)])])
             }
         }
     }),
-    ya = L(va, [
-        ["__scopeId", "data-v-09ca318b"]
+    dl = O(cl, [
+        ["__scopeId", "data-v-49e80cb1"]
     ]),
-    wa = j({
-        __name: "DateTimeSelect",
-        emits: ["datetime"],
-        setup(t, {
-            emit: v
-        }) {
-            const i = [new Date(2e3, 1, 1, 0, 0, 0), new Date(2e3, 2, 1, 23, 59, 59)],
-                r = [{
-                    text: "全部",
-                    value: () => {
-                        const _ = new Date;
-                        return [new Date(2010, 0, 1, 0, 0, 0), _]
-                    }
-                }, {
-                    text: "最近一周",
-                    value: () => {
-                        const _ = new Date,
-                            s = new Date;
-                        return s.setTime(s.getTime() - 3600 * 1e3 * 24 * 7), [s, _]
-                    }
-                }, {
-                    text: "最近一个月",
-                    value: () => {
-                        const _ = new Date,
-                            s = new Date;
-                        return s.setTime(s.getTime() - 3600 * 1e3 * 24 * 30), [s, _]
-                    }
-                }, {
-                    text: "最近三个月",
-                    value: () => {
-                        const _ = new Date,
-                            s = new Date;
-                        return s.setTime(s.getTime() - 3600 * 1e3 * 24 * 90), [s, _]
-                    }
-                }, {
-                    text: "最近半年",
-                    value: () => {
-                        const _ = new Date,
-                            s = new Date;
-                        return s.setTime(s.getTime() - 3600 * 1e3 * 24 * 180), [s, _]
-                    }
-                }, {
-                    text: "最近一年",
-                    value: () => {
-                        const _ = new Date,
-                            s = new Date;
-                        return s.setTime(s.getTime() - 3600 * 1e3 * 24 * 365), [s, _]
-                    }
-                }, {
-                    text: "去年一整年",
-                    value: () => {
-                        const _ = new Date;
-                        _.setFullYear(_.getFullYear() - 1), _.setMonth(0), _.setDate(1), _.setHours(0, 0, 0);
-                        const s = new Date;
-                        return s.setFullYear(s.getFullYear() - 1), s.setMonth(11), s.setDate(31), s.setHours(23, 59, 59), [_, s]
+    ul = e("br", null, null, -1),
+    _l = e("br", null, null, -1),
+    pl = {
+        style: {
+            position: "relative"
+        }
+    },
+    vl = M({
+        __name: "ExportENDB",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (r, p) => {
+                console.log(r)
+            });
+            const l = m(""),
+                a = m(""),
+                s = async () => {
+                    a.value = "请求中...";
+                    try {
+                        a.value = await T.post("/api/export_endb", {
+                            wx_path: l.value
+                        })
+                    } catch (r) {
+                        return console.error("Error fetching data msg_count:", r), a.value = `请求失败
+` + r, []
                     }
-                }],
-                h = m([Date, Date]),
-                $ = v;
-            return J(() => h.value, (_, s) => {
-                let d = _[0].getTime(),
-                    b = _[1].getTime();
-                $("datetime", [d, b])
-            }), (_, s) => {
-                const d = k("el-date-picker");
-                return l(), E(d, {
-                    modelValue: h.value,
-                    "onUpdate:modelValue": s[0] || (s[0] = b => h.value = b),
-                    type: "datetimerange",
-                    shortcuts: r,
-                    "range-separator": "至",
-                    "start-placeholder": "开始时间",
-                    "end-placeholder": "结束时间",
-                    "default-time": i,
-                    format: "YYYY-MM-DD HH:mm"
-                }, null, 8, ["modelValue"])
+                };
+            return (r, p) => {
+                const u = x("el-input"),
+                    v = x("el-button"),
+                    w = x("el-divider");
+                return o(), c("div", null, [h(" 微信文件夹路径(可选)： "), n(u, {
+                    placeholder: "微信文件夹路径[可为空,空表示使用默认的，无默认会报错](eg: C:\\****\\WeChat Files\\wxid_**** )",
+                    modelValue: l.value,
+                    "onUpdate:modelValue": p[0] || (p[0] = d => l.value = d),
+                    style: {
+                        width: "70%"
+                    }
+                }, null, 8, ["modelValue"]), ul, _l, e("div", pl, [n(v, {
+                    type: "primary",
+                    onClick: p[1] || (p[1] = d => s())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })]), n(w), n(u, {
+                    type: "textarea",
+                    rows: 6,
+                    readonly: "",
+                    placeholder: "",
+                    modelValue: a.value,
+                    "onUpdate:modelValue": p[2] || (p[2] = d => a.value = d),
+                    style: {
+                        width: "100%"
+                    }
+                }, null, 8, ["modelValue"])])
             }
         }
     }),
-    ga = L(wa, [
-        ["__scopeId", "data-v-320582f6"]
-    ]),
-    xa = {
+    hl = e("br", null, null, -1),
+    ml = e("br", null, null, -1),
+    fl = e("br", null, null, -1),
+    yl = e("br", null, null, -1),
+    xl = {
+        style: {
+            position: "relative"
+        }
+    },
+    wl = M({
+        __name: "ExportDEDB",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (p, u) => {
+                console.log(p)
+            });
+            const l = m(""),
+                a = m(""),
+                s = m(""),
+                r = async () => {
+                    s.value = "正在处理中...";
+                    try {
+                        s.value = await T.post("/api/export_dedb", {
+                            key: a.value,
+                            wx_path: l.value
+                        })
+                    } catch (p) {
+                        return console.error("Error fetching data msg_count:", p), s.value = `请求失败
+` + p, []
+                    }
+                };
+            return (p, u) => {
+                const v = x("el-input"),
+                    w = x("el-button"),
+                    d = x("el-divider");
+                return o(), c("div", null, [h(" 密钥(可选)： "), n(v, {
+                    placeholder: "密钥[可为空,空表示使用默认的，无默认会报错]",
+                    modelValue: a.value,
+                    "onUpdate:modelValue": u[0] || (u[0] = g => a.value = g),
+                    style: {
+                        width: "75%"
+                    }
+                }, null, 8, ["modelValue"]), hl, ml, h(" 微信文件夹路径(可选)： "), n(v, {
+                    placeholder: "微信文件夹路径[可为空,空表示使用默认的，无默认会报错](eg: C:\\****\\WeChat Files\\wxid_**** )",
+                    modelValue: l.value,
+                    "onUpdate:modelValue": u[1] || (u[1] = g => l.value = g),
+                    style: {
+                        width: "70%"
+                    }
+                }, null, 8, ["modelValue"]), fl, yl, e("div", xl, [n(w, {
+                    type: "primary",
+                    onClick: u[2] || (u[2] = g => r())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })]), n(d), n(v, {
+                    type: "textarea",
+                    rows: 6,
+                    readonly: "",
+                    placeholder: "",
+                    modelValue: s.value,
+                    "onUpdate:modelValue": u[3] || (u[3] = g => s.value = g),
+                    style: {
+                        width: "100%"
+                    }
+                }, null, 8, ["modelValue"])])
+            }
+        }
+    }),
+    gl = {
+        style: {
+            position: "relative"
+        }
+    },
+    bl = M({
+        __name: "ExportCSV",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (s, r) => {
+                console.log(s)
+            });
+            const l = m(""),
+                a = async () => {
+                    l.value = "正在处理中...";
+                    try {
+                        l.value = await T.post("/api/export_csv", {
+                            wxid: i.wxid
+                        })
+                    } catch (s) {
+                        return console.error("Error fetching data msg_count:", s), l.value = `请求失败
+` + s, []
+                    }
+                };
+            return (s, r) => {
+                const p = x("el-button"),
+                    u = x("el-divider"),
+                    v = x("el-input");
+                return o(), c("div", null, [e("div", gl, [n(p, {
+                    type: "primary",
+                    onClick: r[0] || (r[0] = w => a())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })]), n(u), n(v, {
+                    type: "textarea",
+                    rows: 6,
+                    readonly: "",
+                    placeholder: "",
+                    modelValue: l.value,
+                    "onUpdate:modelValue": r[1] || (r[1] = w => l.value = w),
+                    style: {
+                        width: "100%"
+                    }
+                }, null, 8, ["modelValue"])])
+            }
+        }
+    }),
+    $l = {
+        style: {
+            position: "relative"
+        }
+    },
+    kl = M({
+        __name: "ExportJSON",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (s, r) => {
+                console.log(s)
+            }), m([]);
+            const l = m(""),
+                a = async () => {
+                    l.value = "正在处理中...";
+                    try {
+                        l.value = await T.post("/api/export_json", {
+                            wxid: i.wxid
+                        })
+                    } catch (s) {
+                        return console.error("Error fetching data msg_count:", s), l.value = `请求失败
+` + s, []
+                    }
+                };
+            return (s, r) => {
+                const p = x("el-button"),
+                    u = x("el-divider"),
+                    v = x("el-input");
+                return o(), c("div", null, [e("div", $l, [n(p, {
+                    type: "primary",
+                    onClick: r[0] || (r[0] = w => a())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })]), n(u), n(v, {
+                    type: "textarea",
+                    rows: 6,
+                    readonly: "",
+                    placeholder: "",
+                    modelValue: l.value,
+                    "onUpdate:modelValue": r[1] || (r[1] = w => l.value = w),
+                    style: {
+                        width: "100%"
+                    }
+                }, null, 8, ["modelValue"])])
+            }
+        }
+    }),
+    Sl = {
+        style: {
+            position: "relative"
+        }
+    },
+    Vl = M({
+        __name: "ExportHTML",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (s, r) => {
+                console.log(s)
+            }), m([]);
+            const l = m(""),
+                a = async () => {
+                    l.value = "正在处理中...";
+                    try {
+                        l.value = await T.post("/api/export_html", {
+                            wxid: i.wxid
+                        })
+                    } catch (s) {
+                        return console.error("Error fetching data msg_count:", s), l.value = `请求失败
+` + s, []
+                    }
+                };
+            return (s, r) => {
+                const p = x("el-button"),
+                    u = x("el-divider"),
+                    v = x("el-input");
+                return o(), c("div", null, [e("div", Sl, [n(p, {
+                    type: "primary",
+                    onClick: r[0] || (r[0] = w => a())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })]), n(u), n(v, {
+                    type: "textarea",
+                    rows: 6,
+                    readonly: "",
+                    placeholder: "",
+                    modelValue: l.value,
+                    "onUpdate:modelValue": r[1] || (r[1] = w => l.value = w),
+                    style: {
+                        width: "100%"
+                    }
+                }, null, 8, ["modelValue"])])
+            }
+        }
+    }),
+    Ul = e("br", null, null, -1),
+    Ml = M({
+        __name: "ExportPDF",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (a, s) => {
+                console.log(a)
+            });
+            const l = () => {
+                console.log("requestExport")
+            };
+            return (a, s) => {
+                const r = x("el-button");
+                return o(), c("div", null, [e("span", null, k(i.wxid), 1), Ul, n(r, {
+                    type: "primary",
+                    onClick: s[0] || (s[0] = p => l())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })])
+            }
+        }
+    }),
+    El = e("br", null, null, -1),
+    Cl = M({
+        __name: "ExportDOCX",
+        props: {
+            wxid: {
+                type: String,
+                required: !0
+            }
+        },
+        setup(t) {
+            const i = t;
+            I(() => i.wxid, (a, s) => {
+                console.log(a)
+            });
+            const l = () => {
+                console.log("requestExport")
+            };
+            return (a, s) => {
+                const r = x("el-button");
+                return o(), c("div", null, [e("span", null, k(i.wxid), 1), El, n(r, {
+                    type: "primary",
+                    onClick: s[0] || (s[0] = p => l())
+                }, {
+                    default: _(() => [h("导出")]),
+                    _: 1
+                })])
+            }
+        }
+    }),
+    Tl = {
         id: "chat_export",
         style: {
             "background-color": "#d2d2fa",
             padding: "0"
         }
     },
-    ba = {
+    Dl = {
         style: {
             "background-color": "#d2d2fa",
             height: "calc(100vh - 65px)",
             display: "grid",
             "place-items": "center"
         }
     },
-    ka = {
+    ql = {
         style: {
             "background-color": "#fff",
             width: "70%",
             height: "70%",
             "border-radius": "10px",
             padding: "20px",
             overflow: "auto"
         }
     },
-    $a = e("div", {
+    zl = e("div", {
         style: {
             display: "flex",
             "justify-content": "space-between",
             "align-items": "center"
         }
     }, [e("div", {
         style: {
@@ -1287,500 +1578,269 @@
     }, "导出与备份(未完待续...）"), e("div", {
         style: {
             display: "flex",
             "justify-content": "space-between",
             "align-items": "center"
         }
     })], -1),
-    Sa = {
+    Rl = {
         style: {
             "margin-top": "20px"
         }
     },
-    Da = e("br", null, null, -1),
-    Ta = e("br", null, null, -1),
-    Ua = e("br", null, null, -1),
-    Ma = {
+    jl = e("br", null, null, -1),
+    Hl = e("br", null, null, -1),
+    Il = {
         key: 0
     },
-    Va = {
-        key: 1
-    },
-    Ca = e("strong", null, "** 时间(默认全部)：", -1),
-    Ea = {
-        key: 2
-    },
-    za = {
-        key: 3
-    },
-    Ha = {
-        key: 4
-    },
-    Ia = j({
+    Ol = M({
         __name: "ChatExportMain",
         props: {
-            userData: {
-                type: Object,
+            wxid: {
+                type: String,
                 required: !0
             }
         },
         setup(t) {
-            const v = t,
-                i = m(""),
-                r = m([]),
-                h = m(["文本"]),
-                $ = m(""),
-                _ = m(""),
-                s = m(""),
-                d = {
-                    endb: {
-                        brief: "加密文件",
-                        detail: `导出的内容为微信加密数据库（）。
-可还原回微信,但会覆盖微信后续消息。`,
-                        userShow: !1,
-                        timeShow: !1,
-                        chatTypeShow: !1,
-                        keyShow: !1,
-                        wxPathShow: !0
-                    },
-                    dedb: {
-                        brief: "解密文件",
-                        detail: "导出的文件为解密后的sqlite数据库，并且会自动合并msg和media数据库为同一个，但是无法还原回微信。",
-                        userShow: !1,
-                        timeShow: !0,
-                        chatTypeShow: !1,
-                        keyShow: !1,
-                        wxPathShow: !1
-                    },
-                    csv: {
-                        brief: "csv",
-                        detail: "只包含文本，但是可以用excel软件（wps，office）打开。",
-                        userShow: !0,
-                        timeShow: !1,
-                        chatTypeShow: !1,
-                        keyShow: !1,
-                        wxPathShow: !1
-                    },
-                    json: {
-                        brief: "json",
-                        detail: "只包含文本，可用于数据分析，情感分析等方面。",
-                        userShow: !0,
-                        timeShow: !1,
-                        chatTypeShow: !1,
-                        keyShow: !1,
-                        wxPathShow: !1
-                    },
-                    html: {
-                        brief: "html-测试中",
-                        detail: "主要用于浏览器可视化查看。",
-                        userShow: !0,
-                        timeShow: !1,
-                        chatTypeShow: !1,
-                        keyShow: !1,
-                        wxPathShow: !1
-                    },
-                    pdf: {
-                        brief: "pdf-开发中",
-                        detail: "就是html的pdf版本。",
-                        userShow: !0,
-                        timeShow: !0,
-                        chatTypeShow: !0,
-                        keyShow: !1,
-                        wxPathShow: !0
-                    },
-                    docx: {
-                        brief: "docx-开发中",
-                        detail: "就是html的docx版本。",
-                        userShow: !0,
-                        timeShow: !0,
-                        chatTypeShow: !0,
-                        keyShow: !1,
-                        wxPathShow: !0
-                    }
+            const i = t;
+            I(() => i.wxid, (s, r) => {
+                console.log(s)
+            });
+            const l = m("");
+            m("");
+            const a = {
+                endb: {
+                    brief: "加密文件",
+                    detail: "导出的内容为微信加密数据库。可还原回微信,但会覆盖微信后续消息。(全程不解密，所以数据安全)"
                 },
-                b = ["文本", "图片", "语音", "视频", "动画表情", "文件", "卡片式链接", "用户上传的GIF表情", "转账消息", "赠送红包封面", "语音通话", "系统通知", "拍一拍", "系统通知", "其他"],
-                w = m(!1),
-                D = m(!0),
-                z = n => {
-                    h.value = n ? b : [], D.value = !1
+                dedb: {
+                    brief: "解密文件",
+                    detail: "导出的文件为解密后的sqlite数据库，并且会自动合并msg和media数据库为同一个，但是无法还原回微信。"
                 },
-                p = n => {
-                    const f = n.length;
-                    w.value = f === b.length, D.value = f > 0 && f < b.length
+                csv: {
+                    brief: "csv",
+                    detail: "只包含文本，但是可以用excel软件（wps，office）打开。"
                 },
-                U = n => {
-                    r.value = n
+                json: {
+                    brief: "json",
+                    detail: "只包含文本，可用于数据分析，情感分析等方面。"
                 },
-                H = m(!1),
-                I = m(!1),
-                S = m(!1),
-                g = m(!1),
-                V = m(!1);
-            J(i, n => {
-                H.value = d[n].userShow, I.value = d[n].timeShow, S.value = d[n].chatTypeShow, g.value = d[n].keyShow, V.value = d[n].wxPathShow, s.value = d[n].detail
-            });
-            const T = async () => {
-                try {
-                    if (i.value === "") {
-                        s.value = "导出类型不能为空";
-                        return
-                    }
-                    const n = await O.post("/api/export", {
-                        export_type: i.value,
-                        start_time: r.value[0],
-                        end_time: r.value[1],
-                        chat_type: h.value,
-                        username: v.userData.wxid,
-                        wx_path: _.value
-                    });
-                    s.value = n
-                } catch (n) {
-                    W.alert(n, "error", {
-                        confirmButtonText: "确认",
-                        callback: f => {
-                            ne({
-                                type: "error",
-                                message: `action: ${f}`
-                            })
-                        }
-                    }), s.value = String(n) + `
-更多信息请查看控制台；`
+                html: {
+                    brief: "html-开发中",
+                    detail: "主要用于浏览器可视化查看。"
+                },
+                pdf: {
+                    brief: "pdf-开发中",
+                    detail: "pdf版本。"
+                },
+                docx: {
+                    brief: "docx-开发中",
+                    detail: "docx版本。"
                 }
             };
-            return (n, f) => {
-                const y = k("el-option"),
-                    N = k("el-select"),
-                    q = k("el-text"),
-                    P = k("el-col"),
-                    M = k("el-row"),
-                    ee = k("el-checkbox"),
-                    oe = k("el-checkbox-group"),
-                    Q = k("el-input"),
-                    ie = k("el-button"),
-                    re = k("el-divider"),
-                    ce = k("el-main");
-                return l(), u("div", xa, [a(ce, {
+            return (s, r) => {
+                const p = x("el-option"),
+                    u = x("el-select"),
+                    v = x("el-divider"),
+                    w = x("el-main");
+                return o(), c("div", Tl, [n(w, {
                     style: {
                         "overflow-y": "auto",
                         height: "calc(100vh - 65px)",
                         padding: "0"
                     }
                 }, {
-                    default: o(() => [e("div", ba, [e("div", ka, [$a, e("div", Sa, [c(" 导出类型: "), a(N, {
+                    default: _(() => [e("div", Dl, [e("div", ql, [zl, e("div", Rl, [h(" 导出类型: "), n(u, {
                         placeholder: "请选择导出类型",
                         style: {
                             width: "50%"
                         },
-                        modelValue: i.value,
-                        "onUpdate:modelValue": f[0] || (f[0] = C => i.value = C)
+                        modelValue: l.value,
+                        "onUpdate:modelValue": r[0] || (r[0] = d => l.value = d)
                     }, {
-                        default: o(() => [(l(), u(K, null, X(d, (C, te) => a(y, {
-                            label: C.brief,
-                            value: te,
-                            key: te
+                        default: _(() => [(o(), c(G, null, Z(a, (d, g) => n(p, {
+                            label: d.brief,
+                            value: g,
+                            key: g
                         }, {
-                            default: o(() => [c(x(C.brief), 1)]),
+                            default: _(() => [h(k(d.brief), 1)]),
                             _: 2
                         }, 1032, ["label", "value"])), 64))]),
                         _: 1
-                    }, 8, ["modelValue"]), Da, Ta, e("div", null, [c(" 选项:"), Ua, H.value ? (l(), u("div", Ma, [c(" ** 用户(默认全部，从左边选择具体用户)： "), a(M, {
-                        gutter: 5,
-                        style: {
-                            width: "100%"
-                        }
-                    }, {
-                        default: o(() => [a(P, {
-                            span: 6,
-                            style: {
-                                "white-space": "nowrap"
-                            }
-                        }, {
-                            default: o(() => [a(q, {
-                                class: "label_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c("原始id:")]),
-                                _: 1
-                            }), c("  "), a(q, {
-                                class: "data_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c(x(t.userData.wxid), 1)]),
-                                _: 1
-                            })]),
-                            _: 1
-                        }), a(P, {
-                            span: 6,
-                            style: {
-                                "white-space": "nowrap"
-                            }
-                        }, {
-                            default: o(() => [a(q, {
-                                class: "label_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c("账号:")]),
-                                _: 1
-                            }), c("  "), a(q, {
-                                class: "data_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c(x(t.userData.account), 1)]),
-                                _: 1
-                            })]),
-                            _: 1
-                        }), a(P, {
-                            span: 6,
-                            style: {
-                                "white-space": "nowrap"
-                            }
-                        }, {
-                            default: o(() => [a(q, {
-                                class: "label_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c("昵称:")]),
-                                _: 1
-                            }), c("  "), a(q, {
-                                class: "data_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c(x(t.userData.nickname), 1)]),
-                                _: 1
-                            })]),
-                            _: 1
-                        }), a(P, {
-                            span: 6,
-                            style: {
-                                "white-space": "nowrap"
-                            }
-                        }, {
-                            default: o(() => [a(q, {
-                                class: "label_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c("备注:")]),
-                                _: 1
-                            }), c("  "), a(q, {
-                                class: "data_color mx-1",
-                                truncated: ""
-                            }, {
-                                default: o(() => [c(x(t.userData.remark), 1)]),
-                                _: 1
-                            })]),
-                            _: 1
-                        })]),
-                        _: 1
-                    })])) : R("", !0), I.value ? (l(), u("div", Va, [Ca, a(ga, {
-                        onDatetime: U
-                    })])) : R("", !0), S.value ? (l(), u("div", Ea, [c(" ** 消息类型： "), a(ee, {
-                        modelValue: w.value,
-                        "onUpdate:modelValue": f[1] || (f[1] = C => w.value = C),
-                        indeterminate: D.value,
-                        onChange: z
-                    }, {
-                        default: o(() => [c("全选 ")]),
-                        _: 1
-                    }, 8, ["modelValue", "indeterminate"]), a(oe, {
-                        modelValue: h.value,
-                        "onUpdate:modelValue": f[2] || (f[2] = C => h.value = C),
-                        onChange: p
-                    }, {
-                        default: o(() => [(l(), u(K, null, X(b, C => a(ee, {
-                            key: C,
-                            label: C
-                        }, {
-                            default: o(() => [c(x(C), 1)]),
-                            _: 2
-                        }, 1032, ["label"])), 64))]),
-                        _: 1
-                    }, 8, ["modelValue"])])) : R("", !0), g.value ? (l(), u("div", za, [c(" ** 微信文件夹路径： "), a(Q, {
-                        placeholder: "密钥key[可为空]",
-                        modelValue: $.value,
-                        "onUpdate:modelValue": f[3] || (f[3] = C => $.value = C),
-                        style: {
-                            width: "50%"
-                        }
-                    }, null, 8, ["modelValue"])])) : R("", !0), V.value ? (l(), u("div", Ha, [c(" ** 微信文件夹路径： "), a(Q, {
-                        placeholder: "微信文件夹路径[可为空](eg: C:\\****\\WeChat Files\\wxid_**** )",
-                        modelValue: _.value,
-                        "onUpdate:modelValue": f[4] || (f[4] = C => _.value = C),
-                        style: {
-                            width: "50%"
-                        }
-                    }, null, 8, ["modelValue"])])) : R("", !0)]), a(ie, {
-                        style: {
-                            "margin-top": "10px",
-                            width: "50%"
-                        },
-                        type: "success",
-                        onClick: T
-                    }, {
-                        default: o(() => [c("导出")]),
-                        _: 1
-                    }), a(re), a(Q, {
-                        type: "textarea",
-                        rows: 6,
-                        readonly: "",
-                        placeholder: "",
-                        modelValue: s.value,
-                        "onUpdate:modelValue": f[5] || (f[5] = C => s.value = C),
-                        style: {
-                            width: "100%"
-                        }
-                    }, null, 8, ["modelValue"])])])])]),
+                    }, 8, ["modelValue"]), jl, Hl, l.value ? (o(), c("span", Il, k(a[l.value].detail), 1)) : E("", !0)]), n(v), l.value == "endb" ? (o(), U(vl, {
+                        key: 0,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0), l.value == "dedb" ? (o(), U(wl, {
+                        key: 1,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0), l.value == "csv" ? (o(), U(bl, {
+                        key: 2,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0), l.value == "json" ? (o(), U(kl, {
+                        key: 3,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0), l.value == "html" ? (o(), U(Vl, {
+                        key: 4,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0), l.value == "pdf" ? (o(), U(Ml, {
+                        key: 5,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0), l.value == "docx" ? (o(), U(Cl, {
+                        key: 6,
+                        wxid: i.wxid
+                    }, null, 8, ["wxid"])) : E("", !0)])])]),
                     _: 1
                 })])
             }
         }
     }),
-    Ra = j({
+    Ll = M({
         __name: "ChatRecords",
         props: {
             wxid: {
                 type: String,
                 required: !0
             }
         },
         setup(t) {
-            const v = m(null),
-                i = m(null);
+            const i = m(null),
+                l = m(null);
             m(0);
-            const r = m(0),
-                h = () => {
-                    G(() => {
-                        if (v.value) {
-                            const p = v.value.$el.children[0];
-                            p && (p.scrollTop = p.scrollHeight, r.value = p.scrollHeight)
+            const a = m(0),
+                s = () => {
+                    A(() => {
+                        if (i.value) {
+                            const y = i.value.$el.children[0];
+                            y && (y.scrollTop = y.scrollHeight, a.value = y.scrollHeight)
                         }
                     })
                 },
-                $ = () => {
-                    const p = v.value.$el.children[0];
-                    if (p) {
-                        const U = r.value,
-                            H = p.scrollHeight - U;
-                        p.scrollTop = p.scrollTop + H, r.value = p.scrollHeight
+                r = () => {
+                    const y = i.value.$el.children[0];
+                    if (y) {
+                        const q = a.value,
+                            j = y.scrollHeight - q;
+                        y.scrollTop = y.scrollTop + j, a.value = y.scrollHeight
                     }
                 };
 
-            function _({
-                scrollTop: p
+            function p({
+                scrollTop: y
             }) {
-                p === 0 && i.value && i.value.loadMore()
+                y === 0 && l.value && l.value.loadMore()
             }
-            const s = t,
-                d = m({
+            const u = t,
+                v = m({
                     account: "",
                     describe: "",
                     headImgUrl: "",
                     nickname: "",
                     remark: "",
                     wxid: "",
                     msg_count: 0
                 }),
-                b = async () => {
+                w = async () => {
                     try {
-                        const p = await O.post("/api/wxid2user", {
-                            wxid: s.wxid
+                        const y = await T.post("/api/wxid2user", {
+                            wxid: u.wxid
                         });
-                        return d.value.account = p[s.wxid].account, d.value.describe = p[s.wxid].describe, d.value.headImgUrl = p[s.wxid].headImgUrl, d.value.nickname = p[s.wxid].nickname, d.value.remark = p[s.wxid].remark, d.value.wxid = s.wxid, p
-                    } catch (p) {
-                        return console.error("Error fetching data wxid2user :", p), []
+                        return v.value.account = y[u.wxid].account, v.value.describe = y[u.wxid].describe, v.value.headImgUrl = y[u.wxid].headImgUrl, v.value.nickname = y[u.wxid].nickname, v.value.remark = y[u.wxid].remark, v.value.wxid = u.wxid, y
+                    } catch (y) {
+                        return console.error("Error fetching data wxid2user :", y), []
                     }
-                }, w = async () => {
+                }, d = async () => {
                     try {
-                        const p = await O.post("/api/msg_count", {
-                            wxid: s.wxid
+                        const y = await T.post("/api/msg_count", {
+                            wxid: u.wxid
                         });
-                        return d.value.msg_count = p[s.wxid], p
-                    } catch (p) {
-                        return console.error("Error fetching data msg_count:", p), []
+                        return v.value.msg_count = y[u.wxid], y
+                    } catch (y) {
+                        return console.error("Error fetching data msg_count:", y), []
                     }
                 };
-            Z(() => {
-                w(), b(), G(() => {
-                    h()
+            Y(() => {
+                d(), w(), A(() => {
+                    s()
                 })
             });
-            const D = m(!1),
-                z = p => {
-                    D.value = p
+            const g = m(!1),
+                D = y => {
+                    g.value = y, g.value === !1 && (v.value.wxid = "", w())
                 };
-            return J(() => s.wxid, async (p, U) => {
-                p !== U && (b(), w(), D.value = !1, G(() => {
-                    h()
+            return I(() => u.wxid, async (y, q) => {
+                y !== q && (w(), d(), g.value = !1, A(() => {
+                    s()
                 }))
-            }), (p, U) => {
-                const H = k("el-header"),
-                    I = k("el-scrollbar"),
-                    S = k("el-main"),
-                    g = k("el-container");
-                return l(), E(g, null, {
-                    default: o(() => [a(H, {
+            }), (y, q) => {
+                const j = x("el-header"),
+                    H = x("el-scrollbar"),
+                    V = x("el-main"),
+                    $ = x("el-container");
+                return o(), U($, null, {
+                    default: _(() => [n(j, {
                         style: {
                             height: "65px",
                             "max-height": "65px",
                             width: "100%",
                             "background-color": "#d2d2fa",
                             "padding-top": "5px"
                         }
                     }, {
-                        default: o(() => [a(xe, {
-                            userData: d.value,
-                            onExporting: z
+                        default: _(() => [n(pe, {
+                            userData: v.value,
+                            onExporting: D
                         }, null, 8, ["userData"])]),
                         _: 1
-                    }), a(S, {
+                    }), n(V, {
                         style: {
                             "overflow-y": "auto",
                             height: "calc(100vh - 65px)",
                             padding: "0"
                         }
                     }, {
-                        default: o(() => [a(I, {
+                        default: _(() => [n(H, {
                             ref_key: "scrollbarRef",
-                            ref: v,
-                            onScroll: _
+                            ref: i,
+                            onScroll: p
                         }, {
-                            default: o(() => [D.value ? (l(), E(Ia, {
+                            default: _(() => [g.value ? (o(), U(Ol, {
                                 key: 0,
-                                userData: d.value
-                            }, null, 8, ["userData"])) : (l(), E(ya, {
+                                wxid: v.value.wxid
+                            }, null, 8, ["wxid"])) : (o(), U(dl, {
                                 key: 1,
                                 ref_key: "chatRecordsMainRef",
-                                ref: i,
-                                userData: d.value,
-                                setScrollTop: h,
-                                updateScrollTop: $
+                                ref: l,
+                                userData: v.value,
+                                setScrollTop: s,
+                                updateScrollTop: r
                             }, null, 8, ["userData"]))]),
                             _: 1
                         }, 512)]),
                         _: 1
                     })]),
                     _: 1
                 })
             }
         }
     }),
-    ja = {
+    Nl = {
         class: "progress-bar"
     },
-    le = j({
+    Q = M({
         __name: "ProgressBar",
         props: {
             startORstop: {
                 type: Number,
                 required: !0
             }
         },
         setup(t) {
-            const v = m(0),
-                i = m(500),
-                r = [{
+            const i = m(0),
+                l = m(500),
+                a = [{
                     color: "#f56c6c",
                     percentage: 20
                 }, {
                     color: "#e6a23c",
                     percentage: 40
                 }, {
                     color: "#5cb87a",
@@ -1788,98 +1848,98 @@
                 }, {
                     color: "#1989fa",
                     percentage: 80
                 }, {
                     color: "#6f7ad3",
                     percentage: 100
                 }],
-                h = m(new Date().getTime()),
-                $ = t,
-                _ = () => {
-                    if ($.startORstop === 1) {
-                        v.value = 100;
+                s = m(new Date().getTime()),
+                r = t,
+                p = () => {
+                    if (r.startORstop === 1) {
+                        i.value = 100;
                         return
                     }
-                    h.value = new Date().getTime(), !(v.value >= 99) && (v.value >= 80 && (i.value = i.value + 50), v.value = v.value + 1, setTimeout(_, i.value))
+                    s.value = new Date().getTime(), !(i.value >= 99) && (i.value >= 80 && (l.value = l.value + 50), i.value = i.value + 1, setTimeout(p, l.value))
                 };
-            return _(), (s, d) => {
-                const b = k("el-progress");
-                return l(), u("div", ja, [a(b, {
+            return p(), (u, v) => {
+                const w = x("el-progress");
+                return o(), c("div", Nl, [n(w, {
                     type: "dashboard",
-                    percentage: v.value,
-                    color: r
+                    percentage: i.value,
+                    color: a
                 }, null, 8, ["percentage"])])
             }
         }
     }),
-    Oa = {
+    Bl = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "flex",
             "justify-content": "center",
             "align-items": "center"
         }
     },
-    qa = {
+    Fl = {
         key: 0
     },
-    La = {
+    Al = {
         key: 1,
         style: {
             "background-color": "#fff",
             width: "90%",
             "min-width": "800px",
             height: "80%",
             "border-radius": "10px",
             padding: "20px",
             overflow: "auto"
         }
     },
-    Pa = e("div", {
+    Pl = e("div", {
         style: {
             display: "flex",
             "justify-content": "space-between",
             "align-items": "center"
         }
     }, [e("div", {
         style: {
             "font-size": "20px",
             "font-weight": "bold"
         }
     }, "选择要查看的微信")], -1),
-    Fa = {
+    Wl = {
         style: {
             "margin-top": "20px"
         }
     },
-    Na = {
+    Kl = {
         style: {
             "margin-top": "20px"
         }
     },
-    Ba = {
+    Gl = {
         key: 1
     },
-    Aa = {
+    Yl = {
         key: 0
     },
-    Ya = {
+    Jl = {
         key: 1,
         style: {
             "background-color": "#fff",
             width: "80%",
             "min-width": "800px",
             height: "70%",
             "border-radius": "10px",
             padding: "20px",
             overflow: "auto"
         }
     },
-    Wa = e("div", {
+    Xl = e("div", {
         style: {
             display: "flex",
             "justify-content": "space-between",
             "align-items": "center"
         }
     }, [e("div", {
         style: {
@@ -1889,400 +1949,400 @@
     }, "自定义-文件位置"), e("div", {
         style: {
             display: "flex",
             "justify-content": "space-between",
             "align-items": "center"
         }
     })], -1),
-    Ga = {
+    Ql = {
         style: {
             "margin-top": "20px"
         }
     },
-    Ka = {
+    Zl = {
         key: 0
     },
-    Ja = e("br", null, null, -1),
-    Qa = e("br", null, null, -1),
-    Xa = {
+    en = e("br", null, null, -1),
+    tn = e("br", null, null, -1),
+    ln = {
         key: 1
     },
-    Za = e("br", null, null, -1),
-    es = e("br", null, null, -1),
-    ts = {
+    nn = e("br", null, null, -1),
+    on = e("br", null, null, -1),
+    sn = {
         key: 2
     },
-    as = e("label", null, "密钥key(必填): ", -1),
-    ss = e("br", null, null, -1),
-    ls = {
+    an = e("label", null, "密钥key(必填): ", -1),
+    rn = e("br", null, null, -1),
+    cn = {
         key: 3
     },
-    ns = e("label", null, "merge_all.db 路径(必填): ", -1),
-    os = e("br", null, null, -1),
-    is = e("label", null, "微信文件夹路径(必填): ", -1),
-    rs = e("br", null, null, -1),
-    cs = e("label", null, "微信原始id(必填): ", -1),
-    ds = e("br", null, null, -1),
-    us = {
+    dn = e("label", null, "merge_all.db 路径(必填): ", -1),
+    un = e("br", null, null, -1),
+    _n = e("label", null, "微信文件夹路径(必填): ", -1),
+    pn = e("br", null, null, -1),
+    vn = e("label", null, "微信原始id(必填): ", -1),
+    hn = e("br", null, null, -1),
+    mn = {
         key: 2
     },
-    _s = {
+    fn = {
         key: 3,
         style: {
             display: "flex",
             "justify-content": "space-between"
         }
     },
-    hs = {
+    yn = {
         style: {
             width: "200px",
             height: "150px",
             "background-color": "#fff",
             display: "flex",
             "flex-direction": "column",
             "align-items": "center",
             "border-radius": "10px",
             "margin-right": "20px"
         }
     },
-    ms = e("div", {
+    xn = e("div", {
         style: {
             display: "flex",
             "flex-direction": "column",
             "justify-content": "center",
             "align-items": "center",
             height: "100%"
         }
     }, [e("div", null, "使用上次设置")], -1),
-    fs = {
+    wn = {
         style: {
             width: "200px",
             height: "150px",
             "background-color": "#fff",
             display: "flex",
             "flex-direction": "column",
             "align-items": "center",
             "border-radius": "10px",
             "margin-right": "20px"
         }
     },
-    ps = e("div", {
+    gn = e("div", {
         style: {
             display: "flex",
             "flex-direction": "column",
             "justify-content": "center",
             "align-items": "center",
             height: "100%"
         }
     }, [e("div", null, "自动解密已登录微信")], -1),
-    vs = {
+    bn = {
         style: {
             width: "200px",
             height: "150px",
             "background-color": "#fff",
             display: "flex",
             "flex-direction": "column",
             "align-items": "center",
             "border-radius": "10px"
         }
     },
-    ys = e("div", {
+    $n = e("div", {
         style: {
             display: "flex",
             "flex-direction": "column",
             "justify-content": "center",
             "align-items": "center",
             height: "100%"
         }
     }, [e("div", null, "自定义文件位置")], -1),
-    ws = j({
+    kn = M({
         __name: "IsAutoShow",
         emits: ["isAutoShow"],
         setup(t, {
-            emit: v
+            emit: i
         }) {
-            const i = m(0),
-                r = m(-1),
-                h = m(""),
-                $ = m(!1),
-                _ = m([]),
+            const l = m(0),
+                a = m(-1),
                 s = m(""),
-                d = m(!1),
-                b = m(!1),
-                w = m("false"),
+                r = m(!1),
+                p = m([]),
+                u = m(""),
+                v = m(!1),
+                w = m(!1),
+                d = m("false"),
+                g = m(""),
                 D = m(""),
-                z = m(""),
-                p = m(""),
-                U = m(""),
-                H = v,
-                I = async () => {
+                y = m(""),
+                q = m(""),
+                j = i,
+                H = async () => {
                     try {
-                        _.value = await O.post("/api/wxinfo"), _.value.length === 1 && (S(_.value[0]), s.value = " (检测到只有一个微信，将在5秒后自动选择) ", setTimeout(g, 5e3))
-                    } catch (f) {
-                        return console.error("Error fetching data:", f), []
-                    }
-                }, S = async f => {
-                    D.value = "", z.value = f.filePath, p.value = f.key, U.value = f.wxid
-                }, g = () => {
-                    z.value === "" && p.value === "" && U.value === "" || d.value || (d.value = !0, V())
-                }, V = async () => {
-                    if (!d.value) try {
-                        d.value = !0, r.value = 0;
-                        let f = {
-                            wx_path: z.value,
-                            key: p.value,
-                            my_wxid: U.value
+                        p.value = await T.post("/api/wxinfo"), p.value.length === 1 && (V(p.value[0]), u.value = " (检测到只有一个微信，将在5秒后自动选择) ", setTimeout($, 5e3))
+                    } catch (S) {
+                        return console.error("Error fetching data:", S), []
+                    }
+                }, V = async S => {
+                    g.value = "", D.value = S.filePath, y.value = S.key, q.value = S.wxid
+                }, $ = () => {
+                    D.value === "" && y.value === "" && q.value === "" || v.value || (v.value = !0, z())
+                }, z = async () => {
+                    if (!v.value) try {
+                        v.value = !0, a.value = 0;
+                        let S = {
+                            wx_path: D.value,
+                            key: y.value,
+                            my_wxid: q.value
                         };
-                        const y = await O.post("/api/init_key", f);
-                        $.value = y.is_init, y.is_init && (i.value = 100, d.value = !1), H("isAutoShow", y.is_init)
-                    } catch (f) {
-                        return i.value = 0, b.value = !0, W.alert(f, "error", {
+                        const b = await T.post("/api/init_key", S);
+                        r.value = b.is_init, b.is_init && (l.value = 100, v.value = !1), j("isAutoShow", b.is_init)
+                    } catch (S) {
+                        return l.value = 0, w.value = !0, K.alert(S, "error", {
                             confirmButtonText: "确认",
-                            callback: y => {
-                                ne({
+                            callback: b => {
+                                oe({
                                     type: "error",
-                                    message: `action: ${y}`
+                                    message: `action: ${b}`
                                 })
                             }
                         }), []
                     }
-                }, T = async () => {
+                }, C = async () => {
                     try {
-                        let f = {
-                            wx_path: z.value,
-                            merge_path: D.value,
-                            my_wxid: U.value
+                        let S = {
+                            wx_path: D.value,
+                            merge_path: g.value,
+                            my_wxid: q.value
                         };
-                        const y = await O.post("/api/init_nokey", f);
-                        $.value = y.is_init, y.is_init && (i.value = 100, d.value = !1), H("isAutoShow", y.is_init)
-                    } catch (f) {
-                        return i.value = 0, b.value = !0, W.alert(f, "error", {
+                        const b = await T.post("/api/init_nokey", S);
+                        r.value = b.is_init, b.is_init && (l.value = 100, v.value = !1), j("isAutoShow", b.is_init)
+                    } catch (S) {
+                        return l.value = 0, w.value = !0, K.alert(S, "error", {
                             confirmButtonText: "确认",
-                            callback: y => {
-                                h.value = ""
+                            callback: b => {
+                                s.value = ""
                             }
                         }), []
                     }
-                }, n = async () => {
+                }, f = async () => {
                     try {
-                        let f = {
-                            wx_path: z.value,
-                            merge_path: D.value,
-                            my_wxid: U.value
+                        let S = {
+                            wx_path: D.value,
+                            merge_path: g.value,
+                            my_wxid: q.value
                         };
-                        const y = await O.post("/api/init_last", f);
-                        $.value = y.is_init, y.is_init ? (i.value = 100, d.value = !1, H("isAutoShow", y.is_init)) : (b.value = !0, W.alert("未发现上次的设置数据！", "error", {
+                        const b = await T.post("/api/init_last", S);
+                        r.value = b.is_init, b.is_init ? (l.value = 100, v.value = !1, j("isAutoShow", b.is_init)) : (w.value = !0, K.alert("未发现上次的设置数据！", "error", {
                             confirmButtonText: "确认",
-                            callback: N => {
-                                h.value = ""
+                            callback: P => {
+                                s.value = ""
                             }
                         }))
-                    } catch (f) {
-                        return b.value = !0, W.alert(f, "error", {
+                    } catch (S) {
+                        return w.value = !0, K.alert(S, "error", {
                             confirmButtonText: "确认",
-                            callback: y => {
-                                h.value = ""
+                            callback: b => {
+                                s.value = ""
                             }
                         }), []
                     }
                 };
-            return J(h, f => {
-                f === "auto" ? I() : f === "custom" || f === "last" && n()
-            }), (f, y) => {
-                const N = k("el-button"),
-                    q = k("el-divider"),
-                    P = k("el-input");
-                return l(), u("div", Oa, [h.value === "auto" ? (l(), u("div", qa, [d.value ? (l(), E(le, {
+            return I(s, S => {
+                S === "auto" ? H() : S === "custom" || S === "last" && f()
+            }), (S, b) => {
+                const P = x("el-button"),
+                    ee = x("el-divider"),
+                    W = x("el-input");
+                return o(), c("div", Bl, [s.value === "auto" ? (o(), c("div", Fl, [v.value ? (o(), U(Q, {
                     key: 0,
-                    startORstop: r.value
-                }, null, 8, ["startORstop"])) : (l(), u("div", La, [Pa, e("div", Fa, [a(F(_e), {
-                    data: _.value,
-                    onCurrentChange: S,
+                    startORstop: a.value
+                }, null, 8, ["startORstop"])) : (o(), c("div", Al, [Pl, e("div", Wl, [n(L(ne), {
+                    data: p.value,
+                    onCurrentChange: V,
                     "highlight-current-row": "",
                     style: {
                         width: "100%"
                     }
                 }, {
-                    default: o(() => [a(F(B), {
+                    default: _(() => [n(L(N), {
                         "min-width": 30,
                         prop: "pid",
                         label: "进程id"
-                    }), a(F(B), {
+                    }), n(L(N), {
                         "min-width": 40,
                         prop: "version",
                         label: "微信版本"
-                    }), a(F(B), {
+                    }), n(L(N), {
                         "min-width": 40,
                         prop: "account",
                         label: "账号"
-                    }), a(F(B), {
+                    }), n(L(N), {
                         "min-width": 40,
                         prop: "name",
                         label: "昵称"
-                    }), a(F(B), {
+                    }), n(L(N), {
                         "min-width": 50,
                         prop: "wxid",
                         label: "微信原始id"
                     })]),
                     _: 1
-                }, 8, ["data"])]), e("div", Na, [a(N, {
+                }, 8, ["data"])]), e("div", Kl, [n(P, {
                     style: {
                         "margin-right": "10px",
                         "margin-top": "10px",
                         width: "100%"
                     },
                     type: "success",
-                    onClick: g
+                    onClick: $
                 }, {
-                    default: o(() => [c("确定" + x(s.value), 1)]),
+                    default: _(() => [h("确定" + k(u.value), 1)]),
                     _: 1
-                })])]))])) : h.value === "custom" ? (l(), u("div", Ba, [d.value ? (l(), u("div", Aa, [d.value ? (l(), E(le, {
+                })])]))])) : s.value === "custom" ? (o(), c("div", Gl, [v.value ? (o(), c("div", Yl, [v.value ? (o(), U(Q, {
                     key: 0,
-                    startORstop: r.value
-                }, null, 8, ["startORstop"])) : R("", !0)])) : (l(), u("div", Ya, [Wa, e("div", Ga, [A(e("input", {
+                    startORstop: a.value
+                }, null, 8, ["startORstop"])) : E("", !0)])) : (o(), c("div", Jl, [Xl, e("div", Ql, [B(e("input", {
                     type: "radio",
-                    "onUpdate:modelValue": y[0] || (y[0] = M => w.value = M),
+                    "onUpdate:modelValue": b[0] || (b[0] = R => d.value = R),
                     value: "true"
                 }, null, 512), [
-                    [Y, w.value]
-                ]), c(" 使用 KEY          "), A(e("input", {
+                    [F, d.value]
+                ]), h(" 使用 KEY          "), B(e("input", {
                     type: "radio",
-                    "onUpdate:modelValue": y[1] || (y[1] = M => w.value = M),
+                    "onUpdate:modelValue": b[1] || (b[1] = R => d.value = R),
                     value: "false"
                 }, null, 512), [
-                    [Y, w.value]
-                ]), c(" 不使用 KEY "), w.value == "false" ? (l(), u("div", Ka, [c(" 说明：1、表示数据库已解密并合并"), Ja, c("2、合并后的数据库需要包含(MediaMSG,MSG,MicroMsg,OpenIMMsg)这些数据库合并的内容"), Qa])) : R("", !0), w.value == "true" ? (l(), u("div", Xa, [c(" 说明：1、自动根据key解密微信文件夹下的数据库"), Za, c("2、必须保证key正确，否则解密失败"), es])) : R("", !0), a(q), w.value == "true" ? (l(), u("div", ts, [as, a(P, {
+                    [F, d.value]
+                ]), h(" 不使用 KEY "), d.value == "false" ? (o(), c("div", Zl, [h(" 说明：1、表示数据库已解密并合并"), en, h("2、合并后的数据库需要包含(MediaMSG,MSG,MicroMsg,OpenIMMsg)这些数据库合并的内容"), tn])) : E("", !0), d.value == "true" ? (o(), c("div", ln, [h(" 说明：1、自动根据key解密微信文件夹下的数据库"), nn, h("2、必须保证key正确，否则解密失败"), on])) : E("", !0), n(ee), d.value == "true" ? (o(), c("div", sn, [an, n(W, {
                     placeholder: "密钥key (64位)",
-                    modelValue: p.value,
-                    "onUpdate:modelValue": y[2] || (y[2] = M => p.value = M),
+                    modelValue: y.value,
+                    "onUpdate:modelValue": b[2] || (b[2] = R => y.value = R),
                     style: {
                         width: "80%"
                     }
-                }, null, 8, ["modelValue"]), ss])) : R("", !0), w.value == "false" ? (l(), u("div", ls, [ns, a(P, {
+                }, null, 8, ["modelValue"]), rn])) : E("", !0), d.value == "false" ? (o(), c("div", cn, [dn, n(W, {
                     placeholder: "(MediaMSG.db,MSG.db,MicroMsg.db,OpenIMMsg.db)合并后的数据库",
-                    modelValue: D.value,
-                    "onUpdate:modelValue": y[3] || (y[3] = M => D.value = M),
+                    modelValue: g.value,
+                    "onUpdate:modelValue": b[3] || (b[3] = R => g.value = R),
                     style: {
                         width: "80%"
                     }
-                }, null, 8, ["modelValue"]), os])) : R("", !0), is, a(P, {
+                }, null, 8, ["modelValue"]), un])) : E("", !0), _n, n(W, {
                     placeholder: "C:\\***\\WeChat Files\\wxid_*******",
-                    modelValue: z.value,
-                    "onUpdate:modelValue": y[4] || (y[4] = M => z.value = M),
+                    modelValue: D.value,
+                    "onUpdate:modelValue": b[4] || (b[4] = R => D.value = R),
                     style: {
                         width: "80%"
                     }
-                }, null, 8, ["modelValue"]), rs, cs, a(P, {
+                }, null, 8, ["modelValue"]), pn, vn, n(W, {
                     placeholder: "wxid_*******",
-                    modelValue: U.value,
-                    "onUpdate:modelValue": y[5] || (y[5] = M => U.value = M),
+                    modelValue: q.value,
+                    "onUpdate:modelValue": b[5] || (b[5] = R => q.value = R),
                     style: {
                         width: "80%"
                     }
-                }, null, 8, ["modelValue"]), ds, w.value == "true" ? (l(), E(N, {
+                }, null, 8, ["modelValue"]), hn, d.value == "true" ? (o(), U(P, {
                     key: 4,
                     style: {
                         "margin-top": "10px",
                         width: "100%"
                     },
                     type: "success",
-                    onClick: V
+                    onClick: z
                 }, {
-                    default: o(() => [c(" 确定 ")]),
+                    default: _(() => [h(" 确定 ")]),
                     _: 1
-                })) : R("", !0), w.value == "false" ? (l(), E(N, {
+                })) : E("", !0), d.value == "false" ? (o(), U(P, {
                     key: 5,
                     style: {
                         "margin-top": "10px",
                         width: "100%"
                     },
                     type: "success",
-                    onClick: T
+                    onClick: C
                 }, {
-                    default: o(() => [c(" 确定 ")]),
+                    default: _(() => [h(" 确定 ")]),
                     _: 1
-                })) : R("", !0)])]))])) : h.value === "last" ? (l(), u("div", us)) : h.value === "" ? (l(), u("div", _s, [e("label", hs, [A(e("input", {
+                })) : E("", !0)])]))])) : s.value === "last" ? (o(), c("div", mn)) : s.value === "" ? (o(), c("div", fn, [e("label", yn, [B(e("input", {
                     type: "radio",
-                    "onUpdate:modelValue": y[6] || (y[6] = M => h.value = M),
+                    "onUpdate:modelValue": b[6] || (b[6] = R => s.value = R),
                     value: "last"
                 }, null, 512), [
-                    [Y, h.value]
-                ]), ms]), e("label", fs, [A(e("input", {
+                    [F, s.value]
+                ]), xn]), e("label", wn, [B(e("input", {
                     type: "radio",
-                    "onUpdate:modelValue": y[7] || (y[7] = M => h.value = M),
+                    "onUpdate:modelValue": b[7] || (b[7] = R => s.value = R),
                     value: "auto"
                 }, null, 512), [
-                    [Y, h.value]
-                ]), ps]), e("label", vs, [A(e("input", {
+                    [F, s.value]
+                ]), gn]), e("label", bn, [B(e("input", {
                     type: "radio",
-                    "onUpdate:modelValue": y[8] || (y[8] = M => h.value = M),
+                    "onUpdate:modelValue": b[8] || (b[8] = R => s.value = R),
                     value: "custom"
                 }, null, 512), [
-                    [Y, h.value]
-                ]), ys])])) : R("", !0)])
+                    [F, s.value]
+                ]), $n])])) : E("", !0)])
             }
         }
     }),
-    gs = {
+    Sn = {
         id: "chat_view",
         class: "common-layout"
     },
-    xs = {
+    Vn = {
         key: 0
     },
-    bs = {
+    Un = {
         key: 1
     },
-    ks = {
+    Mn = {
         key: 0,
         style: {
             height: "calc(100vh)",
             width: "100%"
         }
     },
-    $s = {
+    En = {
         key: 1,
         style: {
             width: "100%",
             height: "100%"
         }
     },
-    Ms = j({
+    zn = M({
         __name: "ChatView",
         setup(t) {
-            const v = m(!1),
-                i = $ => {
-                    v.value = $
+            const i = m(!1),
+                l = r => {
+                    i.value = r
                 },
-                r = m(""),
-                h = $ => {
-                    r.value = $
+                a = m(""),
+                s = r => {
+                    a.value = r
                 };
-            return ($, _) => {
-                const s = k("el-aside"),
-                    d = k("el-container");
-                return l(), u("div", gs, [v.value ? (l(), u("div", bs, [a(d, null, {
-                    default: o(() => [a(s, {
+            return (r, p) => {
+                const u = x("el-aside"),
+                    v = x("el-container");
+                return o(), c("div", Sn, [i.value ? (o(), c("div", Un, [n(v, null, {
+                    default: _(() => [n(u, {
                         width: "auto",
                         style: {
                             "overflow-y": "auto",
                             height: "calc(100vh)"
                         }
                     }, {
-                        default: o(() => [a(we, {
-                            onWxid: h
+                        default: _(() => [n(ue, {
+                            onWxid: s
                         })]),
                         _: 1
-                    }), r.value != "" ? (l(), u("div", ks, [a(Ra, {
-                        wxid: r.value
-                    }, null, 8, ["wxid"])])) : (l(), u("div", $s, [a(he)]))]),
+                    }), a.value != "" ? (o(), c("div", Mn, [n(Ll, {
+                        wxid: a.value
+                    }, null, 8, ["wxid"])])) : (o(), c("div", En, [n(se)]))]),
                     _: 1
-                })])) : (l(), u("div", xs, [a(ws, {
-                    onIsAutoShow: i
+                })])) : (o(), c("div", Vn, [n(kn, {
+                    onIsAutoShow: l
                 })]))])
             }
         }
     });
 export {
-    Ms as
+    zn as
     default
 };
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/CleanupView-E355vjQT.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/CleanupView-JwdNAC7i.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import "./axios--FnjuHWf.js"; /* empty css                                                                       */
 import {
     d as o,
     b as s,
     c as a,
     e,
     h as t
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const c = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
         }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/DateTimeSelect-L-ShBE0O.css` & `pywxdump-3.0.8/pywxdump/ui/web/assets/DateTimeSelect-_xTa7bZL.css`

 * *Files 22% similar despite different names*

```diff
@@ -1 +1 @@
-.label_color[data-v-7bc26671]{color:#333;font-size:15px;padding-left:15px;padding-right:0}.data_color[data-v-7bc26671]{color:#08488c;background-color:#f4f4f4;font-size:15px;padding-left:6px;padding-right:6px;font-weight:700;white-space:nowrap;max-width:80%}.button_color[data-v-7bc26671]{color:#0048ff;font-size:15px;padding-left:15px;padding-right:0;text-decoration:underline}.block[data-v-320582f6]{padding:30px 0;text-align:center;border-right:solid 1px var(--el-border-color);flex:1}.block[data-v-320582f6]:last-child{border-right:none}.block .demonstration[data-v-320582f6]{display:block;color:var(--el-text-color-secondary);font-size:14px;margin-bottom:20px}
+.label_color[data-v-0c9eea5d]{color:#333;font-size:15px;padding-left:15px;padding-right:0}.data_color[data-v-0c9eea5d]{color:#08488c;background-color:#f4f4f4;font-size:15px;padding-left:6px;padding-right:6px;font-weight:700;white-space:nowrap;max-width:80%}.button_color[data-v-0c9eea5d]{color:#0048ff;font-size:15px;padding-left:15px;padding-right:0;text-decoration:underline}.block[data-v-320582f6]{padding:30px 0;text-align:center;border-right:solid 1px var(--el-border-color);flex:1}.block[data-v-320582f6]:last-child{border-right:none}.block .demonstration[data-v-320582f6]{display:block;color:var(--el-text-color-secondary);font-size:14px;margin-bottom:20px}
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/DecryptView-j3edNkwI.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/DecryptView-emfcQg74.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     b as v,
     c as f,
     e,
     f as o,
     g as b,
     a as c,
     h as w
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const V = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
         }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/HelpView-8d8K8EDR.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/HelpView-eMRBH9mj.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     d as t,
     b as e,
     c as a,
     A as o
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const r = {
         class: "about"
     },
     b = o('<h1 id="-center-pywxdump-center-" style="text-align:center;"> PyWxDump UserGuide &amp; FAQ </h1><br><br><br><br><br><br><h2 style="text-align:center;"><a href="https://github.com/xaoyaoo/PyWxDump/blob/master/doc/UserGuide.md" target="_blank">使用教程</a><br><a href="https://github.com/xaoyaoo/PyWxDump/blob/master/doc/FAQ.md" target="_blank">常见问题</a><br><a href="https://github.com/xaoyaoo/PyWxDump/blob/master/doc/CE%E8%8E%B7%E5%8F%96%E5%9F%BA%E5%9D%80.md" target="_blank">CE获取基址</a><br><a href="https://github.com/xaoyaoo/PyWxDump/blob/master/doc/wx%E6%95%B0%E6%8D%AE%E5%BA%93%E7%AE%80%E8%BF%B0.md" target="_blank">wx数据库简述</a><br><a href="https://github.com/xaoyaoo/PyWxDump/blob/master/doc/MAC%E6%95%B0%E6%8D%AE%E5%BA%93%E8%A7%A3%E5%AF%86.md" target="_blank">MAC数据库解密</a></h2>', 8),
     s = [b],
     d = t({
         __name: "HelpView",
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/HomeView.vue_vue_type_script_setup_true_lang-5w2dEJdv.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/HomeView.vue_vue_type_script_setup_true_lang-dZI7DIut.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     r as c,
     o as r,
     b as i,
     c as _,
     e as o,
     h as s,
     t as d
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const l = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
         }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/MergeView-R4wK5Hv8.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/MergeView-pn-ejbod.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     b as f,
     c as v,
     e,
     f as o,
     g as y,
     a as u,
     h as b
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const g = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
         }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/StatisticsView-g0EfwdVR.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/StatisticsView-sWS8TEdn.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as s,
     b as o,
     c,
     e,
     h as t
-} from "./index-CtkzF4da.js";
+} from "./index-VdcdRmrH.js";
 const a = {},
     n = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/WxinfoView-dBviDsRz.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/WxinfoView-UlpcKPEi.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -9,17 +9,17 @@
     c as x,
     e as l,
     f as e,
     g as c,
     u as t,
     a as g,
     h as p,
-    v as a,
-    x as C
-} from "./index-CtkzF4da.js";
+    q as a,
+    s as C
+} from "./index-VdcdRmrH.js";
 const k = {
         style: {
             "background-color": "#d2d2fa",
             height: "100vh",
             display: "grid",
             "place-items": "center"
         }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/axios--FnjuHWf.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/axios--FnjuHWf.js`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/index-55UIhNbb.css` & `pywxdump-3.0.8/pywxdump/ui/web/assets/index-55UIhNbb.css`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/assets/index-CtkzF4da.js` & `pywxdump-3.0.8/pywxdump/ui/web/assets/index-VdcdRmrH.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -69221,70 +69221,70 @@
         })
     },
     FJ = bJ({
         history: PZ("./"),
         routes: [{
             path: "/",
             name: "home",
-            component: () => Pa(() => import("./HomeView-DcUxYQHB.js"), __vite__mapDeps([0, 1, 2]), import.meta.url)
+            component: () => Pa(() => import("./HomeView-oLhVq41M.js"), __vite__mapDeps([0, 1, 2]), import.meta.url)
         }, {
             path: "/chat",
             name: "chat",
-            component: () => Pa(() => import("./ChatView-zX7v9ucw.js"), __vite__mapDeps([3, 2, 1, 4, 5]), import.meta.url)
+            component: () => Pa(() => import("./ChatView-PSmCcQTu.js"), __vite__mapDeps([3, 2, 1, 4, 5]), import.meta.url)
         }, {
             path: "/cleanup",
             name: "cleanup",
-            component: () => Pa(() => import("./CleanupView-E355vjQT.js"), __vite__mapDeps([6, 2, 5]), import.meta.url)
+            component: () => Pa(() => import("./CleanupView-JwdNAC7i.js"), __vite__mapDeps([6, 2, 5]), import.meta.url)
         }, {
             path: "/statistics",
             name: "statistics",
-            component: () => Pa(() => import("./StatisticsView-g0EfwdVR.js"), __vite__mapDeps([]), import.meta.url)
+            component: () => Pa(() => import("./StatisticsView-sWS8TEdn.js"), __vite__mapDeps([]), import.meta.url)
         }, {
             path: "/wxinfo",
             name: "wxinfo",
-            component: () => Pa(() => import("./WxinfoView-dBviDsRz.js"), __vite__mapDeps([7, 2]), import.meta.url)
+            component: () => Pa(() => import("./WxinfoView-UlpcKPEi.js"), __vite__mapDeps([7, 2]), import.meta.url)
         }, {
             path: "/bias",
             name: "bias",
-            component: () => Pa(() => import("./BiasView-HrnP52sC.js"), __vite__mapDeps([8, 2]), import.meta.url)
+            component: () => Pa(() => import("./BiasView-8tCrt-Mg.js"), __vite__mapDeps([8, 2]), import.meta.url)
         }, {
             path: "/merge",
             name: "merge",
-            component: () => Pa(() => import("./MergeView-R4wK5Hv8.js"), __vite__mapDeps([9, 2]), import.meta.url)
+            component: () => Pa(() => import("./MergeView-pn-ejbod.js"), __vite__mapDeps([9, 2]), import.meta.url)
         }, {
             path: "/decrypt",
             name: "decrypt",
-            component: () => Pa(() => import("./DecryptView-j3edNkwI.js"), __vite__mapDeps([10, 2]), import.meta.url)
+            component: () => Pa(() => import("./DecryptView-emfcQg74.js"), __vite__mapDeps([10, 2]), import.meta.url)
         }, {
             path: "/about",
             name: "about",
-            component: () => Pa(() => import("./AboutView-Zw8iwR0j.js"), __vite__mapDeps([11, 2]), import.meta.url)
+            component: () => Pa(() => import("./AboutView-YDN8Uqso.js"), __vite__mapDeps([11, 2]), import.meta.url)
         }, {
             path: "/help",
             name: "help",
-            component: () => Pa(() => import("./HelpView-8d8K8EDR.js"), __vite__mapDeps([]), import.meta.url)
+            component: () => Pa(() => import("./HelpView-eMRBH9mj.js"), __vite__mapDeps([]), import.meta.url)
         }, {
             path: "/setting",
             name: "setting",
-            component: () => Pa(() => import("./SettingView-7PdMki0v.js"), __vite__mapDeps([]), import.meta.url)
+            component: () => Pa(() => import("./SettingView-LZJej87E.js"), __vite__mapDeps([]), import.meta.url)
         }]
     }),
     Hr = z_(MJ);
 Hr.use(FJ);
 Hr.use(_Z);
 Hr.use(hZ);
 Hr.provide("msg_path", "");
 Hr.provide("micro_path", "");
 Hr.provide("media_path", "");
 Hr.provide("filestorage_path", "");
 Hr.provide("user_list", []);
 Hr.mount("#app");
 export {
-    cw as A, pZ as E, Ye as F, hZ as M, xJ as _, ot as a, L as b, V as c, X as d, q as e, K as f, ee as g, Ct as h, _e as i, pe as j, _Z as k, Pt as l, Te as m, Tt as n, ut as o, He as p, JX as q, G as r, UX as s, Me as t, m as u, MK as v, It as w, xK as x, st as y, ql as z
+    cw as A, pZ as E, Ye as F, hZ as M, xJ as _, ot as a, L as b, V as c, X as d, q as e, K as f, ee as g, Ct as h, _e as i, pe as j, _Z as k, Pt as l, Te as m, Tt as n, ut as o, He as p, MK as q, G as r, xK as s, Me as t, m as u, st as v, It as w, ql as x, JX as y, UX as z
 };
 
 function __vite__mapDeps(indexes) {
     if (!__vite__mapDeps.viteFileDeps) {
-        __vite__mapDeps.viteFileDeps = ["./HomeView-DcUxYQHB.js", "./HomeView.vue_vue_type_script_setup_true_lang-5w2dEJdv.js", "./axios--FnjuHWf.js", "./ChatView-zX7v9ucw.js", "./ChatView-3ZOUdUTv.css", "./DateTimeSelect-L-ShBE0O.css", "./CleanupView-E355vjQT.js", "./WxinfoView-dBviDsRz.js", "./BiasView-HrnP52sC.js", "./MergeView-R4wK5Hv8.js", "./DecryptView-j3edNkwI.js", "./AboutView-Zw8iwR0j.js"]
+        __vite__mapDeps.viteFileDeps = ["./HomeView-oLhVq41M.js", "./HomeView.vue_vue_type_script_setup_true_lang-dZI7DIut.js", "./axios--FnjuHWf.js", "./ChatView-PSmCcQTu.js", "./ChatView-I_cUSrgs.css", "./DateTimeSelect-_xTa7bZL.css", "./CleanupView-JwdNAC7i.js", "./WxinfoView-UlpcKPEi.js", "./BiasView-8tCrt-Mg.js", "./MergeView-pn-ejbod.js", "./DecryptView-emfcQg74.js", "./AboutView-YDN8Uqso.js"]
     }
     return indexes.map((i) => __vite__mapDeps.viteFileDeps[i])
 }
```

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/favicon.ico` & `pywxdump-3.0.8/pywxdump/ui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/ui/web/index.html` & `pywxdump-3.0.8/pywxdump/ui/web/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     <style>
         html,
         body {
             margin: 0;
             height: 100%;
         }
     </style>
-  <script type="module" crossorigin src="./assets/index-CtkzF4da.js"></script>
+  <script type="module" crossorigin src="./assets/index-VdcdRmrH.js"></script>
   <link rel="stylesheet" crossorigin href="./assets/index-55UIhNbb.css">
 </head>
 <body>
 <div id="app" style="height: 100%;"></div>
 </body>
 </html>
```

### Comparing `pywxdump-3.0.6/pywxdump/version_list.json` & `pywxdump-3.0.8/pywxdump/version_list.json`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/__init__.py` & `pywxdump-3.0.8/pywxdump/wx_info/__init__.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/decryption.py` & `pywxdump-3.0.8/pywxdump/wx_info/decryption.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/get_bias_addr.py` & `pywxdump-3.0.8/pywxdump/wx_info/get_bias_addr.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/get_wx_info.py` & `pywxdump-3.0.8/pywxdump/wx_info/get_wx_info.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/merge_db.py` & `pywxdump-3.0.8/pywxdump/wx_info/merge_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         db.close()
     outdb.close()
     return save_path
 
 
 def decrypt_merge(wx_path, key, outpath="", CreateTime: int = 0, endCreateTime: int = 0) -> (bool, str):
     """
-    解密合并数据库 msg.db, microMsg.db, media.db
+    解密合并数据库 msg.db, microMsg.db, media.db,注意：会删除原数据库
     :param wx_path: 微信路径 eg: C:\*******\WeChat Files\wxid_*********
     :param key: 解密密钥
     :return: (true,解密后的数据库路径) or (false,错误信息)
     """
     from .decryption import batch_decrypt
     from .get_wx_info import get_core_db
```

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/tools/libcrypto-1_1-x64.dll` & `pywxdump-3.0.8/pywxdump/wx_info/tools/libcrypto-1_1-x64.dll`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/tools/realTime.exe` & `pywxdump-3.0.8/pywxdump/wx_info/tools/realTime.exe`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump/wx_info/utils.py` & `pywxdump-3.0.8/pywxdump/wx_info/utils.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/pywxdump.egg-info/PKG-INFO` & `pywxdump-3.0.8/pywxdump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdump
-Version: 3.0.6
+Version: 3.0.8
 Summary: 微信信息获取工具
 Home-page: https://github.com/xaoyaoo/PyWxDump
 Author: xaoyaoo
 Author-email: xaoyaoo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pywxdump-3.0.6/pywxdump.egg-info/SOURCES.txt` & `pywxdump-3.0.8/pywxdump.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,37 +23,40 @@
 pywxdump/dbpreprocess/__init__.py
 pywxdump/dbpreprocess/dbbase.py
 pywxdump/dbpreprocess/parsingMSG.py
 pywxdump/dbpreprocess/parsingMediaMSG.py
 pywxdump/dbpreprocess/parsingMicroMsg.py
 pywxdump/dbpreprocess/parsingOpenIMContact.py
 pywxdump/dbpreprocess/utils.py
+pywxdump/dbpreprocess/export/__init__.py
+pywxdump/dbpreprocess/export/exportCSV.py
+pywxdump/dbpreprocess/export/exportJSON.py
 pywxdump/ui/__init__.py
 pywxdump/ui/view_chat.py
 pywxdump/ui/templates/chat.html
 pywxdump/ui/templates/index.html
 pywxdump/ui/web/favicon.ico
 pywxdump/ui/web/index.html
-pywxdump/ui/web/assets/AboutView-Zw8iwR0j.js
-pywxdump/ui/web/assets/BiasView-HrnP52sC.js
-pywxdump/ui/web/assets/ChatView-3ZOUdUTv.css
-pywxdump/ui/web/assets/ChatView-zX7v9ucw.js
-pywxdump/ui/web/assets/CleanupView-E355vjQT.js
-pywxdump/ui/web/assets/DateTimeSelect-L-ShBE0O.css
-pywxdump/ui/web/assets/DecryptView-j3edNkwI.js
-pywxdump/ui/web/assets/HelpView-8d8K8EDR.js
-pywxdump/ui/web/assets/HomeView-DcUxYQHB.js
-pywxdump/ui/web/assets/HomeView.vue_vue_type_script_setup_true_lang-5w2dEJdv.js
-pywxdump/ui/web/assets/MergeView-R4wK5Hv8.js
-pywxdump/ui/web/assets/SettingView-7PdMki0v.js
-pywxdump/ui/web/assets/StatisticsView-g0EfwdVR.js
-pywxdump/ui/web/assets/WxinfoView-dBviDsRz.js
+pywxdump/ui/web/assets/AboutView-YDN8Uqso.js
+pywxdump/ui/web/assets/BiasView-8tCrt-Mg.js
+pywxdump/ui/web/assets/ChatView-I_cUSrgs.css
+pywxdump/ui/web/assets/ChatView-PSmCcQTu.js
+pywxdump/ui/web/assets/CleanupView-JwdNAC7i.js
+pywxdump/ui/web/assets/DateTimeSelect-_xTa7bZL.css
+pywxdump/ui/web/assets/DecryptView-emfcQg74.js
+pywxdump/ui/web/assets/HelpView-eMRBH9mj.js
+pywxdump/ui/web/assets/HomeView-oLhVq41M.js
+pywxdump/ui/web/assets/HomeView.vue_vue_type_script_setup_true_lang-dZI7DIut.js
+pywxdump/ui/web/assets/MergeView-pn-ejbod.js
+pywxdump/ui/web/assets/SettingView-LZJej87E.js
+pywxdump/ui/web/assets/StatisticsView-sWS8TEdn.js
+pywxdump/ui/web/assets/WxinfoView-UlpcKPEi.js
 pywxdump/ui/web/assets/axios--FnjuHWf.js
 pywxdump/ui/web/assets/index-55UIhNbb.css
-pywxdump/ui/web/assets/index-CtkzF4da.js
+pywxdump/ui/web/assets/index-VdcdRmrH.js
 pywxdump/wx_info/__init__.py
 pywxdump/wx_info/decryption.py
 pywxdump/wx_info/get_bias_addr.py
 pywxdump/wx_info/get_wx_info.py
 pywxdump/wx_info/merge_db.py
 pywxdump/wx_info/utils.py
 pywxdump/wx_info/tools/libcrypto-1_1-x64.dll
```

### Comparing `pywxdump-3.0.6/setup.py` & `pywxdump-3.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,21 +37,22 @@
     description="微信信息获取工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xaoyaoo/PyWxDump",
     license='MIT',
 
     packages=['pywxdump', 'pywxdump.ui', 'pywxdump.wx_info', 'pywxdump.analyzer', 'pywxdump.api',
-              'pywxdump.dbpreprocess'],
+              'pywxdump.dbpreprocess', 'pywxdump.dbpreprocess.export'],
     package_dir={'pywxdump': 'pywxdump',
                  'pywxdump.wx_info': 'pywxdump/wx_info',
                  'pywxdump.analyzer': 'pywxdump/analyzer',
                  'pywxdump.ui': 'pywxdump/ui',
                  'pywxdump.api': 'pywxdump/api',
-                 'pywxdump.dbpreprocess': 'pywxdump/dbpreprocess'
+                 'pywxdump.dbpreprocess': 'pywxdump/dbpreprocess',
+                 'pywxdump.dbpreprocess.export': 'pywxdump/dbpreprocess/export'
                  },
 
     package_data={
         'pywxdump': ['version_list.json', 'ui/templates/*', 'ui/web/*', 'ui/web/assets/*', 'wx_info/tools/*',
                      "ui/export/*", "ui/export/assets/*", "ui/export/assets/css/*", "ui/export/assets/js/*",
                      ]
     },
```

### Comparing `pywxdump-3.0.6/tests/test_Bias.py` & `pywxdump-3.0.8/tests/test_Bias.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/tests/test_dbshow.py` & `pywxdump-3.0.8/tests/test_dbshow.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/tests/test_decrypt.py` & `pywxdump-3.0.8/tests/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `pywxdump-3.0.6/tests/test_read_info.py` & `pywxdump-3.0.8/tests/test_read_info.py`

 * *Files identical despite different names*

