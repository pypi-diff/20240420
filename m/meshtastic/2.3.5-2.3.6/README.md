# Comparing `tmp/meshtastic-2.3.5.tar.gz` & `tmp/meshtastic-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.3.5.tar", last modified: Mon Apr 15 06:47:19 2024, max compression
+gzip compressed data, was "meshtastic-2.3.6.tar", last modified: Sat Apr 20 17:50:19 2024, max compression
```

## Comparing `meshtastic-2.3.5.tar` & `meshtastic-2.3.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:47:19.329728 meshtastic-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 06:47:12.000000 meshtastic-2.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 06:47:12.000000 meshtastic-2.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-15 06:47:19.329728 meshtastic-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-15 06:47:12.000000 meshtastic-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:47:19.329728 meshtastic-2.3.5/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53865 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/apponly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/atak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/atak_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/cannedmessages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/clientonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    65909 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/connection_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/deviceonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/localonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    42944 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    86471 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/module_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mqtt_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/nanopb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    31340 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/paxcount_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/paxcount_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/portnums_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/remote_hardware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/rtttl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/storeforward_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/telemetry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/xmodem_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/xmodem_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:47:19.329728 meshtastic-2.3.5/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:47:19.329728 meshtastic-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-15 06:47:12.000000 meshtastic-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:50:19.300067 meshtastic-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-20 17:50:14.000000 meshtastic-2.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 17:50:14.000000 meshtastic-2.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-20 17:50:19.300067 meshtastic-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-20 17:50:14.000000 meshtastic-2.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:50:19.296067 meshtastic-2.3.6/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55024 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/apponly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/atak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/atak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/cannedmessages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/clientonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66055 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/connection_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/deviceonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/localonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    44751 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86740 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/mesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/module_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/mqtt_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/mt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/nanopb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    31340 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/paxcount_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/paxcount_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/portnums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/remote_hardware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/rtttl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/storeforward_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/telemetry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/xmodem_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-20 17:50:14.000000 meshtastic-2.3.6/meshtastic/xmodem_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:50:19.300067 meshtastic-2.3.6/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-20 17:50:19.000000 meshtastic-2.3.6/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-20 17:50:19.000000 meshtastic-2.3.6/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:50:19.000000 meshtastic-2.3.6/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-20 17:50:19.000000 meshtastic-2.3.6/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 17:50:19.000000 meshtastic-2.3.6/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 17:50:19.000000 meshtastic-2.3.6/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:50:19.300067 meshtastic-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-20 17:50:14.000000 meshtastic-2.3.6/setup.py
```

### Comparing `meshtastic-2.3.5/LICENSE.txt` & `meshtastic-2.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/PKG-INFO` & `meshtastic-2.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.5
+Version: 2.3.6
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.3.5/README.md` & `meshtastic-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/__init__.py` & `meshtastic-2.3.6/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/__main__.py` & `meshtastic-2.3.6/meshtastic/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,22 @@
 import pyqrcode # type: ignore[import-untyped]
 import yaml
 from google.protobuf.json_format import MessageToDict
 from pubsub import pub # type: ignore[import-untyped]
 
 import meshtastic.test
 import meshtastic.util
+from meshtastic import mt_config
 from meshtastic import channel_pb2, config_pb2, portnums_pb2, remote_hardware, BROADCAST_ADDR
 from meshtastic.version import get_active_version
 from meshtastic.ble_interface import BLEInterface
-from meshtastic.globals import Globals
-
 
 def onReceive(packet, interface):
     """Callback invoked when a packet arrives"""
