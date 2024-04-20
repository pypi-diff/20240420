# Comparing `tmp/victron-0.0.1.tar.gz` & `tmp/victron-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "victron-0.0.1.tar", last modified: Fri Apr 19 08:41:19 2024, max compression
+gzip compressed data, was "victron-0.0.2.tar", last modified: Sat Apr 20 18:19:35 2024, max compression
```

## Comparing `victron-0.0.1.tar` & `victron-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:41:19.752655 victron-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-19 08:41:13.000000 victron-0.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 08:41:13.000000 victron-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-19 08:41:19.752655 victron-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-19 08:41:13.000000 victron-0.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-19 08:41:19.752655 victron-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-19 08:41:13.000000 victron-0.0.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-19 08:41:13.000000 victron-0.0.1/versioneer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:41:19.751655 victron-0.0.1/victron/
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-19 08:41:13.000000 victron-0.0.1/victron/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-19 08:41:19.752655 victron-0.0.1/victron/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-19 08:41:13.000000 victron-0.0.1/victron/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2907 2024-04-19 08:41:13.000000 victron-0.0.1/victron/victron.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:41:19.752655 victron-0.0.1/victron.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-19 08:41:19.000000 victron-0.0.1/victron.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      296 2024-04-19 08:41:19.000000 victron-0.0.1/victron.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 08:41:19.000000 victron-0.0.1/victron.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-19 08:41:19.000000 victron-0.0.1/victron.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 08:41:19.000000 victron-0.0.1/victron.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 18:19:35.742142 victron-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-20 18:19:29.000000 victron-0.0.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-20 18:19:29.000000 victron-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-20 18:19:35.742142 victron-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-20 18:19:29.000000 victron-0.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-20 18:19:35.743142 victron-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-20 18:19:29.000000 victron-0.0.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-20 18:19:29.000000 victron-0.0.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 18:19:35.741142 victron-0.0.2/victron/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-20 18:19:29.000000 victron-0.0.2/victron/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-20 18:19:35.743142 victron-0.0.2/victron/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-04-20 18:19:29.000000 victron-0.0.2/victron/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2024-04-20 18:19:29.000000 victron-0.0.2/victron/victron.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 18:19:35.742142 victron-0.0.2/victron.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      296 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/top_level.txt
```

### Comparing `victron-0.0.1/LICENSE` & `victron-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `victron-0.0.1/PKG-INFO` & `victron-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron
-Version: 0.0.1
+Version: 0.0.2
 Summary: An SDK for Victron via Modbus TCP
 Home-page: https://gitlab.com/jfk344/python-victron-sdk
 Author: @jfk344
 Author-email: info@jfk-enterprise.com
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `victron-0.0.1/README.md` & `victron-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `victron-0.0.1/setup.cfg` & `victron-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `victron-0.0.1/versioneer.py` & `victron-0.0.2/versioneer.py`

 * *Files identical despite different names*

### Comparing `victron-0.0.1/victron/victron.py` & `victron-0.0.2/victron/victron.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,17 @@
         self.host = host
         self.port = port
         self.unit_id = unit_id
         self.client = None
 
         self.gridLimit = config.get(c.CFG_GRID_LIMIT)
         self.essFeedLimit = config.get(c.CFG_ESS_FEED_LIMIT)
-        self.socLimit = config.get(c.CFG_ESS_SOC_LIMIT)
+        self.essChargeLimit = config.get(c.CFG_ESS_CHARGE_LIMIT)
+        self.socLimit = config.get(c.CFG_SOC_LIMIT)
+        self.batteryCapacity = config.get(c.CFG_BATTERY_CAPACITY)
 
         self.connect()
 
     def connect(self):
         self.client = ModbusClient(
             host=self.host,
             port=self.port,
@@ -44,28 +46,33 @@
 
     def writeSingleHoldingRegisters(self, address:int, value:float):
         return self.client.write_single_register(address, int(value))
 
     def getSoc(self, address:int=843) -> float:
         return self.readSingleHoldingRegisters(address, 1)
     
-    def isSocLimitReached(self, soc:float|None=None) -> bool:
+    def isSocLimitReached(self, soc:float|None=None, socLimit:float|None=None) -> bool:
         if soc is None:
             soc = self.getSoc()
-        return soc <= self.socLimit
+        if socLimit is None:
+            if self.socLimit is None:
+                log.error("SOC limit not set.")
+                return False
+            socLimit = self.socLimit
+        return soc <= socLimit
 
     def getPower(self, address:int=820):
         return self.readSingleHoldingRegisters(address, 1)
 
     def getEssSetPoint(self, address:int=2700):
         return self.readSingleHoldingRegisters(address, 1)
 
     def applyLimit(self, value:int, limit:int) -> int:
         if value < 0:
-            if value < limit * -1:
+            if value < (limit * -1):
                 log.debug(f"Limit reached: {value} of {limit * -1}.")
                 value = limit * -1
         else:
             if value > limit:
                 log.debug(f"Limit reached: {value} of {limit}.")
                 value = limit
         return value
@@ -76,12 +83,25 @@
         return value
 
     def applyFeedLimit(self, value:int) -> int:
         if self.essFeedLimit is not None:
             value = self.applyLimit(value, self.essFeedLimit)
         return value
 
-    def setEssSetPoint(self, value:int, address:int=2700):
+    def applyChargeLimit(self, value:int) -> int:
+        if self.essChargeLimit is not None:
+            value = self.applyLimit(value, self.essChargeLimit)
+        return value
+
+    def setEssSetPoint(self, value:int, address:int=2700, soc:float|None=None, socLimit:float|None=None) -> int:
         value = self.applyGridLimit(value)
-        value = self.applyFeedLimit(value)
+        if value < 0: # only apply feed limit if value is negative
+            value = self.applyFeedLimit(value)
+            if socLimit is not None and soc is not None:
+                if self.isSocLimitReached(soc=soc, socLimit=socLimit):
+                    log.debug(f"SOC limit reached. Setting ESS feed limit to 0.")
+                    value = 0
+        else:
+            value = self.applyChargeLimit(value)
         value = self.parseSetPoint(value)
-        return self.writeSingleHoldingRegisters(address, value)
+        self.writeSingleHoldingRegisters(address, value)
+        return self.parseValue(value)
```

### Comparing `victron-0.0.1/victron.egg-info/PKG-INFO` & `victron-0.0.2/victron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron
-Version: 0.0.1
+Version: 0.0.2
 Summary: An SDK for Victron via Modbus TCP
 Home-page: https://gitlab.com/jfk344/python-victron-sdk
 Author: @jfk344
 Author-email: info@jfk-enterprise.com
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

