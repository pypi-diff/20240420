# Comparing `tmp/DFRobotUPS-0.3.1.tar.gz` & `tmp/DFRobotUPS-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobotUPS-0.3.1.tar", last modified: Wed Apr 17 09:12:33 2024, max compression
+gzip compressed data, was "DFRobotUPS-0.3.2.tar", last modified: Fri Apr 19 23:43:06 2024, max compression
```

## Comparing `DFRobotUPS-0.3.1.tar` & `DFRobotUPS-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-17 09:12:33.099957 DFRobotUPS-0.3.1/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-17 09:12:33.059957 DFRobotUPS-0.3.1/DFRobotUPS/
--rw-r--r--   0 pi        (1000) pi        (1000)      195 2024-04-17 09:09:31.000000 DFRobotUPS-0.3.1/DFRobotUPS/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3173 2024-04-17 09:04:38.000000 DFRobotUPS-0.3.1/DFRobotUPS/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3632 2024-04-17 00:41:12.000000 DFRobotUPS-0.3.1/DFRobotUPS/ups.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-17 09:12:33.089957 DFRobotUPS-0.3.1/DFRobotUPS.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-17 09:12:30.000000 DFRobotUPS-0.3.1/DFRobotUPS.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-17 09:12:32.000000 DFRobotUPS-0.3.1/DFRobotUPS.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-17 09:12:30.000000 DFRobotUPS-0.3.1/DFRobotUPS.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-17 09:12:30.000000 DFRobotUPS-0.3.1/DFRobotUPS.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-17 09:12:30.000000 DFRobotUPS-0.3.1/DFRobotUPS.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-17 00:41:12.000000 DFRobotUPS-0.3.1/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-17 09:12:33.099957 DFRobotUPS-0.3.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-17 00:41:12.000000 DFRobotUPS-0.3.1/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-17 09:12:33.109957 DFRobotUPS-0.3.1/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-17 00:41:12.000000 DFRobotUPS-0.3.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-19 23:43:06.693239 DFRobotUPS-0.3.2/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-19 23:43:06.693239 DFRobotUPS-0.3.2/DFRobotUPS/
+-rw-r--r--   0 pi        (1000) pi        (1000)      327 2024-04-19 23:42:10.000000 DFRobotUPS-0.3.2/DFRobotUPS/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4290 2024-04-19 23:42:10.000000 DFRobotUPS-0.3.2/DFRobotUPS/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-04-19 23:42:10.000000 DFRobotUPS-0.3.2/DFRobotUPS/ups.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-19 23:43:06.693239 DFRobotUPS-0.3.2/DFRobotUPS.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-19 23:43:06.000000 DFRobotUPS-0.3.2/DFRobotUPS.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-19 23:43:06.000000 DFRobotUPS-0.3.2/DFRobotUPS.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-19 23:43:06.000000 DFRobotUPS-0.3.2/DFRobotUPS.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-19 23:43:06.000000 DFRobotUPS-0.3.2/DFRobotUPS.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-19 23:43:06.000000 DFRobotUPS-0.3.2/DFRobotUPS.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-19 23:42:10.000000 DFRobotUPS-0.3.2/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-19 23:43:06.693239 DFRobotUPS-0.3.2/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-19 23:42:10.000000 DFRobotUPS-0.3.2/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-19 23:43:06.693239 DFRobotUPS-0.3.2/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-19 23:42:10.000000 DFRobotUPS-0.3.2/setup.py
```

### Comparing `DFRobotUPS-0.3.1/DFRobotUPS/__main__.py` & `DFRobotUPS-0.3.2/DFRobotUPS/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,28 @@
 
 import argparse
 import functools
 import os
 import sys
 from time import sleep
 
-from . import __version__, DFRobotUPS, DEFAULT_ADDR, DEFAULT_BUS, PID
+from . import (__version__, DFRobotUPS, DEFAULT_ADDR, DEFAULT_BUS, PID,
+               DETECT_OK, DETECT_NODEVICE, DETECT_INVALIDPID)
+
+
+
+# --- constants ---
+
+
+
+# default values for command line parameters
+
+DEFAULT_PERCENT = 7
+DEFAULT_INTERVAL = 60
+DEFAULT_RETRY = 10
 
 
 
 # --- parse arguments ---
 
 
 
