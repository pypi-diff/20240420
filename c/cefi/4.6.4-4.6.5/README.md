# Comparing `tmp/cefi-4.6.4.tar.gz` & `tmp/cefi-4.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.6.4.tar", max compression
+gzip compressed data, was "cefi-4.6.5.tar", max compression
```

## Comparing `cefi-4.6.4.tar` & `cefi-4.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-19 04:26:31.559533 cefi-4.6.4/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-19 04:26:31.559533 cefi-4.6.4/README.md
--rw-r--r--   0        0        0       87 2024-04-19 04:27:09.655373 cefi-4.6.4/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/handler/__init__.py
--rw-r--r--   0        0        0    11183 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9015 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8160 2024-04-19 04:26:31.559533 cefi-4.6.4/cefi/main.py
--rw-r--r--   0        0        0     3768 2024-04-19 04:27:09.655373 cefi-4.6.4/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 06:05:07.102684 cefi-4.6.5/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-19 06:05:07.102684 cefi-4.6.5/README.md
+-rw-r--r--   0        0        0       87 2024-04-19 06:05:47.278849 cefi-4.6.5/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    11153 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9015 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8160 2024-04-19 06:05:07.102684 cefi-4.6.5/cefi/main.py
+-rw-r--r--   0        0        0     3770 2024-04-19 06:05:47.278849 cefi-4.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.5/PKG-INFO
```

### Comparing `cefi-4.6.4/LICENSE` & `cefi-4.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/README.md` & `cefi-4.6.5/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/cefi/default_settings.toml` & `cefi-4.6.5/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/cefi/handler/capitalcom.py` & `cefi-4.6.5/cefi/handler/capitalcom.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             instrument = await self.replace_instrument(instrument)
             logger.debug("Changed Instrument: {}", instrument)
             # search_markets = self.client.searching_market(searchTerm=instrument)
             await asyncio.sleep(1)  # Wait for 1 second
             # logger.debug("Instrument verification: {}", search_markets)
 
             market = self.client.single_market(instrument)
-            # logger.debug("Raw Quote: {}", market)
+            # logger.debug("market: {}", market)
 
             quote = market["snapshot"]["offer"]
             logger.debug("Quote: {}", quote)
 
             return float(quote)
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
@@ -250,16 +250,16 @@
         instrument_info = self.client.single_market(instrument)
         logger.debug("instrument_info {}", instrument_info)
         minimum_amount = (
             instrument_info.get("dealingRules", {})
             .get("minDealSize", {})
             .get("value", 0)
         )
-        logger.debug("Minimum {}", minimum_amount)
-        return int(minimum_amount)
+        logger.debug("Minimum Amount Needed {}", minimum_amount)
+        return float(minimum_amount)
 
     async def execute_order(self, order_params):
         """
         Execute order
 
         Args:
             order_params (dict):
@@ -279,17 +279,16 @@
             quantity = order_params.get("quantity", self.trading_risk_amount)
             amount = await self.get_order_amount(
                 quantity=quantity,
                 instrument=instrument,
                 is_percentage=self.trading_risk_percentage,
             )
             min_amount = await self.get_instrument_min_amount(instrument)
-            logger.debug("min_amount {}", min_amount)
             amount = max(amount, min_amount)
-            logger.debug("amount {}", amount)
+            logger.debug("Amount to execute {}", amount)
             await asyncio.sleep(1)  # Wait for 1 second
 
             if not (await self.pre_order_checks(order_params)):
                 return f"Error executing {self.name}"
 
             decimals = await self.get_instrument_decimals(instrument)
             await asyncio.sleep(1)  # Wait for 1 second
```

### Comparing `cefi-4.6.4/cefi/handler/ccxt.py` & `cefi-4.6.5/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/cefi/handler/client.py` & `cefi-4.6.5/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/cefi/handler/ctrader.py` & `cefi-4.6.5/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/cefi/handler/ib_sync.py` & `cefi-4.6.5/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/cefi/main.py` & `cefi-4.6.5/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.4/pyproject.toml` & `cefi-4.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.6.4"
+version = "4.6.5"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -163,27 +163,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.6.4/PKG-INFO` & `cefi-4.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.6.4
+Version: 4.6.5
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.6.4 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.6.5 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

