# Comparing `tmp/pkscreener-0.44.20240419.279.tar.gz` & `tmp/pkscreener-0.44.20240419.280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240419.279.tar", last modified: Fri Apr 19 20:06:29 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240419.280.tar", last modified: Fri Apr 19 21:27:11 2024, max compression
```

## Comparing `pkscreener-0.44.20240419.279.tar` & `pkscreener-0.44.20240419.280.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/
--rw-rw-rw-   0        0        0     1086 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.693153 pkscreener-0.44.20240419.279/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25094 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     6185 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29416 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17603 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   111467 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46418 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79118 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-19 20:06:21.000000 pkscreener-0.44.20240419.279/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   118637 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47947 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    21899 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.693153 pkscreener-0.44.20240419.279/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/
+-rw-rw-rw-   0        0        0     1086 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.347669 pkscreener-0.44.20240419.280/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25094 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     6185 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29416 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17734 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   111467 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46418 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79118 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-19 21:27:04.000000 pkscreener-0.44.20240419.280/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   119023 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47947 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    22164 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.347669 pkscreener-0.44.20240419.280/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/setup.py
```

### Comparing `pkscreener-0.44.20240419.279/LICENSE` & `pkscreener-0.44.20240419.280/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/LICENSE-Others` & `pkscreener-0.44.20240419.280/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/PKG-INFO` & `pkscreener-0.44.20240419.280/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240419.279
+Version: 0.44.20240419.280
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.279.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.280.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240419.279/README.md` & `pkscreener-0.44.20240419.280/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240419.279/pkscreener/__init__.py` & `pkscreener-0.44.20240419.280/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PKScanRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,19 @@
                     if sys.platform.startswith("win"):
                         import signal
 
                         signal.signal(signal.SIGBREAK, PKScanRunner.shutdown)
                         sleep(1)
                     # worker.join()  # necessary so that the Process exists before the test suite exits (thus coverage is collected)
                 # else:
+                # try:
+                    # while worker.is_alive():
                 worker.terminate()
+                # except:
+                #     continue
             except OSError as e: # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 # if e.winerror == 5:
                 continue
 
         # Flush the queue so depending processes will end
         while True:
