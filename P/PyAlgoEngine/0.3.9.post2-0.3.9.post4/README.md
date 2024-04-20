# Comparing `tmp/PyAlgoEngine-0.3.9.post2.tar.gz` & `tmp/PyAlgoEngine-0.3.9.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlgoEngine-0.3.9.post2.tar", last modified: Fri Jul 14 07:52:30 2023, max compression
+gzip compressed data, was "PyAlgoEngine-0.3.9.post4.tar", last modified: Tue Dec 26 15:01:34 2023, max compression
```

## Comparing `PyAlgoEngine-0.3.9.post2.tar` & `PyAlgoEngine-0.3.9.post4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-14 07:52:30.674513 PyAlgoEngine-0.3.9.post2/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-14 07:52:29.965490 PyAlgoEngine-0.3.9.post2/AlgoEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-14 07:52:30.248058 PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31104 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/AlgoEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1465 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/EventEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    32307 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/MarketEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    80159 2023-07-13 07:54:27.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/TradeEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3653 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-14 07:52:30.468784 PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1814 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/BackTest.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    14977 2023-07-14 07:49:44.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/_StrategyEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1738 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      432 2023-07-14 07:50:55.000000 PyAlgoEngine-0.3.9.post2/AlgoEngine/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      521 2023-07-14 07:52:30.674513 PyAlgoEngine-0.3.9.post2/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-14 07:52:30.642216 PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      521 2023-07-14 07:52:26.000000 PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-07-14 07:52:27.000000 PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-07-14 07:52:26.000000 PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       57 2023-07-14 07:52:26.000000 PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-07-14 07:52:26.000000 PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-07-14 07:52:30.689567 PyAlgoEngine-0.3.9.post2/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1528 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post2/setup.py
+drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/
+drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/AlgoEngine/
+drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/
+-rw-r--r--   0 bolun     (1000) bolun     (1000)    31104 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/AlgoEngine.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)     1465 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/EventEngine.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)    32576 2023-12-26 14:54:56.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/MarketEngine.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)    80159 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/TradeEngine.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)     3653 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/__init__.py
+drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/
+-rw-r--r--   0 bolun     (1000) bolun     (1000)     1814 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/BackTest.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)    14977 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/_StrategyEngine.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)     1738 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/__init__.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)      432 2023-12-26 14:55:20.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/__init__.py
+-rw-r--r--   0 bolun     (1000) bolun     (1000)     1066 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/LICENSE
+-rw-r--r--   0 bolun     (1000) bolun     (1000)      653 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/PKG-INFO
+drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/
+-rw-r--r--   0 bolun     (1000) bolun     (1000)      653 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/PKG-INFO
+-rw-r--r--   0 bolun     (1000) bolun     (1000)      499 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/SOURCES.txt
+-rw-r--r--   0 bolun     (1000) bolun     (1000)        1 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/dependency_links.txt
+-rw-r--r--   0 bolun     (1000) bolun     (1000)       57 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/requires.txt
+-rw-r--r--   0 bolun     (1000) bolun     (1000)       11 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/top_level.txt
+-rw-r--r--   0 bolun     (1000) bolun     (1000)       42 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/README.md
+-rw-r--r--   0 bolun     (1000) bolun     (1000)       38 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/setup.cfg
+-rw-r--r--   0 bolun     (1000) bolun     (1000)     1528 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/setup.py
```

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/AlgoEngine.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/AlgoEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/EventEngine.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/EventEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/MarketEngine.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/MarketEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import abc
 import datetime
 import functools
 import threading
 import uuid
 from collections import defaultdict
+from typing import Iterable
 
 from PyQuantKit import TickData, TradeData, OrderBook, MarketData, Progress, TransactionSide, BarData, TransactionData
 
 from . import LOGGER
 
 __all__ = ['MDS', 'MarketDataService', 'MarketDataMonitor', 'SyntheticOrderBookMonitor', 'MinuteBarMonitor', 'Profile', 'ProgressiveReplay', 'SimpleReplay', 'Replay']
 LOGGER = LOGGER.getChild('MarketEngine')
@@ -35,17 +36,20 @@
         self.name = name
         self.monitor_id = uuid.uuid4().hex if monitor_id is None else monitor_id
         self.mds = MDS if mds is None else mds
 
     @abc.abstractmethod
     def __call__(self, market_data: MarketData, **kwargs): ...
 
+    @abc.abstractmethod
+    def clear(self) -> None: ...
+
     @property
     @abc.abstractmethod
-    def value(self): ...
+    def value(self) -> dict[str, float] | float: ...
 
     @property
     @abc.abstractmethod
     def is_ready(self) -> bool: ...
 
 
 class SyntheticOrderBookMonitor(MarketDataMonitor):
@@ -554,15 +558,15 @@
             if monitor is None:
                 continue
 
             monitor.__call__(market_data)
 
         self.lock.release()
 
-    def get_order_book(self, ticker: str) -> OrderBook:
+    def get_order_book(self, ticker: str) -> OrderBook | None:
         return self._order_book.get(ticker, None)
 
     def get_queued_volume(self, ticker: str, side: TransactionSide | str | int, prior: float, posterior: float = None) -> float:
         """
         get queued volume prior / posterior to given price, NOT COUNTING GIVEN PRICE!
         :param ticker: the given ticker
         :param side: the given trade side
@@ -751,36 +755,40 @@
 
     def __init__(
             self,
             loader,
             **kwargs
     ):
         self.loader = loader
-        self.start_date: datetime.date = kwargs.pop('start_date', None)
-        self.end_date: datetime.date = kwargs.pop('end_date', None)
-        self.calendar: list[datetime.date] = kwargs.pop('calendar', None)
+        self.start_date: datetime.date | None = kwargs.pop('start_date', None)
+        self.end_date: datetime.date | None = kwargs.pop('end_date', None)
+        self.calendar: list[datetime.date] | None = kwargs.pop('calendar', None)
 
         self.eod = kwargs.pop('eod', None)
         self.bod = kwargs.pop('bod', None)
 
         self.replay_subscription = {}
         self.replay_calendar = []
         self.replay_task = []
 
         self.date_progress = 0
         self.task_progress = 0
         self.progress = Progress(tasks=1, **kwargs)
 
-        tickers = kwargs.pop('ticker', kwargs.pop('tickers', []))
-        dtypes = kwargs.pop('dtype', kwargs.pop('dtypes', [TradeData, OrderBook, TickData]))
+        tickers: list[str] = kwargs.pop('ticker', kwargs.pop('tickers', []))
+        dtypes: list[str | type] = kwargs.pop('dtype', kwargs.pop('dtypes', [TradeData, OrderBook, TickData]))
 
-        if not isinstance(tickers, list):
+        if isinstance(tickers, Iterable):
+            tickers = list(tickers)
+        else:
             tickers = [tickers]
 
-        if not isinstance(dtypes, list):
+        if isinstance(dtypes, Iterable):
+            dtypes = list(dtypes)
+        else:
             dtypes = [dtypes]
 
         for ticker in tickers:
             for dtype in dtypes:
                 self.add_subscription(ticker=ticker, dtype=dtype)
 
         subscription = kwargs.pop('subscription', kwargs.pop('subscribe', []))
```

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/TradeEngine.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/TradeEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Engine/__init__.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/BackTest.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/BackTest.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/_StrategyEngine.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/_StrategyEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/AlgoEngine/Strategies/__init__.py` & `PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/LICENSE` & `PyAlgoEngine-0.3.9.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post2/PKG-INFO` & `PyAlgoEngine-0.3.9.post4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.9.post2
+Version: 0.3.9.post4
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: exchange_calendars
+Requires-Dist: PyQuantKit
+Requires-Dist: PyEventEngine
 
 # PyAlgoEngine
 python algo trading engine
```

### Comparing `PyAlgoEngine-0.3.9.post2/PyAlgoEngine.egg-info/PKG-INFO` & `PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.9.post2
+Version: 0.3.9.post4
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: exchange_calendars
+Requires-Dist: PyQuantKit
+Requires-Dist: PyEventEngine
 
 # PyAlgoEngine
 python algo trading engine
```

### Comparing `PyAlgoEngine-0.3.9.post2/setup.py` & `PyAlgoEngine-0.3.9.post4/setup.py`

 * *Files identical despite different names*

