# Comparing `tmp/PaifuLogger-0.4.0.1.tar.gz` & `tmp/paifulogger-0.4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaifuLogger-0.4.0.1.tar", last modified: Sat Apr 13 09:54:41 2024, max compression
+gzip compressed data, was "paifulogger-0.4.0.2.tar", last modified: Sat Apr 20 12:41:46 2024, max compression
```

## Comparing `PaifuLogger-0.4.0.1.tar` & `paifulogger-0.4.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-13 09:54:41.000000 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-13 09:54:41.000000 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:54:41.000000 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-13 09:54:41.000000 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 09:54:41.000000 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 09:54:41.000000 PaifuLogger-0.4.0.1/PaifuLogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.202942 PaifuLogger-0.4.0.1/paifulogger/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.202942 PaifuLogger-0.4.0.1/paifulogger/localizations/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/localizations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/localizations/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/localizations/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/localizations/zh_tw.json
--rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/paifu_dl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/paifulogger/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/Paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/get_paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/log_into_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/log_into_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/log_into_xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/paifulogger/src/mjlog2mjai/
--rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-13 09:54:37.000000 PaifuLogger-0.4.0.1/paifulogger/src/mjlog2mjai/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-13 09:54:37.000000 PaifuLogger-0.4.0.1/paifulogger/src/mjlog2mjai/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/src/url_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/paifulogger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/pub_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/pub_tools/pub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:41.206941 PaifuLogger-0.4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-13 09:54:36.000000 PaifuLogger-0.4.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/PaifuLogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.872611 paifulogger-0.4.0.2/paifulogger/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/paifulogger/localizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/zh_tw.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/paifu_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/paifulogger/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/Paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/get_paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/log_into_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/log_into_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/log_into_xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/url_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/pub_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/pub_tools/pub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/test/test.py
```

### Comparing `PaifuLogger-0.4.0.1/LICENSE` & `paifulogger-0.4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/PKG-INFO` & `paifulogger-0.4.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.4.0.1
+Version: 0.4.0.2
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
         Copyright (c) 2023-2024 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -58,46 +58,76 @@
 
 ```
 pip install PaifuLogger==0.3.7.1
 ```
 
 ## Usage
 
+### Command Line / Script
+
 1. Download the project.
 
-> a. Download from github.
+> a. Via GitHub.
 >
 >> i. Clone the repository or download the [latest release](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest).
 >>
 >> ```
 >> git clone https://github.com/Jim137/Tenhou-Paifu-Logger.git
 >> ```
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard.
 >>
->> iii. Open `runlog-user.bat` or `runlog-user.sh`.
+>> iii. Run `runlog-user.bat` or `runlog-user.sh`.
 >
-> b. Download from pypi.
+> b. Via pypi.
 >
->> i. Open command line and type
+>> i. Open terminal and install with pip command.
 >>
 >> ```
 >> pip install PaifuLogger
 >> ```
 >>
->> ii. Copy the paifu URL from tenhou.net to clipboard. And type
+>> ii. Copy the paifu URL from tenhou.net to clipboard. And run by
 >>
->> ```
+>> ```shell
 >> plog -l [language] -o [output directory] [paifu URLs]
 >> ```
+>> ```shell
+>> paifulogger plog -l [language] -o [output directory] [paifu URLs]
+>> ```
 
-2. Once ![1675261153312](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/README/1675261153312.png) appears, paste the paifu URL and press Enter.\
+2. Once `Please enter the URL of match:` appears, paste the URL and press Enter.\
 Note: In the latest version, you can input multiple URLs at once, separated by whatever you like. If you are lazy, you can just paste w/o anything.
-3. After ![1675264143738](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/README/1675264143738.png) appears, the paifu is successfully logged.
-4. When ![1675261153312](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/README/1675261153312.png) appears again, you can paste the next the URL.
+3. After `Match of {paifu name} has been recorded` appears, the paifu has been successfully logged.
+
+### Inline
+
+You can manually log the paifu by the following code.
+
+```python
+from paifulogger import get_paifu, localized_str, log_paifu, main_path
+from paifulogger.log import _get_log_func
+
+url = "Your paifu URL"
+local_lang = localized_str("en", main_path) # Localization
+log_formats = _get_log_func(["csv", "html"]) # Log into csv and html file.
+output = "./" # Output directory
+mjai = False # Whether have output in mjai format
+
+# Log the paifu into the file.
+log_paifu(
+    url,
+    log_formats = log_formats,
+    local_lang = local_lang,
+    output = output,
+    mjai = mjai
+)
+# Get Paifu object, which contains all the information of the paifu.
+paifu = get_paifu(url, local_lang)
+```
 
 ## Features
 * [x] Support multiple URLs at once.
 * [x] Log paifu into excel, csv or html file with some key information. (-f, --format)
 * [x] Support logging to multiple formats at once. (e.g.: -f csv -f html; -a, --all-formats)
 * [x] Distinguish Sanma(3p) and Yonma(4p) and log into separate sheets.
 * [x] Skip duplicated paifu
@@ -134,8 +164,8 @@
 ## Contribute
 We welcome all kinds of contributions, including but not limited to bug reports, pull requests, feature requests, documentation improvements, localizations...etc.
 
 See [CONTRIBUTING.md](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/CONTRIBUTING.md) for more details.
 
 ## License
 
-[MIT](LICENSE)
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PaifuLogger-0.4.0.1/PaifuLogger.egg-info/PKG-INFO` & `paifulogger-0.4.0.2/PaifuLogger.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.4.0.1
+Version: 0.4.0.2
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
         Copyright (c) 2023-2024 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -58,46 +58,76 @@
 
 ```
 pip install PaifuLogger==0.3.7.1
 ```
 
 ## Usage
 
+### Command Line / Script
+
 1. Download the project.
 
-> a. Download from github.
+> a. Via GitHub.
 >
 >> i. Clone the repository or download the [latest release](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest).
 >>
 >> ```
 >> git clone https://github.com/Jim137/Tenhou-Paifu-Logger.git
 >> ```
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard.
 >>
->> iii. Open `runlog-user.bat` or `runlog-user.sh`.
+>> iii. Run `runlog-user.bat` or `runlog-user.sh`.
 >
-> b. Download from pypi.
+> b. Via pypi.
 >
->> i. Open command line and type
+>> i. Open terminal and install with pip command.
 >>
 >> ```
 >> pip install PaifuLogger
 >> ```
 >>
->> ii. Copy the paifu URL from tenhou.net to clipboard. And type
+>> ii. Copy the paifu URL from tenhou.net to clipboard. And run by
 >>
->> ```
+>> ```shell
 >> plog -l [language] -o [output directory] [paifu URLs]
 >> ```
