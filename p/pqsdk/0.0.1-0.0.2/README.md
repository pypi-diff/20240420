# Comparing `tmp/pqsdk-0.0.1.tar.gz` & `tmp/pqsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqsdk-0.0.1.tar", last modified: Fri Apr 12 14:05:25 2024, max compression
+gzip compressed data, was "pqsdk-0.0.2.tar", last modified: Sat Apr 20 11:59:59 2024, max compression
```

## Comparing `pqsdk-0.0.1.tar` & `pqsdk-0.0.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.734522 pqsdk-0.0.1/
--rw-rw-rw-   0        0        0      766 2024-04-12 14:05:25.733523 pqsdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.703003 pqsdk-0.0.1/pqsdk/
--rw-rw-rw-   0        0        0      169 2024-04-12 13:30:06.000000 pqsdk-0.0.1/pqsdk/__init__.py
--rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.1/pqsdk/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.715522 pqsdk-0.0.1/pqsdk/api/
--rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.1/pqsdk/api/__init__.py
--rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.1/pqsdk/api/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.721521 pqsdk-0.0.1/pqsdk/backtest/
--rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.1/pqsdk/backtest/__init__.py
--rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/backtest/analyzer.py
--rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/backtest/context.py
--rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/backtest/current_data.py
--rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/backtest/instrument.py
--rw-rw-rw-   0        0        0    13324 2024-04-10 04:41:02.000000 pqsdk-0.0.1/pqsdk/backtest/main.py
--rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.1/pqsdk/backtest/order.py
--rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/backtest/portfolio.py
--rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/backtest/position.py
--rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/backtest/run_info.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.722522 pqsdk-0.0.1/pqsdk/enums/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/enums/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.1/pqsdk/enums/orderStatus.py
--rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/faxconstant.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.728522 pqsdk-0.0.1/pqsdk/interface/
--rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/__init__.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/abstractInstrument.py
--rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.1/pqsdk/interface/abstractOrder.py
--rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/abstractPortfolio.py
--rw-rw-rw-   0        0        0     1677 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/abstractPosition.py
--rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/abstractRunInfo.py
--rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/abstractStrategyContext.py
--rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/interface/abstractTrader.py
--rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.1/pqsdk/interface/constant.py
--rw-rw-rw-   0        0        0     3520 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/logger.py
--rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.1/pqsdk/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.731522 pqsdk-0.0.1/pqsdk/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/utils/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/utils/dynamic_import.py
--rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/utils/file_util.py
--rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/utils/import_global_modules.py
--rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.1/pqsdk/utils/timer_factory.py
--rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.1/pqsdk/utils/value_type_util.py
--rw-rw-rw-   0        0        0      441 2024-04-12 14:05:13.000000 pqsdk-0.0.1/pqsdk/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.714522 pqsdk-0.0.1/pqsdk.egg-info/
--rw-rw-rw-   0        0        0      766 2024-04-12 14:05:25.000000 pqsdk-0.0.1/pqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2024-04-12 14:05:25.000000 pqsdk-0.0.1/pqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:05:25.000000 pqsdk-0.0.1/pqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-12 14:05:25.000000 pqsdk-0.0.1/pqsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      183 2024-04-12 14:05:25.000000 pqsdk-0.0.1/pqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 14:05:25.000000 pqsdk-0.0.1/pqsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 14:05:25.734522 pqsdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1604 2024-04-08 09:16:06.000000 pqsdk-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:25.732522 pqsdk-0.0.1/tests/
--rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.1/tests/test_backtest.py
--rw-rw-rw-   0        0        0     2059 2024-04-10 03:10:26.000000 pqsdk-0.0.1/tests/test_pqsdk_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.651836 pqsdk-0.0.2/
+-rw-rw-rw-   0        0        0      766 2024-04-20 11:59:59.650837 pqsdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.520871 pqsdk-0.0.2/pqsdk/
+-rw-rw-rw-   0        0        0      169 2024-04-12 13:30:06.000000 pqsdk-0.0.2/pqsdk/__init__.py
+-rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.2/pqsdk/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.546604 pqsdk-0.0.2/pqsdk/api/
+-rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.2/pqsdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.2/pqsdk/api/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.586629 pqsdk-0.0.2/pqsdk/backtest/
+-rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.2/pqsdk/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/backtest/analyzer.py
+-rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/backtest/context.py
+-rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/backtest/current_data.py
+-rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/backtest/instrument.py
+-rw-rw-rw-   0        0        0    13963 2024-04-20 11:54:44.000000 pqsdk-0.0.2/pqsdk/backtest/main.py
+-rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.2/pqsdk/backtest/order.py
+-rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/backtest/portfolio.py
+-rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/backtest/position.py
+-rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/backtest/run_info.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.590644 pqsdk-0.0.2/pqsdk/enums/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.2/pqsdk/enums/orderStatus.py
+-rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/faxconstant.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.628835 pqsdk-0.0.2/pqsdk/interface/
+-rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/abstractInstrument.py
+-rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.2/pqsdk/interface/abstractOrder.py
+-rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/abstractPortfolio.py
+-rw-rw-rw-   0        0        0     1677 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/abstractPosition.py
+-rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/abstractRunInfo.py
+-rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/abstractStrategyContext.py
+-rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/interface/abstractTrader.py
+-rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.2/pqsdk/interface/constant.py
+-rw-rw-rw-   0        0        0     3520 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/logger.py
+-rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.2/pqsdk/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.648836 pqsdk-0.0.2/pqsdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/utils/dynamic_import.py
+-rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/utils/file_util.py
+-rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/utils/import_global_modules.py
+-rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.2/pqsdk/utils/timer_factory.py
+-rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.2/pqsdk/utils/value_type_util.py
+-rw-rw-rw-   0        0        0      441 2024-04-12 14:05:13.000000 pqsdk-0.0.2/pqsdk/version.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.650837 pqsdk-0.0.2/pqsdk.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-04-20 11:59:59.000000 pqsdk-0.0.2/pqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2024-04-20 11:59:59.000000 pqsdk-0.0.2/pqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 11:59:59.000000 pqsdk-0.0.2/pqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-20 11:59:59.000000 pqsdk-0.0.2/pqsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2024-04-20 11:59:59.000000 pqsdk-0.0.2/pqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 11:59:59.000000 pqsdk-0.0.2/pqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 11:59:59.651836 pqsdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:59:59.649837 pqsdk-0.0.2/tests/
+-rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.2/tests/test_backtest.py
+-rw-rw-rw-   0        0        0     2059 2024-04-10 03:10:26.000000 pqsdk-0.0.2/tests/test_pqsdk_api.py
```

### Comparing `pqsdk-0.0.1/PKG-INFO` & `pqsdk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.1/pqsdk/__main__.py` & `pqsdk-0.0.2/pqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/api/__init__.py` & `pqsdk-0.0.2/pqsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/api/main.py` & `pqsdk-0.0.2/pqsdk/api/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/__init__.py` & `pqsdk-0.0.2/pqsdk/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/analyzer.py` & `pqsdk-0.0.2/pqsdk/backtest/analyzer.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/context.py` & `pqsdk-0.0.2/pqsdk/backtest/context.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/current_data.py` & `pqsdk-0.0.2/pqsdk/backtest/current_data.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/instrument.py` & `pqsdk-0.0.2/pqsdk/backtest/instrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/main.py` & `pqsdk-0.0.2/pqsdk/backtest/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,23 +124,33 @@
         :return:
         """
         if hasattr(self.strategy, 'process_initialize'):
             self.strategy.process_initialize(context=context)
 
     def before_trading_start(self, context):
         """