```

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/classes/keys.py` & `pkscreener-0.44.20240419.280/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/courbd.ttf` & `pkscreener-0.44.20240419.280/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/globals.py` & `pkscreener-0.44.20240419.280/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -605,14 +605,17 @@
             },
             inplace=True,
         )
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
     return screenResults, saveResults
 
+def isInterrupted():
+    global keyboardInterruptEventFired
+    return keyboardInterruptEventFired
 
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
     global screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDict, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
     start_time = 0
@@ -624,14 +627,16 @@
     defaultAnswer = None if userArgs is None else userArgs.answerdefault
     userPassedArgs = userArgs
     options = []
     strategyFilter=[]
     screenCounter = multiprocessing.Value("i", 1)
     screenResultsCounter = multiprocessing.Value("i", 0)
     keyboardInterruptEvent = multiprocessing.Manager().Event()
+    if keyboardInterruptEventFired:
+        return None, None
     keyboardInterruptEventFired = False
     if stockDict is None:
         stockDict = multiprocessing.Manager().dict()
         loadCount = 0
     endOfdayCandles = None
     minRSI = 0
     maxRSI = 100
@@ -658,15 +663,15 @@
             indexOption=indexOption,
             executeOption=executeOption,
             defaultAnswer=defaultAnswer,
             user=user,
         )
 
         if menuOption in ["H", "U", "T", "E", "Y"]:
-            return
+            return None, None
     elif menuOption in ["B", "G"]:
         # Backtests
         backtestPeriod = 0
         if len(options) >= 2:
             if str(indexOption).isnumeric():
                 backtestPeriod = int(indexOption)
             if len(options) >= 4:
@@ -706,18 +711,18 @@
                 pass
             except Exception as e:# pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 pass
         userOption = userOption.upper()
         if userOption == "M":
                 # Go back to the caller. It will show the console menu again.
-                return
+                return None, None
         elif userOption == "Z":
             handleExitRequest(userOption)
-            return
+            return None, None
         
         if userOption == "S":
             OutputControls().printOutput(
                 colorText.GREEN
                 + "[+] Collecting all metrics for summarising..."
                 + colorText.END
             )
@@ -740,15 +745,15 @@
                 )
             else:
                 OutputControls().printOutput("[!] Nothing to show here yet. Check back later.")
             # reinstate whatever was the earlier saved value
             configManager.showPastStrategyData = savedValue
             if defaultAnswer is None:
                 input("Press <Enter> to continue...")
-            return
+            return None, None
         else:
             userOptions = userOption.split(",")
             for usrOption in userOptions:
                 strategyFilter.append(m1.find(usrOption).menuText.strip())
             menuOption, indexOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,
             downloadOnly,
@@ -759,20 +764,20 @@
             defaultAnswer=defaultAnswer,
             user=user,
         )
 
     else:
         OutputControls().printOutput("Not implemented yet! Try selecting a different option.")
         sleep(3)
-        return
+        return None, None
 
     handleMenu_XBG(menuOption, indexOption, executeOption)
     if indexOption == "M" or executeOption == "M":
         # Go back to the caller. It will show the console menu again.
-        return
+        return None, None
     listStockCodes = handleRequestForSpecificStocks(options, indexOption)
     handleExitRequest(executeOption)
     if executeOption is None:
         executeOption = 0
     executeOption = int(executeOption)
     volumeRatio = configManager.volumeRatio
     if executeOption == 3:
@@ -795,15 +800,15 @@
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Error: Invalid values for RSI! Values should be in range of 0 to 100. Please try again!"
                 + colorText.END
             )
             input("PRess <Enter> to continue...")
-            return
+            return None, None
     if executeOption == 6:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             reversalOption = int(options[3])
             if reversalOption in [4, 6, 7, 10]:
                 if len(options) >= 5:
                     if str(options[4]).isnumeric():
@@ -818,15 +823,15 @@
                         selectedMenu
                     )
         else:
             reversalOption, maLength = Utility.tools.promptReversalScreening(
                 selectedMenu
             )
         if reversalOption is None or reversalOption == 0 or maLength == 0:
-            return
+            return None, None
         else:
             selectedChoice["3"] = str(reversalOption)
             if str(reversalOption) in ["7", "10"]:
                 selectedChoice["4"] = str(maLength)
     if executeOption == 7:
         selectedMenu = m2.find(str(executeOption))
         maLength = 0
@@ -881,15 +886,15 @@
                 maLength = Utility.tools.promptChartPatternSubMenu(selectedMenu, respChartPattern)
         if (
             respChartPattern is None
             or insideBarToLookback is None
             or respChartPattern == 0
             or (maLength == 0 and respChartPattern in [1, 2, 3, 6])
         ):
-            return
+            return None, None
         else:
             selectedChoice["3"] = str(respChartPattern)
             selectedChoice["4"] = str(maLength)
     if executeOption == 8:
         if len(options) >= 5:
             if "".join(str(options[3]).split(".")).isdecimal():
                 minRSI = int(options[3])
@@ -904,15 +909,15 @@
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Error: Invalid values for CCI! Values should be in range of -300 to 500. Please try again!"
                 + colorText.END
             )
             input("Press <Enter> to continue...")
-            return
+            return None, None
     if executeOption == 9:
         if len(options) >= 4:
             if str(options[3]).isnumeric():
                 volumeRatio = float(options[3])
             elif str(options[3]).upper() == "D":
                 volumeRatio = configManager.volumeRatio
         else:
@@ -921,29 +926,29 @@
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Error: Invalid values for Volume Ratio! Value should be a positive number. Please try again!"
                 + colorText.END
             )
             input("Press <Enter> to continue...")
-            return
+            return None, None
         else:
             configManager.volumeRatio = float(volumeRatio)
     if executeOption == 12:
         configManager.toggleConfig(candleDuration="15m")
     if executeOption == 21:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             popOption = int(options[3])
             if popOption >= 0 and popOption <= 9:
                 pass
         else:
             popOption = Utility.tools.promptSubMenuOptions(selectedMenu)
         if popOption is None or popOption == 0:
-            return
+            return None, None
         else:
             selectedChoice["3"] = str(popOption)
         if popOption in [1,2,4]:
             updateMenuChoiceHierarchy()
             if popOption == 4:
                 screenResults = mstarFetcher.fetchMorningstarTopDividendsYieldStocks()
             elif popOption in [1,2]:
@@ -957,30 +962,30 @@
                     selectedChoice,
                     menuChoiceHierarchy,
                     False,
                     None,
                 )
                 if defaultAnswer is None:
                     input("Press <Enter> to continue...")
-                return
+                return None, None
             else:
                 listStockCodes = ",".join(list(screenResults.index))
         else:
             userPassedArgs.maxdisplayresults = 2000 # force evaluate all stocks before getting the top results
             reversalOption = popOption
     if executeOption == 22:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             popOption = int(options[3])
             if popOption >= 0 and popOption <= 3:
                 pass
         else:
             popOption = Utility.tools.promptSubMenuOptions(selectedMenu)
         if popOption is None or popOption == 0:
-            return
+            return None, None
         else:
             selectedChoice["3"] = str(popOption)
         updateMenuChoiceHierarchy()
         screenResults = mstarFetcher.fetchMorningstarStocksPerformanceForExchange()
         if menuOption in ["X"]:
             printNotifySaveScreenedResults(
                 screenResults,
@@ -988,38 +993,38 @@
                 selectedChoice,
                 menuChoiceHierarchy,
                 False,
                 None,
             )
             if defaultAnswer is None:
                 input("Press <Enter> to continue...")
-            return
+            return None, None
         else:
             listStockCodes = ",".join(list(screenResults.index))
     if executeOption == 26:
         dividend_df, bonus_df, stockSplit_df = mstarFetcher.getCorporateActions()
         ca_dfs = [dividend_df, bonus_df, stockSplit_df]
         listStockCodes = []
         for df in ca_dfs:
             df = df[
                 df["Stock"].astype(str).str.contains("BSE:") == False
             ]
             listStockCodes.extend(list(df["Stock"]))
     if executeOption == 42:
         Utility.tools.getLastScreenedResults(defaultAnswer)
-        return
+        return None, None
     if executeOption >= 27 and executeOption <= 41:
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "\n[+] Error: Option 25 to 41 Not implemented yet! Press <Enter> to continue."
             + colorText.END
         )
         input("Press <Enter> to continue...")
-        return
+        return None, None
     if (
         not str(indexOption).isnumeric() and indexOption in ["W", "E", "M", "N", "Z"]
     ) or (
         str(indexOption).isnumeric()
         and (int(indexOption) >= 0 and int(indexOption) < 16)
     ):
         configManager.getConfig(ConfigManager.parser)
@@ -1052,17 +1057,17 @@
                     pass
                 sendMessageToTelegramChannel(
                     message=f"{Utility.tools.removeAllColorStyles(Utility.marketStatus())}\nNifty AI prediction for the Next Day: {pText}. {sText}.{warningText}",
                     user=user,
                 )
                 if defaultAnswer is None:
                     input("\nPress <Enter> to Continue...\n")
-                return
+                return None, None
             elif indexOption == "M":
-                return
+                return None, None
             elif indexOption == "Z":
                 input(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Press <Enter> to Exit!"
                     + colorText.END
                 )
@@ -1070,15 +1075,15 @@
             elif indexOption == "E":
                 return handleMonitorFiveEMA()
             else:
                 if str(menuOption).upper() == "C":
                     stockDict,endOfdayCandles = PKMarketOpenCloseAnalyser.getStockDataForSimulation()
                     if stockDict is None or endOfdayCandles is None:
                         OutputControls().printOutput(f"Cannot proceed! Stock data is unavailable. Please check the error logs/messages !")
-                        return
+                        return None, None
                     listStockCodes = sorted(list(filter(None,list(set(stockDict.keys())))))
                 listStockCodes = prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption)
         except urllib.error.URLError as e:
             default_logger().debug(e, exc_info=True)
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
```