-    our_globals = Globals.getInstance()
-    args = our_globals.get_args()
+    args = mt_config.args
     try:
         d = packet.get("decoded")
         logging.debug(f"in onReceive() d:{d}")
 
         # Exit once we receive a reply
         if (
             args
@@ -65,15 +63,15 @@
     name = splitCompoundName(comp_name)
     wholeField = name[0] == name[1]  # We want the whole field
 
     camel_name = meshtastic.util.snake_to_camel(name[1])
     # Note: protobufs has the keys in snake_case, so snake internally
     snake_name = meshtastic.util.camel_to_snake(name[1])
     logging.debug(f"snake_name:{snake_name} camel_name:{camel_name}")
-    logging.debug(f"use camel:{Globals.getInstance().get_camel_case()}")
+    logging.debug(f"use camel:{mt_config.camel_case}")
 
     # First validate the input
     localConfig = node.localConfig
     moduleConfig = node.moduleConfig
     found = False
     for config in [localConfig, moduleConfig]:
         objDesc = config.DESCRIPTOR
@@ -82,15 +80,15 @@
         if config_type:
             pref = config_type.message_type.fields_by_name.get(snake_name)
             if pref or wholeField:
                 found = True
                 break
 
     if not found:
-        if Globals.getInstance().get_camel_case():
+        if mt_config.camel_case:
             print(
                 f"{localConfig.__class__.__name__} and {moduleConfig.__class__.__name__} do not have an attribute {snake_name}."
             )
         else:
             print(
                 f"{localConfig.__class__.__name__} and {moduleConfig.__class__.__name__} do not have attribute {snake_name}."
             )
@@ -101,15 +99,15 @@
 
     # Check if we need to request the config
     if len(config.ListFields()) != 0:
         # read the value
         config_values = getattr(config, config_type.name)
         if not wholeField:
             pref_value = getattr(config_values, pref.name)
-            if Globals.getInstance().get_camel_case():
+            if mt_config.camel_case:
                 print(f"{str(config_type.name)}.{camel_name}: {str(pref_value)}")
                 logging.debug(
                     f"{str(config_type.name)}.{camel_name}: {str(pref_value)}"
                 )
             else:
                 print(f"{str(config_type.name)}.{snake_name}: {str(pref_value)}")
                 logging.debug(
@@ -123,33 +121,54 @@
         node.requestConfig(config_type)
 
     return True
 
 
 def splitCompoundName(comp_name):
     """Split compound (dot separated) preference name into parts"""
-    name = comp_name.split(".", 1)
-    if len(name) != 2:
+    name = comp_name.split(".")
+    if len(name) < 2:
         name[0] = comp_name
         name.append(comp_name)
     return name
 
+def traverseConfig(config_root, config, interface_config):
+    """Iterate through current config level preferences and either traverse deeper if preference is a dict or set preference"""
+    snake_name = meshtastic.util.camel_to_snake(config_root)
+    for pref in config:
+        pref_name = f"{snake_name}.{pref}"
+        if isinstance(config[pref], dict):
+            traverseConfig(pref_name, config[pref], interface_config)
+        else:
+            setPref(
+                interface_config,
+                pref_name,
+                str(config[pref])
+            )
+
+    return True
 
 def setPref(config, comp_name, valStr) -> bool:
     """Set a channel or preferences value"""
 
     name = splitCompoundName(comp_name)
 
-    snake_name = meshtastic.util.camel_to_snake(name[1])
-    camel_name = meshtastic.util.snake_to_camel(name[1])
+    snake_name = meshtastic.util.camel_to_snake(name[-1])
+    camel_name = meshtastic.util.snake_to_camel(name[-1])
     logging.debug(f"snake_name:{snake_name}")
     logging.debug(f"camel_name:{camel_name}")
 
     objDesc = config.DESCRIPTOR
+    config_part = config
     config_type = objDesc.fields_by_name.get(name[0])
+    if config_type and config_type.message_type is not None:
+        for name_part in name[1:-1]:
+            part_snake_name = meshtastic.util.camel_to_snake((name_part))
+            config_part = getattr(config, config_type.name)
+            config_type = config_type.message_type.fields_by_name.get(part_snake_name)
     pref = None
     if config_type and config_type.message_type is not None:
         pref = config_type.message_type.fields_by_name.get(snake_name)
     # Others like ChannelSettings are standalone
     elif config_type:
         pref = config_type
 
@@ -167,15 +186,15 @@
     # pylint: disable=C0123
     if enumType and type(val) == str:
         # We've failed so far to convert this string into an enum, try to find it by reflection
         e = enumType.values_by_name.get(val)
         if e:
             val = e.number
         else:
-            if Globals.getInstance().get_camel_case():
+            if mt_config.camel_case:
                 print(
                     f"{name[0]}.{camel_name} does not have an enum called {val}, so you can not set it."
                 )
             else:
                 print(
                     f"{name[0]}.{snake_name} does not have an enum called {val}, so you can not set it."
                 )
@@ -188,49 +207,48 @@
                 print(f"    {temp_name}")
             return False
 
     # note: 'ignore_incoming' is a repeating field
     if snake_name != "ignore_incoming":
         try:
             if config_type.message_type is not None:
-                config_values = getattr(config, config_type.name)
+                config_values = getattr(config_part, config_type.name)
                 setattr(config_values, pref.name, val)
             else:
-                setattr(config, snake_name, val)
+                setattr(config_part, snake_name, val)
         except TypeError:
             # The setter didn't like our arg type guess try again as a string
-            config_values = getattr(config, config_type.name)
+            config_values = getattr(config_part, config_type.name)
             setattr(config_values, pref.name, valStr)
     else:
         if val == 0:
             # clear values
             print("Clearing ignore_incoming list")
             del config_type.message_type.ignore_incoming[:]
         else:
             print(f"Adding '{val}' to the ignore_incoming list")
             config_type.message_type.ignore_incoming.extend([val])
 
-    prefix = f"{name[0]}." if config_type.message_type is not None else ""
-    if Globals.getInstance().get_camel_case():
+    prefix = f"{'.'.join(name[0:-1])}." if config_type.message_type is not None else ""
+    if mt_config.camel_case:
         print(f"Set {prefix}{camel_name} to {valStr}")
     else:
         print(f"Set {prefix}{snake_name} to {valStr}")
 
     return True
 
 
 def onConnected(interface):
     """Callback invoked when we connect to a radio"""
     closeNow = False  # Should we drop the connection after we finish?
     waitForAckNak = (
         False  # Should we wait for an acknowledgment if we send to a remote node?
     )
     try:
-        our_globals = Globals.getInstance()
-        args = our_globals.get_args()
+        args = mt_config.args
 
         # do not print this line if we are exporting the config
         if not args.export_config:
             print("Connected to radio")
 
         if args.setlat or args.setlon or args.setalt:
             closeNow = True
@@ -255,15 +273,20 @@
 
             print("Setting device position")
             # can include lat/long/alt etc: latitude = 37.5, longitude = -122.1
             interface.sendPosition(lat, lon, alt)
             interface.localNode.writeConfig("position")
         elif not args.no_time:
             # We normally provide a current time to the mesh when we connect
-            interface.sendPosition()
+            if interface.localNode.nodeNum in interface.nodesByNum and "position" in interface.nodesByNum[interface.localNode.nodeNum]:
+                # send the same position the node already knows, just to update time
+                position = interface.nodesByNum[interface.localNode.nodeNum]["position"]
+                interface.sendPosition(position.get("latitude", 0.0), position.get("longitude", 0.0), position.get("altitude", 0.0))
+            else:
+                interface.sendPosition()
 
         if args.set_owner:
             closeNow = True
             waitForAckNak = True
             print(f"Setting device owner to {args.set_owner}")
             interface.getNode(args.dest, False).setOwner(args.set_owner)
 
@@ -408,14 +431,21 @@
         if args.request_telemetry:
             if args.dest == BROADCAST_ADDR:
                 meshtastic.util.our_exit("Warning: Must use a destination node ID.")
             else:
                 print(f"Sending telemetry request to {args.dest} (this could take a while)")
                 interface.sendTelemetry(destinationId=args.dest, wantResponse=True)
 
+        if args.request_position:
+            if args.dest == BROADCAST_ADDR:
+                meshtastic.util.our_exit("Warning: Must use a destination node ID.")
+            else:
+                print(f"Sending position request to {args.dest} (this could take a while)")
+                interface.sendPosition(destinationId=args.dest, wantResponse=True)
+
         if args.gpio_wrb or args.gpio_rd or args.gpio_watch:
             if args.dest == BROADCAST_ADDR:
                 meshtastic.util.our_exit("Warning: Must use a destination node ID.")
             else:
                 rhc = remote_hardware.RemoteHardwareClient(interface)
 
                 if args.gpio_wrb:
@@ -473,15 +503,15 @@
                         if found:
                             break
 
             if found:
                 print("Writing modified preferences to device")
                 node.writeConfig(field)
             else:
-                if Globals.getInstance().get_camel_case():
+                if mt_config.camel_case:
                     print(
                         f"{node.localConfig.__class__.__name__} and {node.moduleConfig.__class__.__name__} do not have an attribute {pref[0]}."
                     )
                 else:
                     print(
                         f"{node.localConfig.__class__.__name__} and {node.moduleConfig.__class__.__name__} do not have attribute {pref[0]}."
                     )
@@ -530,51 +560,41 @@
                 if "location" in configuration:
                     alt = 0
                     lat = 0.0
                     lon = 0.0
                     localConfig = interface.localNode.localConfig
 
                     if "alt" in configuration["location"]:
-                        alt = int(configuration["location"]["alt"])
+                        alt = int(configuration["location"]["alt"] or 0)
                         localConfig.position.fixed_position = True
                         print(f"Fixing altitude at {alt} meters")
                     if "lat" in configuration["location"]:
-                        lat = float(configuration["location"]["lat"])
+                        lat = float(configuration["location"]["lat"] or 0)
                         localConfig.position.fixed_position = True
                         print(f"Fixing latitude at {lat} degrees")
                     if "lon" in configuration["location"]:
-                        lon = float(configuration["location"]["lon"])
+                        lon = float(configuration["location"]["lon"] or 0)
                         localConfig.position.fixed_position = True
                         print(f"Fixing longitude at {lon} degrees")
                     print("Setting device position")
                     interface.sendPosition(lat, lon, alt)
                     interface.localNode.writeConfig("position")
 
                 if "config" in configuration:
                     localConfig = interface.getNode(args.dest).localConfig
                     for section in configuration["config"]:
-                        for pref in configuration["config"][section]:
-                            setPref(
-                                localConfig,
-                                f"{meshtastic.util.camel_to_snake(section)}.{pref}",
-                                str(configuration["config"][section][pref]),
-                            )
+                        traverseConfig(section, configuration["config"][section], localConfig)
                         interface.getNode(args.dest).writeConfig(
                             meshtastic.util.camel_to_snake(section)
                         )
 
                 if "module_config" in configuration:
                     moduleConfig = interface.getNode(args.dest).moduleConfig
                     for section in configuration["module_config"]:
-                        for pref in configuration["module_config"][section]:
-                            setPref(
-                                moduleConfig,
-                                f"{meshtastic.util.camel_to_snake(section)}.{pref}",
-                                str(configuration["module_config"][section][pref]),
-                            )
+                        traverseConfig(section, configuration["module_config"][section], moduleConfig)
                         interface.getNode(args.dest).writeConfig(
                             meshtastic.util.camel_to_snake(section)
                         )
 
                 interface.getNode(args.dest, False).commitSettingsTransaction()
                 print("Writing modified configuration to device")
 
@@ -586,15 +606,15 @@
         if args.seturl:
             closeNow = True
             interface.getNode(args.dest).setURL(args.seturl)
 
         # handle changing channels
 
         if args.ch_add:
-            channelIndex = our_globals.get_channel_index()
+            channelIndex = mt_config.channel_index
             if channelIndex is not None:
                 # Since we set the channel index after adding a channel, don't allow --ch-index
                 meshtastic.util.our_exit(
                     "Warning: '--ch-add' and '--ch-index' are incompatible. Channel not added."
                 )
             closeNow = True
             if len(args.ch_add) > 10:
@@ -617,20 +637,20 @@
                 chs.name = args.ch_add
                 ch.settings.CopyFrom(chs)
                 ch.role = channel_pb2.Channel.Role.SECONDARY
                 print(f"Writing modified channels to device")
                 n.writeChannel(ch.index)
                 if channelIndex is None:
                     print(f"Setting newly-added channel's {ch.index} as '--ch-index' for further modifications")
-                    our_globals.set_channel_index(ch.index)
+                    mt_config.channel_index = ch.index
 
         if args.ch_del:
             closeNow = True
 
-            channelIndex = our_globals.get_channel_index()
+            channelIndex = mt_config.channel_index
             if channelIndex is None:
                 meshtastic.util.our_exit(
                     "Warning: Need to specify '--ch-index' for '--ch-del'.", 1
                 )
             else:
                 if channelIndex == 0:
                     meshtastic.util.our_exit(
@@ -638,15 +658,15 @@
                     )
                 else:
                     print(f"Deleting channel {channelIndex}")
                     ch = interface.getNode(args.dest).deleteChannel(channelIndex)
 
         def setSimpleConfig(modem_preset):
             """Set one of the simple modem_config"""
-            channelIndex = our_globals.get_channel_index()
+            channelIndex = mt_config.channel_index
             if channelIndex is not None and channelIndex > 0:
                 meshtastic.util.our_exit(
                     "Warning: Cannot set modem preset for non-primary channel", 1
                 )
             # Overwrite modem_preset
             prefs = interface.getNode(args.dest).localConfig
             prefs.lora.modem_preset = modem_preset
@@ -673,15 +693,15 @@
 
         if args.ch_shortfast:
             setSimpleConfig(config_pb2.Config.LoRaConfig.ModemPreset.SHORT_FAST)
 
         if args.ch_set or args.ch_enable or args.ch_disable:
             closeNow = True
 
-            channelIndex = our_globals.get_channel_index()
+            channelIndex = mt_config.channel_index
             if channelIndex is None:
                 meshtastic.util.our_exit("Warning: Need to specify '--ch-index'.", 1)
             ch = interface.getNode(args.dest).channels[channelIndex]
 
             if args.ch_enable or args.ch_disable:
                 if channelIndex == 0:
                     meshtastic.util.our_exit(
@@ -828,15 +848,15 @@
     for config_section in objDesc.fields:
         if config_section.name != "version":
             config = objDesc.fields_by_name.get(config_section.name)
             print(f"{config_section.name}:")
             names = []
             for field in config.message_type.fields:
                 tmp_name = f"{config_section.name}.{field.name}"
-                if Globals.getInstance().get_camel_case():
+                if mt_config.camel_case:
                     tmp_name = meshtastic.util.snake_to_camel(tmp_name)
                 names.append(tmp_name)
             for temp_name in sorted(names):
                 print(f"    {temp_name}")
 
 
 def onNode(node):
@@ -873,59 +893,61 @@
         alt = pos.get("altitude")
 
     if owner:
         configObj["owner"] = owner
     if owner_short:
         configObj["owner_short"] = owner_short
     if channel_url:
-        if Globals.getInstance().get_camel_case():
+        if mt_config.camel_case:
             configObj["channelUrl"] = channel_url
         else:
             configObj["channel_url"] = channel_url
-    if lat or lon or alt:
-        configObj["location"] = {"lat": lat, "lon": lon, "alt": alt}
+    # lat and lon don't make much sense without the other (so fill with 0s), and alt isn't meaningful without both
+    if lat or lon:
+        configObj["location"] = {"lat": lat or float(0), "lon": lon or float(0)}
+        if alt:
+            configObj["location"]["alt"] = alt
 
     config = MessageToDict(interface.localNode.localConfig)
     if config:
         # Convert inner keys to correct snake/camelCase
         prefs = {}
         for pref in config:
-            if Globals.getInstance().get_camel_case():
+            if mt_config.camel_case:
                 prefs[meshtastic.util.snake_to_camel(pref)] = config[pref]
             else:
                 prefs[pref] = config[pref]
-        if Globals.getInstance().get_camel_case():
+        if mt_config.camel_case:
             configObj["config"] = config
         else:
             configObj["config"] = config
 
     module_config = MessageToDict(interface.localNode.moduleConfig)
     if module_config:
         # Convert inner keys to correct snake/camelCase
         prefs = {}
         for pref in module_config:
             if len(module_config[pref]) > 0:
                 prefs[pref] = module_config[pref]
-        if Globals.getInstance().get_camel_case():
+        if mt_config.camel_case:
             configObj["module_config"] = prefs
         else:
             configObj["module_config"] = prefs
 
     config = "# start of Meshtastic configure yaml\n"
     config += yaml.dump(configObj)
     print(config)
     return config
 
 
 def common():
     """Shared code for all of our command line wrappers"""
     logfile = None
-    our_globals = Globals.getInstance()
-    args = our_globals.get_args()
-    parser = our_globals.get_parser()
+    args = mt_config.args
+    parser = mt_config.parser
     logging.basicConfig(
         level=logging.DEBUG if (args.debug or args.listen) else logging.INFO,
         format="%(levelname)s file:%(filename)s %(funcName)s line:%(lineno)s %(message)s",
     )
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
@@ -933,15 +955,15 @@
     else:
         if args.support:
             meshtastic.util.support_info()
             meshtastic.util.our_exit("", 0)
 
         if args.ch_index is not None:
             channelIndex = int(args.ch_index)
-            our_globals.set_channel_index(channelIndex)
+            mt_config.channel_index = channelIndex
 
         if not args.dest:
             args.dest = BROADCAST_ADDR
 
         if not args.seriallog:
             if args.noproto:
                 args.seriallog = "stdout"
@@ -968,15 +990,15 @@
                 logging.debug("Not logging serial output")
                 logfile = None
             else:
                 logging.info(f"Logging serial output to {args.seriallog}")
                 # Note: using "line buffering"
                 # pylint: disable=R1732
                 logfile = open(args.seriallog, "w+", buffering=1, encoding="utf8")
-                our_globals.set_logfile(logfile)
+                mt_config.logfile = logfile
 
             subscribe()
             if args.ble_scan:
                 logging.debug("BLE scan starting")
                 client = BLEInterface(None, debugOut=logfile, noProto=args.noproto)
                 try:
                     for x in client.scan():
@@ -1059,17 +1081,16 @@
     )
 
     return parser
 
 
 def initParser():
     """Initialize the command line argument parsing."""
-    our_globals = Globals.getInstance()
-    parser = our_globals.get_parser()
-    args = our_globals.get_args()
+    parser = mt_config.parser
+    args = mt_config.args
 
     # The "Help" group includes the help option and other informational stuff about the CLI itself
     outerHelpGroup = parser.add_argument_group('Help')
     helpGroup = outerHelpGroup.add_mutually_exclusive_group()
     helpGroup.add_argument("-h", "--help", action="help", help="show this help message and exit")
 
     the_version = get_active_version()
@@ -1282,17 +1303,25 @@
         help="Traceroute from connected node to a destination. "
         "You need pass the destination ID as argument, like "
         "this: '--traceroute !ba4bf9d0' "
         "Only nodes that have the encryption key can be traced.",
     )
 
     group.add_argument(
-        "--request-telemetry", 
+        "--request-telemetry",
         help="Request telemetry from a node. "
-        "You need pass the destination ID as argument with '--dest'. "
+        "You need to pass the destination ID as argument with '--dest'. "
+        "For repeaters, the nodeNum is required.",
+        action="store_true",
+    )
+
+    group.add_argument(
+        "--request-position",
+        help="Request the position from a nade. "
+        "You need to pass the destination ID as an argument with '--dest'. "
         "For repeaters, the nodeNum is required.",
         action="store_true",
     )
 
     group.add_argument(
         "--ack",
         help="Use in combination with --sendtext to wait for an acknowledgment.",
@@ -1427,40 +1456,38 @@
             default=None,
         )
 
     parser.set_defaults(deprecated=None)
 
 
     args = parser.parse_args()
-    our_globals.set_args(args)
-    our_globals.set_parser(parser)
+    mt_config.args = args
+    mt_config.parser = parser
 
 
 def main():
     """Perform command line meshtastic operations"""
-    our_globals = Globals.getInstance()
     parser = argparse.ArgumentParser(
         add_help=False,
         epilog="If no connection arguments are specified, we search for a compatible serial device, "
                "and if none is found, then attempt a TCP connection to localhost.")
-    our_globals.set_parser(parser)
+    mt_config.parser = parser
     initParser()
     common()
-    logfile = our_globals.get_logfile()
+    logfile = mt_config.logfile
     if logfile:
         logfile.close()
 
 
 def tunnelMain():
     """Run a meshtastic IP tunnel"""
-    our_globals = Globals.getInstance()
     parser = argparse.ArgumentParser(add_help=False)
-    our_globals.set_parser(parser)
+    mt_config.parser = parser
     initParser()
-    args = our_globals.get_args()
+    args = mt_config.args
     args.tunnel = True
-    our_globals.set_args(args)
+    mt_config.args = args
     common()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `meshtastic-2.3.5/meshtastic/admin_pb2.py` & `meshtastic-2.3.6/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/admin_pb2.pyi` & `meshtastic-2.3.6/meshtastic/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/apponly_pb2.py` & `meshtastic-2.3.6/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/apponly_pb2.pyi` & `meshtastic-2.3.6/meshtastic/apponly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/atak_pb2.py` & `meshtastic-2.3.6/meshtastic/atak_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/atak_pb2.pyi` & `meshtastic-2.3.6/meshtastic/atak_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/ble_interface.py` & `meshtastic-2.3.6/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.3.6/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/cannedmessages_pb2.pyi` & `meshtastic-2.3.6/meshtastic/cannedmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/channel_pb2.py` & `meshtastic-2.3.6/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/channel_pb2.pyi` & `meshtastic-2.3.6/meshtastic/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/clientonly_pb2.py` & `meshtastic-2.3.6/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/clientonly_pb2.pyi` & `meshtastic-2.3.6/meshtastic/clientonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/config_pb2.py` & `meshtastic-2.3.6/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/config_pb2.pyi` & `meshtastic-2.3.6/meshtastic/config_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -571,55 +571,50 @@
         WAIT_BLUETOOTH_SECS_FIELD_NUMBER: builtins.int
         SDS_SECS_FIELD_NUMBER: builtins.int
         LS_SECS_FIELD_NUMBER: builtins.int
         MIN_WAKE_SECS_FIELD_NUMBER: builtins.int
         DEVICE_BATTERY_INA_ADDRESS_FIELD_NUMBER: builtins.int
         is_power_saving: builtins.bool
         """
-        If set, we are powered from a low-current source (i.e. solar), so even if it looks like we have power flowing in
-        we should try to minimize power consumption as much as possible.
-        YOU DO NOT NEED TO SET THIS IF YOU'VE set is_router (it is implied in that case).
-        Advanced Option
+        Description: Will sleep everything as much as possible, for the tracker and sensor role this will also include the lora radio. 
+        Don't use this setting if you want to use your device with the phone apps or are using a device without a user button.
+        Technical Details: Works for ESP32 devices and NRF52 devices in the Sensor or Tracker roles
         """
         on_battery_shutdown_after_secs: builtins.int
         """
-        If non-zero, the device will fully power off this many seconds after external power is removed.
+         Description: If non-zero, the device will fully power off this many seconds after external power is removed.
         """
         adc_multiplier_override: builtins.float
         """
         Ratio of voltage divider for battery pin eg. 3.20 (R1=100k, R2=220k)
         Overrides the ADC_MULTIPLIER defined in variant for battery voltage calculation.
-        Should be set to floating point value between 2 and 4
-        Fixes issues on Heltec v2
+        https://meshtastic.org/docs/configuration/radio/power/#adc-multiplier-override
+        Should be set to floating point value between 2 and 6
         """
         wait_bluetooth_secs: builtins.int
         """
-        Wait Bluetooth Seconds
-        The number of seconds for to wait before turning off BLE in No Bluetooth states
-        0 for default of 1 minute
+         Description: The number of seconds for to wait before turning off BLE in No Bluetooth states
+         Technical Details: ESP32 Only 0 for default of 1 minute
         """
         sds_secs: builtins.int
         """
         Super Deep Sleep Seconds
         While in Light Sleep if mesh_sds_timeout_secs is exceeded we will lower into super deep sleep
         for this value (default 1 year) or a button press
         0 for default of one year
         """
         ls_secs: builtins.int
         """
-        Light Sleep Seconds
-        In light sleep the CPU is suspended, LoRa radio is on, BLE is off an GPS is on
-        ESP32 Only
-        0 for default of 300
+        Description: In light sleep the CPU is suspended, LoRa radio is on, BLE is off an GPS is on
+        Technical Details: ESP32 Only 0 for default of 300
         """
         min_wake_secs: builtins.int
         """
-        Minimum Wake Seconds
-        While in light sleep when we receive packets on the LoRa radio we will wake and handle them and stay awake in no BLE mode for this value
-        0 for default of 10 seconds
+        Description: While in light sleep when we receive packets on the LoRa radio we will wake and handle them and stay awake in no BLE mode for this value
+        Technical Details: ESP32 Only 0 for default of 10 seconds
         """
         device_battery_ina_address: builtins.int
         """
         I2C address of INA_2XX to use for reading device battery voltage
         """
         def __init__(
             self,
```

### Comparing `meshtastic-2.3.5/meshtastic/connection_status_pb2.py` & `meshtastic-2.3.6/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/connection_status_pb2.pyi` & `meshtastic-2.3.6/meshtastic/connection_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/deviceonly_pb2.py` & `meshtastic-2.3.6/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/deviceonly_pb2.pyi` & `meshtastic-2.3.6/meshtastic/deviceonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/localonly_pb2.py` & `meshtastic-2.3.6/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/localonly_pb2.pyi` & `meshtastic-2.3.6/meshtastic/localonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/mesh_interface.py` & `meshtastic-2.3.6/meshtastic/mesh_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -333,14 +333,15 @@
         meshPacket.channel = channelIndex
         meshPacket.decoded.payload = data
         meshPacket.decoded.portnum = portNum
         meshPacket.decoded.want_response = wantResponse
         meshPacket.id = self._generatePacketId()
 
         if onResponse is not None:
+            logging.debug(f"Setting a response handler for requestId {meshPacket.id}")
             self._addResponseHandler(meshPacket.id, onResponse)
         p = self._sendPacket(meshPacket, destinationId, wantAck=wantAck)
         return p
 
     def sendPosition(
         self,
         latitude: float=0.0,
@@ -376,21 +377,58 @@
             logging.debug(f"p.altitude:{p.altitude}")
 
         if timeSec == 0:
             timeSec = int(time.time())  # returns unix timestamp in seconds
         p.time = timeSec
         logging.debug(f"p.time:{p.time}")
 
-        return self.sendData(
+        if wantResponse:
+            onResponse = self.onResponsePosition
+        else:
+            onResponse = None
+
+        d = self.sendData(
             p,
             destinationId,
             portNum=portnums_pb2.PortNum.POSITION_APP,
             wantAck=wantAck,
             wantResponse=wantResponse,
+            onResponse=onResponse,
         )
+        if wantResponse:
+            self.waitForPosition()
+        return d
+
+    def onResponsePosition(self, p):
+        """on response for position"""
+        if p["decoded"]["portnum"] == 'POSITION_APP':
+            self._acknowledgment.receivedPosition = True
+            position = mesh_pb2.Position()
+            position.ParseFromString(p["decoded"]["payload"])
+
+            ret = "Position received: "
+            if position.latitude_i != 0 and position.longitude_i != 0:
+                ret += f"({position.latitude_i * 10**-7}, {position.longitude_i * 10**-7})"
+            else:
+                ret += "(unknown)"
+            if position.altitude != 0:
+                ret += f" {position.altitude}m"
+
+            if position.precision_bits not in [0,32]:
+                ret += f" precision:{position.precision_bits}"
+            elif position.precision_bits == 32:
+                ret += " full precision"
+            elif position.precision_bits == 0:
+                ret += " position disabled"
+
+            print(ret)
+
+        elif p["decoded"]["portnum"] == 'ROUTING_APP':
+            if p["decoded"]["routing"]["errorReason"] == 'NO_RESPONSE':
+                our_exit("No response from node. At least firmware 2.1.22 is required on the destination node.")
 
     def sendTraceRoute(self, dest: Union[int, str], hopLimit: int):
         """Send the trace route"""
         r = mesh_pb2.RouteDiscovery()
         self.sendData(
             r,
             destinationId=dest,
@@ -440,19 +478,14 @@
                     r.device_metrics.air_util_tx = air_util_tx
 
         if wantResponse:
             onResponse = self.onResponseTelemetry
         else:
             onResponse = None
 
-        if destinationId.startswith("!"):
-            destinationId = int(destinationId[1:], 16)
-        else:
-            destinationId = int(destinationId)
-
         self.sendData(
             r,
             destinationId=destinationId,
             portNum=portnums_pb2.PortNum.TELEMETRY_APP,
             wantResponse=wantResponse,
             onResponse=onResponse,
         )
@@ -568,14 +601,20 @@
 
     def waitForTelemetry(self):
         """Wait for telemetry"""
         success = self._timeout.waitForTelemetry(self._acknowledgment)
         if not success:
             raise MeshInterface.MeshInterfaceError("Timed out waiting for telemetry")
 
+    def waitForPosition(self):
+        """Wait for position"""
+        success = self._timeout.waitForPosition(self._acknowledgment)
+        if not success:
+            raise MeshInterface.MeshInterfaceError("Timed out waiting for position")
+
     def getMyNodeInfo(self) -> Optional[Dict]:
         """Get info about my node."""
         if self.myInfo is None or self.nodesByNum is None:
             return None
         logging.debug(f"self.nodesByNum:{self.nodesByNum}")
         return self.nodesByNum.get(self.myInfo.my_node_num)
 
@@ -1030,21 +1069,23 @@
                 # Call specialized onReceive if necessary
                 if handler.onReceive is not None:
                     handler.onReceive(self, asDict)
 
             # Is this message in response to a request, if so, look for a handler
             requestId = decoded.get("requestId")
             if requestId is not None:
+                logging.debug(f"Got a response for requestId {requestId}")
                 # We ignore ACK packets, but send NAKs and data responses to the handlers
                 routing = decoded.get("routing")
-                isAck = routing is not None and ("errorReason" not in routing)
+                isAck = routing is not None and ("errorReason" not in routing or routing["errorReason"] == "NONE")
                 if not isAck:
                     # we keep the responseHandler in dict until we get a non ack
                     handler = self.responseHandlers.pop(requestId, None)
                     if handler is not None:
                         if not isAck or (isAck and handler.__name__ == "onAckNak"):
+                            logging.debug(f"Calling response handler for requestId {requestId}")
                             handler.callback(asDict)
 
         logging.debug(f"Publishing {topic}: packet={stripnl(asDict)} ")
         publishingThread.queueWork(
             lambda: pub.sendMessage(topic, packet=asDict, interface=self)
         )
```

### Comparing `meshtastic-2.3.5/meshtastic/mesh_pb2.py` & `meshtastic-2.3.6/meshtastic/mesh_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 from meshtastic import portnums_pb2 as meshtastic_dot_portnums__pb2
 from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import xmodem_pb2 as meshtastic_dot_xmodem__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xe5\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12\x37\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x1e.meshtastic.Position.LocSource\x12\x37\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x1e.meshtastic.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\x12\x16\n\x0eprecision_bits\x18\x17 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\xc4\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12+\n\x08hw_model\x18\x05 \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xfc\x02\n\x07Routing\x12\x33\n\rroute_request\x18\x01 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x19.meshtastic.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\xa7\x01\n\x04\x44\x61ta\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"l\n\x16MqttClientProxyMessage\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x10\n\x08retained\x18\x04 \x01(\x08\x42\x11\n\x0fpayload_variant\"\x95\x04\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12#\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x10.meshtastic.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12\x31\n\x08priority\x18\x0b \x01(\x0e\x32\x1f.meshtastic.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12\x33\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x1e.meshtastic.MeshPacket.DelayedB\x02\x18\x01\x12\x10\n\x08via_mqtt\x18\x0e \x01(\x08\x12\x11\n\thop_start\x18\x0f \x01(\r\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xfe\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.meshtastic.User\x12&\n\x08position\x18\x03 \x01(\x0b\x32\x14.meshtastic.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12\x31\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x19.meshtastic.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"P\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\"\xc0\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12*\n\x05level\x18\x04 \x01(\x0e\x32\x1b.meshtastic.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xdb\x04\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12(\n\x06packet\x18\x02 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12)\n\x07my_info\x18\x03 \x01(\x0b\x32\x16.meshtastic.MyNodeInfoH\x00\x12)\n\tnode_info\x18\x04 \x01(\x0b\x32\x14.meshtastic.NodeInfoH\x00\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12+\n\nlog_record\x18\x06 \x01(\x0b\x32\x15.meshtastic.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12\x30\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12&\n\x07\x63hannel\x18\n \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12.\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x17.meshtastic.QueueStatusH\x00\x12*\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12.\n\x08metadata\x18\r \x01(\x0b\x32\x1a.meshtastic.DeviceMetadataH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x0e \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x42\x11\n\x0fpayload_variant\"\x94\x02\n\x07ToRadio\x12(\n\x06packet\x18\x01 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12*\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x06 \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x12*\n\theartbeat\x18\x07 \x01(\x0b\x32\x15.meshtastic.HeartbeatH\x00\x42\x11\n\x0fpayload_variant\"@\n\nCompressed\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x87\x01\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12$\n\x1cnode_broadcast_interval_secs\x18\x03 \x01(\r\x12\'\n\tneighbors\x18\x04 \x03(\x0b\x32\x14.meshtastic.Neighbor\"d\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\x12\x14\n\x0clast_rx_time\x18\x03 \x01(\x07\x12$\n\x1cnode_broadcast_interval_secs\x18\x04 \x01(\r\"\xad\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12+\n\x08hw_model\x18\t \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08\"\x0b\n\tHeartbeat\"U\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12*\n\x03pin\x18\x02 \x01(\x0b\x32\x1d.meshtastic.RemoteHardwarePin*\xef\x07\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x11\n\rNANO_G2_ULTRA\x10\x12\x12\r\n\tLORA_TYPE\x10\x13\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x14\n\x10SENSELORA_RP2040\x10\x1b\x12\x10\n\x0cSENSELORA_S3\x10\x1c\x12\r\n\tCANARYONE\x10\x1d\x12\x0f\n\x0bRP2040_LORA\x10\x1e\x12\x0e\n\nSTATION_G2\x10\x1f\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x1b\n\x17HELTEC_WIRELESS_TRACKER\x10\x30\x12\x19\n\x15HELTEC_WIRELESS_PAPER\x10\x31\x12\n\n\x06T_DECK\x10\x32\x12\x0e\n\nT_WATCH_S3\x10\x33\x12\x11\n\rPICOMPUTER_S3\x10\x34\x12\x0f\n\x0bHELTEC_HT62\x10\x35\x12\x12\n\x0e\x45\x42YTE_ESP32_S3\x10\x36\x12\x11\n\rESP32_S3_PICO\x10\x37\x12\r\n\tCHATTER_2\x10\x38\x12\x1e\n\x1aHELTEC_WIRELESS_PAPER_V1_0\x10\x39\x12 \n\x1cHELTEC_WIRELESS_TRACKER_V1_0\x10:\x12\x0b\n\x07UNPHONE\x10;\x12\x0c\n\x08TD_LORAC\x10<\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xe5\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12\x37\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x1e.meshtastic.Position.LocSource\x12\x37\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x1e.meshtastic.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\x12\x16\n\x0eprecision_bits\x18\x17 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\xc4\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12+\n\x08hw_model\x18\x05 \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xfc\x02\n\x07Routing\x12\x33\n\rroute_request\x18\x01 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x19.meshtastic.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\xa7\x01\n\x04\x44\x61ta\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"l\n\x16MqttClientProxyMessage\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x10\n\x08retained\x18\x04 \x01(\x08\x42\x11\n\x0fpayload_variant\"\x95\x04\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12#\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x10.meshtastic.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12\x31\n\x08priority\x18\x0b \x01(\x0e\x32\x1f.meshtastic.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12\x33\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x1e.meshtastic.MeshPacket.DelayedB\x02\x18\x01\x12\x10\n\x08via_mqtt\x18\x0e \x01(\x08\x12\x11\n\thop_start\x18\x0f \x01(\r\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xfe\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.meshtastic.User\x12&\n\x08position\x18\x03 \x01(\x0b\x32\x14.meshtastic.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12\x31\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x19.meshtastic.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"P\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\"\xc0\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12*\n\x05level\x18\x04 \x01(\x0e\x32\x1b.meshtastic.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xdb\x04\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12(\n\x06packet\x18\x02 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12)\n\x07my_info\x18\x03 \x01(\x0b\x32\x16.meshtastic.MyNodeInfoH\x00\x12)\n\tnode_info\x18\x04 \x01(\x0b\x32\x14.meshtastic.NodeInfoH\x00\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12+\n\nlog_record\x18\x06 \x01(\x0b\x32\x15.meshtastic.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12\x30\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12&\n\x07\x63hannel\x18\n \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12.\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x17.meshtastic.QueueStatusH\x00\x12*\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12.\n\x08metadata\x18\r \x01(\x0b\x32\x1a.meshtastic.DeviceMetadataH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x0e \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x42\x11\n\x0fpayload_variant\"\x94\x02\n\x07ToRadio\x12(\n\x06packet\x18\x01 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12*\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x06 \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x12*\n\theartbeat\x18\x07 \x01(\x0b\x32\x15.meshtastic.HeartbeatH\x00\x42\x11\n\x0fpayload_variant\"@\n\nCompressed\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x87\x01\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12$\n\x1cnode_broadcast_interval_secs\x18\x03 \x01(\r\x12\'\n\tneighbors\x18\x04 \x03(\x0b\x32\x14.meshtastic.Neighbor\"d\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\x12\x14\n\x0clast_rx_time\x18\x03 \x01(\x07\x12$\n\x1cnode_broadcast_interval_secs\x18\x04 \x01(\r\"\xad\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12+\n\x08hw_model\x18\t \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08\"\x0b\n\tHeartbeat\"U\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12*\n\x03pin\x18\x02 \x01(\x0b\x32\x1d.meshtastic.RemoteHardwarePin*\x84\x08\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x11\n\rNANO_G2_ULTRA\x10\x12\x12\r\n\tLORA_TYPE\x10\x13\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x14\n\x10SENSELORA_RP2040\x10\x1b\x12\x10\n\x0cSENSELORA_S3\x10\x1c\x12\r\n\tCANARYONE\x10\x1d\x12\x0f\n\x0bRP2040_LORA\x10\x1e\x12\x0e\n\nSTATION_G2\x10\x1f\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x1b\n\x17HELTEC_WIRELESS_TRACKER\x10\x30\x12\x19\n\x15HELTEC_WIRELESS_PAPER\x10\x31\x12\n\n\x06T_DECK\x10\x32\x12\x0e\n\nT_WATCH_S3\x10\x33\x12\x11\n\rPICOMPUTER_S3\x10\x34\x12\x0f\n\x0bHELTEC_HT62\x10\x35\x12\x12\n\x0e\x45\x42YTE_ESP32_S3\x10\x36\x12\x11\n\rESP32_S3_PICO\x10\x37\x12\r\n\tCHATTER_2\x10\x38\x12\x1e\n\x1aHELTEC_WIRELESS_PAPER_V1_0\x10\x39\x12 \n\x1cHELTEC_WIRELESS_TRACKER_V1_0\x10:\x12\x0b\n\x07UNPHONE\x10;\x12\x0c\n\x08TD_LORAC\x10<\x12\x13\n\x0f\x43\x44\x45\x42YTE_EORA_S3\x10=\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.mesh_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _USER.fields_by_name['macaddr']._options = None
   _USER.fields_by_name['macaddr']._serialized_options = b'\030\001'
   _MESHPACKET.fields_by_name['delayed']._options = None
   _MESHPACKET.fields_by_name['delayed']._serialized_options = b'\030\001'
   _HARDWAREMODEL._serialized_start=4737
-  _HARDWAREMODEL._serialized_end=5744
-  _CONSTANTS._serialized_start=5746
-  _CONSTANTS._serialized_end=5790
-  _CRITICALERRORCODE._serialized_start=5793
-  _CRITICALERRORCODE._serialized_end=6031
+  _HARDWAREMODEL._serialized_end=5765
+  _CONSTANTS._serialized_start=5767
+  _CONSTANTS._serialized_end=5811
+  _CRITICALERRORCODE._serialized_start=5814
+  _CRITICALERRORCODE._serialized_end=6052
   _POSITION._serialized_start=201
   _POSITION._serialized_end=942
   _POSITION_LOCSOURCE._serialized_start=764
   _POSITION_LOCSOURCE._serialized_end=842
   _POSITION_ALTSOURCE._serialized_start=844
   _POSITION_ALTSOURCE._serialized_end=942
   _USER._serialized_start=945
```

### Comparing `meshtastic-2.3.5/meshtastic/mesh_pb2.pyi` & `meshtastic-2.3.6/meshtastic/mesh_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,18 @@
     unPhone with ESP32-S3, TFT touchscreen,  LSM6DS3TR-C accelerometer and gyroscope
     """
     TD_LORAC: _HardwareModel.ValueType  # 60
     """
     Teledatics TD-LORAC NRF52840 based M.2 LoRA module
     Compatible with the TD-WRLS development board
     """
+    CDEBYTE_EORA_S3: _HardwareModel.ValueType  # 61
+    """
+    CDEBYTE EoRa-S3 board using their own MM modules, clone of LILYGO T3S3
+    """
     PRIVATE_HW: _HardwareModel.ValueType  # 255
     """
     ------------------------------------------------------------------------------------------------------------------------------------------
     Reserved ID For developing private Ports. These will show up in live traffic sparsely, so we can use a high number. Keep it within 8 bits.
     ------------------------------------------------------------------------------------------------------------------------------------------
     """
 
@@ -515,14 +519,18 @@
 unPhone with ESP32-S3, TFT touchscreen,  LSM6DS3TR-C accelerometer and gyroscope
 """
 TD_LORAC: HardwareModel.ValueType  # 60
 """
 Teledatics TD-LORAC NRF52840 based M.2 LoRA module
 Compatible with the TD-WRLS development board
 """
+CDEBYTE_EORA_S3: HardwareModel.ValueType  # 61
+"""
+CDEBYTE EoRa-S3 board using their own MM modules, clone of LILYGO T3S3
+"""
 PRIVATE_HW: HardwareModel.ValueType  # 255
 """
 ------------------------------------------------------------------------------------------------------------------------------------------
 Reserved ID For developing private Ports. These will show up in live traffic sparsely, so we can use a high number. Keep it within 8 bits.
 ------------------------------------------------------------------------------------------------------------------------------------------
 """
 global___HardwareModel = HardwareModel
```

### Comparing `meshtastic-2.3.5/meshtastic/module_config_pb2.py` & `meshtastic-2.3.6/meshtastic/module_config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/module_config_pb2.pyi` & `meshtastic-2.3.6/meshtastic/module_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/mqtt_pb2.py` & `meshtastic-2.3.6/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/mqtt_pb2.pyi` & `meshtastic-2.3.6/meshtastic/mqtt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/nanopb_pb2.py` & `meshtastic-2.3.6/meshtastic/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/nanopb_pb2.pyi` & `meshtastic-2.3.6/meshtastic/nanopb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/node.py` & `meshtastic-2.3.6/meshtastic/node.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/paxcount_pb2.py` & `meshtastic-2.3.6/meshtastic/paxcount_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/paxcount_pb2.pyi` & `meshtastic-2.3.6/meshtastic/paxcount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/portnums_pb2.py` & `meshtastic-2.3.6/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/portnums_pb2.pyi` & `meshtastic-2.3.6/meshtastic/portnums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/remote_hardware.py` & `meshtastic-2.3.6/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.3.6/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/remote_hardware_pb2.pyi` & `meshtastic-2.3.6/meshtastic/remote_hardware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/rtttl_pb2.py` & `meshtastic-2.3.6/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/rtttl_pb2.pyi` & `meshtastic-2.3.6/meshtastic/rtttl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/serial_interface.py` & `meshtastic-2.3.6/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/storeforward_pb2.py` & `meshtastic-2.3.6/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/storeforward_pb2.pyi` & `meshtastic-2.3.6/meshtastic/storeforward_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/stream_interface.py` & `meshtastic-2.3.6/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/supported_device.py` & `meshtastic-2.3.6/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/tcp_interface.py` & `meshtastic-2.3.6/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/telemetry_pb2.py` & `meshtastic-2.3.6/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/telemetry_pb2.pyi` & `meshtastic-2.3.6/meshtastic/telemetry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/test.py` & `meshtastic-2.3.6/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/tunnel.py` & `meshtastic-2.3.6/meshtastic/tunnel.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,22 @@
 import logging
 import platform
 import threading
 
 from pubsub import pub # type: ignore[import-untyped]
 from pytap2 import TapDevice
 
-from meshtastic import portnums_pb2
-from meshtastic.globals import Globals
+from meshtastic import portnums_pb2, mt_config
 from meshtastic.util import ipstr, readnet_u16
 
 
 def onTunnelReceive(packet, interface):  # pylint: disable=W0613
     """Callback for received tunneled messages from mesh."""
     logging.debug(f"in onTunnelReceive()")
-    our_globals = Globals.getInstance()
-    tunnelInstance = our_globals.get_tunnelInstance()
+    tunnelInstance = mt_config.tunnelInstance
     tunnelInstance.onReceive(packet)
 
 
 class Tunnel:
     """A TUN based IP tunnel over meshtastic"""
 
     class TunnelError(Exception):
@@ -63,16 +61,15 @@
 
         self.iface = iface
         self.subnetPrefix = subnet
 
         if platform.system() != "Linux":
             raise Tunnel.TunnelError("Tunnel() can only be run instantiated on a Linux system")
 
-        our_globals = Globals.getInstance()
-        our_globals.set_tunnelInstance(self)
+        mt_config.tunnelInstance = self
 
         """A list of chatty UDP services we should never accidentally
         forward to our slow network"""
         self.udpBlacklist = {
             1900,  # SSDP
             5353,  # multicast DNS
             9001,  # Yggdrasil multicast discovery
```

### Comparing `meshtastic-2.3.5/meshtastic/util.py` & `meshtastic-2.3.6/meshtastic/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -202,32 +202,44 @@
         while time.time() < self.expireTime:
             if getattr(acknowledgment, "receivedTelemetry", None):
                 acknowledgment.reset()
                 return True
             time.sleep(self.sleepInterval)
         return False
 
+    def waitForPosition(self, acknowledgment) -> bool:
+        """Block until position response is received. Returns True if position response has been received."""
+        self.reset()
+        while time.time() < self.expireTime:
+            if getattr(acknowledgment, "receivedPosition", None):
+                acknowledgment.reset()
+                return True
+            time.sleep(self.sleepInterval)
+        return False
+
 class Acknowledgment:
     "A class that records which type of acknowledgment was just received, if any."
 
     def __init__(self):
         """initialize"""
         self.receivedAck = False
         self.receivedNak = False
         self.receivedImplAck = False
         self.receivedTraceRoute = False
         self.receivedTelemetry = False
+        self.receivedPosition = False
 
     def reset(self):
         """reset"""
         self.receivedAck = False
         self.receivedNak = False
         self.receivedImplAck = False
         self.receivedTraceRoute = False
         self.receivedTelemetry = False
+        self.receivedPosition = False
 
 
 class DeferredExecution:
     """A thread that accepts closures to run, and runs them as they are received"""
 
     def __init__(self, name=None):
         self.queue = Queue()
```

### Comparing `meshtastic-2.3.5/meshtastic/xmodem_pb2.py` & `meshtastic-2.3.6/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic/xmodem_pb2.pyi` & `meshtastic-2.3.6/meshtastic/xmodem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.5/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.3.6/meshtastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.5
+Version: 2.3.6
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.3.5/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.3.6/meshtastic.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 meshtastic/clientonly_pb2.pyi
 meshtastic/config_pb2.py
 meshtastic/config_pb2.pyi
 meshtastic/connection_status_pb2.py
 meshtastic/connection_status_pb2.pyi
 meshtastic/deviceonly_pb2.py
 meshtastic/deviceonly_pb2.pyi
-meshtastic/globals.py
 meshtastic/localonly_pb2.py
 meshtastic/localonly_pb2.pyi
 meshtastic/mesh_interface.py
 meshtastic/mesh_pb2.py
 meshtastic/mesh_pb2.pyi
 meshtastic/module_config_pb2.py
 meshtastic/module_config_pb2.pyi
 meshtastic/mqtt_pb2.py
 meshtastic/mqtt_pb2.pyi
+meshtastic/mt_config.py
 meshtastic/nanopb_pb2.py
 meshtastic/nanopb_pb2.pyi
 meshtastic/node.py
 meshtastic/paxcount_pb2.py
 meshtastic/paxcount_pb2.pyi
 meshtastic/portnums_pb2.py
 meshtastic/portnums_pb2.pyi
```

### Comparing `meshtastic-2.3.5/setup.py` & `meshtastic-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.3.5",
+    version="2.3.6",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