@@ -32,40 +45,50 @@
     help="poll the battery SoC and initiate system shutdown when level"
          " drops below the defined level; the default is not to do this"
          " but display information about the UPS HAT instead")
 
 parser.add_argument(
     "-p", "--percent",
     type=int,
-    default=7,
-    help="State of Charge (SoC) percentage at which to trigger shutdown")
+    default=DEFAULT_PERCENT,
+    help="State of Charge (SoC) percentage at which to trigger shutdown"
+         f" shutdown (default: {DEFAULT_PERCENT})")
 
 parser.add_argument(
     "-i", "--interval",
     type=int,
-    default=60,
-    help="number of seconds between polls of the battery SoC")
+    default=DEFAULT_INTERVAL,
+    help="number of seconds between polls of the battery SoC (default:"
+         f" {DEFAULT_INTERVAL})")
 
 parser.add_argument(
     "-c", "--cmd",
     nargs="+",
     default=("/sbin/halt", ),
     help="command to run to trigger shutdown")
 
 parser.add_argument(
     "-a", "--addr",
     type=functools.partial(int, base=0),
     default=DEFAULT_ADDR,
-    help="I2C address for UPS HAT; can be specified in hex as 0xNN")
+    help="I2C address for UPS HAT; can be specified in hex as 0xNN"
+         f" (default: 0x{DEFAULT_ADDR:02x})")
 
 parser.add_argument(
     "-b", "--bus",
     type=int,
     default=DEFAULT_BUS,
-    help="I2C SMBus number for UPS HAT")
+    help=f"I2C SMBus number for UPS HAT (default: {DEFAULT_BUS})")
+
+parser.add_argument(
+    "-r", "--retry",
+    type=int,
+    default=DEFAULT_RETRY,
+    help="number of times to try connecting to the UPS HAT (default:"
+         f" {DEFAULT_RETRY})")
 
 parser.add_argument(
     "-d", "--debug",
     action="store_true",
     help="enable debugging output")
 
 parser.add_argument(
@@ -81,33 +104,55 @@
 
 
 
 if args.debug:
     print(f"DFRobotUPS HAT on bus {args.bus} at I2C address 0x{args.addr:02x}")
 
 
-# get the UPS object to poll SoC
+# try to detect the UPS
 
-ups = DFRobotUPS(addr=args.addr, bus=args.bus)
+tries = 0
+while True:
+    tries += 1
+    ups = DFRobotUPS(addr=args.addr, bus=args.bus)
 
+    if ups.detect == DETECT_OK:
+        break
 
-# if we're debugging, print some information about the UPS HAT
+    if args.debug:
+        print(f"Connection failed error code {ups.detect}, try {tries} of"
+              f" {args.retry}")
 
-if args.debug:
-    print(f"UPS HAT found with product ID 0x{ups.pid:02x} firmware",
-          "version %d.%d" % ups.fwver)
+    # if we've run out of tries, stop
+    if tries == args.retry:
+        break
 
+    sleep(1)
 
-# check we do appear to have a UPS HAT at the specified address/bus
+if ups.detect != DETECT_OK:
+    if ups.detect == DETECT_NODEVICE:
+        print("error: no device found at I2C address", file=sys.stderr)
+
+    elif ups.detect == DETECT_INVALIDPID:
+        print("error: device PID invalid for UPS HAT", file=sys.stderr)
+
+    else:
+        print(f"error: detection failed - unknown reason: {ups.detect}",
+              file=sys.stderr)
 
-if not ups.present:
-    print("error: UPS HAT not found")
     sys.exit(1)
 
 
+# if we're debugging, print some information about the UPS HAT
+
+if args.debug:
+    print(f"UPS HAT found with product ID 0x{ups.pid:02x} firmware",
+          "version %d.%d" % ups.fwver)
+
+
 # if we're in shutdown polling mode, do that
 
 if args.shutdown:
     if args.debug:
         print("Polling SoC for shutdown with command:", *args.cmd)
 
     while True:
```

### Comparing `DFRobotUPS-0.3.1/DFRobotUPS.egg-info/PKG-INFO` & `DFRobotUPS-0.3.2/DFRobotUPS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.3.1
+Version: 0.3.2
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.3.1/LICENSE` & `DFRobotUPS-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.3.1/PKG-INFO` & `DFRobotUPS-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.3.1
+Version: 0.3.2
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.3.1/README.md` & `DFRobotUPS-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.3.1/setup.py` & `DFRobotUPS-0.3.2/setup.py`

 * *Files identical despite different names*