### Comparing `pkscreener-0.44.20240419.279/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240419.280/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240419.280/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240419.280/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy
+    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
@@ -298,14 +298,16 @@
         import pandas as pd
         # Delete any existing data from the previous run.
         configManager.deleteFileWithPattern(pattern="stock_data_*.pkl")
         for runOption in runOptions:
             args.options = runOption
             try:
                 optionalFinalOutcome_df,_ = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
+                if isInterrupted():
+                    break
             except Exception as e:
                 OutputControls().printOutput(e)
                 if args.log:
                     import traceback
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
@@ -365,15 +367,19 @@
                     # We need to pipe the output from previous run into the next one
                     if resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
                 args.options = monitorOption
             try:
                 results, plainResults = main(userArgs=args)
-            except:
+                if isInterrupted():
+                    sys.exit(0)
+            except SystemExit:
+                sys.exit(0)
+            except Exception:
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 resultStocks = plainResults.index
             if results is not None and args.monitor and len(monitorOption_org) > 0:
                 MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy())
 
@@ -476,14 +482,16 @@
             if shouldBreak:
                 break
             runLoopOnScheduleOrStdApplication(hasCronInterval)
         if args.v:
             disableSysOut(disable=False)
             return
         sys.exit(0)
+    except SystemExit:
+        sys.exit(0)
     except (RuntimeError, Exception) as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         if args.prodbuild:
             disableSysOut(disable=False)
         OutputControls().printOutput(
             f"{e}\n[+] An error occurred! Please run with '-l' option to collect the logs.\n[+] For example, 'pkscreener -l' and then contact the developer!"
         )
```

### Comparing `pkscreener-0.44.20240419.279/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240419.280/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240419.279
+Version: 0.44.20240419.280
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.279.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.280.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240419.279/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240419.280/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.279/setup.py` & `pkscreener-0.44.20240419.280/setup.py`

 * *Files identical despite different names*