-        开盘前运行策略(可选)
+        开盘前运行(可选)
         该函数会在每天开始交易前被调用一次, 可以在这里添加一些每天都要初始化的动作。
         该函数依据的时间是股票的交易时间，即该函数启动时间为'09:00'.
         :param context:
         :return:
         """
         if hasattr(self.strategy, 'before_trading_start'):
             self.strategy.before_trading_start(context=context)
 
+    def after_trading_end(self, context):
+        """
+        收盘后运行(可选)
+        每天结束交易后被调用一次, 您可以在这里添加一些每天收盘后要执行的内容
+        :param context:
+        :return:
+        """
+        if hasattr(self.strategy, 'after_trading_end'):
+            self.strategy.after_trading_end(context=context)
+
     def notify_order(self, order):
         """
         新创建委托的通知
         :param order: 委托的对象
         :return:
         """
         order_dict = {"order_id": order.order_id,
@@ -224,14 +234,19 @@
         # 执行Analyzers.start()
         for name, analyzer in self.analyzers.items():
             analyzer.start()
 
         # 按照回测时间范围的交易日播放进行回测
         trade_date = None
         for trade_time in df.index.tolist():
+            # new trade date
+            if trade_date is not None and trade_time.strftime('%Y-%m-%d') != trade_date:
+                # 每日收盘后执行，必须在更新设置context之前执行
+                self.after_trading_end(context=self.context)
+
             # 设置benchmark close price
             self.context.set_benchmark_value(df.loc[trade_time]['close'])
 
             # 设置context.dt
             if self.context.unit in ['1d']:
                 # 如果行情周期unit为天，则回测的当前时间(context.current_dt)指向收盘时间15:00
                 close_15_00 = datetime.datetime(trade_time.year, trade_time.month, trade_time.day, 15, 0, 0)
```

### Comparing `pqsdk-0.0.1/pqsdk/backtest/order.py` & `pqsdk-0.0.2/pqsdk/backtest/order.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/portfolio.py` & `pqsdk-0.0.2/pqsdk/backtest/portfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/position.py` & `pqsdk-0.0.2/pqsdk/backtest/position.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/backtest/run_info.py` & `pqsdk-0.0.2/pqsdk/backtest/run_info.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/enums/orderStatus.py` & `pqsdk-0.0.2/pqsdk/enums/orderStatus.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/faxconstant.py` & `pqsdk-0.0.2/pqsdk/faxconstant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/__init__.py` & `pqsdk-0.0.2/pqsdk/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractInstrument.py` & `pqsdk-0.0.2/pqsdk/interface/abstractInstrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractOrder.py` & `pqsdk-0.0.2/pqsdk/interface/abstractOrder.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractPortfolio.py` & `pqsdk-0.0.2/pqsdk/interface/abstractPortfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractPosition.py` & `pqsdk-0.0.2/pqsdk/interface/abstractPosition.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractRunInfo.py` & `pqsdk-0.0.2/pqsdk/interface/abstractRunInfo.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractStrategyContext.py` & `pqsdk-0.0.2/pqsdk/interface/abstractStrategyContext.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/abstractTrader.py` & `pqsdk-0.0.2/pqsdk/interface/abstractTrader.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/interface/constant.py` & `pqsdk-0.0.2/pqsdk/interface/constant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/logger.py` & `pqsdk-0.0.2/pqsdk/logger.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/main.py` & `pqsdk-0.0.2/pqsdk/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/utils/dynamic_import.py` & `pqsdk-0.0.2/pqsdk/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/utils/file_util.py` & `pqsdk-0.0.2/pqsdk/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/utils/timer_factory.py` & `pqsdk-0.0.2/pqsdk/utils/timer_factory.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk/utils/value_type_util.py` & `pqsdk-0.0.2/pqsdk/utils/value_type_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/pqsdk.egg-info/PKG-INFO` & `pqsdk-0.0.2/pqsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.1/pqsdk.egg-info/SOURCES.txt` & `pqsdk-0.0.2/pqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.1/setup.py` & `pqsdk-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 THIS_FOLDER = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_version():
     scope = {}
     version = '0.0.1'
-    version_file = os.path.join(THIS_FOLDER, "faxdatasdk", "version.py")
+    version_file = os.path.join(THIS_FOLDER, "pqsdk", "version.py")
     if os.path.exists(version_file):
         with open(version_file) as fp:
             exec(fp.read(), scope)
         version = scope.get('__version__', '0.0.1')
     return version
```

### Comparing `pqsdk-0.0.1/tests/test_pqsdk_api.py` & `pqsdk-0.0.2/tests/test_pqsdk_api.py`

 * *Files identical despite different names*