+>> ```shell
+>> paifulogger plog -l [language] -o [output directory] [paifu URLs]
+>> ```
 
-2. Once ![1675261153312](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/README/1675261153312.png) appears, paste the paifu URL and press Enter.\
+2. Once `Please enter the URL of match:` appears, paste the URL and press Enter.\
 Note: In the latest version, you can input multiple URLs at once, separated by whatever you like. If you are lazy, you can just paste w/o anything.
-3. After ![1675264143738](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/README/1675264143738.png) appears, the paifu is successfully logged.
-4. When ![1675261153312](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/README/1675261153312.png) appears again, you can paste the next the URL.
+3. After `Match of {paifu name} has been recorded` appears, the paifu has been successfully logged.
+
+### Inline
+
+You can manually log the paifu by the following code.
+
+```python
+from paifulogger import get_paifu, localized_str, log_paifu, main_path
+from paifulogger.log import _get_log_func
+
+url = "Your paifu URL"
+local_lang = localized_str("en", main_path) # Localization
+log_formats = _get_log_func(["csv", "html"]) # Log into csv and html file.
+output = "./" # Output directory
+mjai = False # Whether have output in mjai format
+
+# Log the paifu into the file.
+log_paifu(
+    url,
+    log_formats = log_formats,
+    local_lang = local_lang,
+    output = output,
+    mjai = mjai
+)
+# Get Paifu object, which contains all the information of the paifu.
+paifu = get_paifu(url, local_lang)
+```
 
 ## Features
 * [x] Support multiple URLs at once.
 * [x] Log paifu into excel, csv or html file with some key information. (-f, --format)
 * [x] Support logging to multiple formats at once. (e.g.: -f csv -f html; -a, --all-formats)
 * [x] Distinguish Sanma(3p) and Yonma(4p) and log into separate sheets.
 * [x] Skip duplicated paifu
@@ -134,8 +164,8 @@
 ## Contribute
 We welcome all kinds of contributions, including but not limited to bug reports, pull requests, feature requests, documentation improvements, localizations...etc.
 
 See [CONTRIBUTING.md](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/CONTRIBUTING.md) for more details.
 
 ## License
 
-[MIT](LICENSE)
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PaifuLogger-0.4.0.1/PaifuLogger.egg-info/SOURCES.txt` & `paifulogger-0.4.0.2/PaifuLogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/localizations/en.json` & `paifulogger-0.4.0.2/paifulogger/localizations/en.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/localizations/ja.json` & `paifulogger-0.4.0.2/paifulogger/localizations/ja.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/localizations/zh.json` & `paifulogger-0.4.0.2/paifulogger/localizations/zh.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/localizations/zh_tw.json` & `paifulogger-0.4.0.2/paifulogger/localizations/zh_tw.json`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/log.py` & `paifulogger-0.4.0.2/paifulogger/log.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/paifu_dl.py` & `paifulogger-0.4.0.2/paifulogger/paifu_dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     return retCode
 
 
 def pdl(args: argparse.Namespace) -> int:
     if args.version:
         from .version import __version__
 
-        print(f"PaifuLogger version {__version__}")
+        print("Tenhou-Paifu-Logger", __version__)
         return 0
 
     local_lang = _get_lang(args.lang)
 
     return paifu_dl(
         args.url,
         local_lang=local_lang,
```

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/Paifu.py` & `paifulogger-0.4.0.2/paifulogger/src/Paifu.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/get_paifu.py` & `paifulogger-0.4.0.2/paifulogger/src/get_paifu.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/i18n.py` & `paifulogger-0.4.0.2/paifulogger/src/i18n.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/log_into_csv.py` & `paifulogger-0.4.0.2/paifulogger/src/log_into_csv.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/log_into_html.py` & `paifulogger-0.4.0.2/paifulogger/src/log_into_html.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/log_into_xlsx.py` & `paifulogger-0.4.0.2/paifulogger/src/log_into_xlsx.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/mjlog2mjai/parse.py` & `paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/parse.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/mjlog2mjai/test.py` & `paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/test.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/paifulogger/src/url_log.py` & `paifulogger-0.4.0.2/paifulogger/src/url_log.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/pub_tools/pub.py` & `paifulogger-0.4.0.2/pub_tools/pub.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.4.0.1/pyproject.toml` & `paifulogger-0.4.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PaifuLogger"
-version = "0.4.0.1"
+version = "0.4.0.2"
 description = "Logging tenhou paifu into excel or html file with some key information."
 readme = "README.md"
 authors = [{ name = "Jim137", email = "jim@mail.jim137.eu.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
```

### Comparing `PaifuLogger-0.4.0.1/test/test.py` & `paifulogger-0.4.0.2/test/test.py`

 * *Files identical despite different names*

