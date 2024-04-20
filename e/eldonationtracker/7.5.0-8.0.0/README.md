# Comparing `tmp/eldonationtracker-7.5.0.tar.gz` & `tmp/eldonationtracker-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eldonationtracker-7.5.0.tar", last modified: Sun Mar 19 00:35:34 2023, max compression
+gzip compressed data, was "eldonationtracker-8.0.0.tar", last modified: Sat Apr 20 20:16:28 2024, max compression
```

## Comparing `eldonationtracker-7.5.0.tar` & `eldonationtracker-8.0.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.602238 eldonationtracker-7.5.0/eldonationtracker/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.602238 eldonationtracker-7.5.0/eldonationtracker/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/badge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/donation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/donor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9293 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/team.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/api/team_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    53391 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/eldonationtracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/test_donation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/test_donor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24176 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/test_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    21155 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/test_team.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/tests/test_team_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/eldonationtracker/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/about.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/call_about.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/call_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/call_main_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/call_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/call_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/main_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/ui/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/eldonationtracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/utils/extralife_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/eldonationtracker/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/utils/tests/test_extralife_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/utils/tests/test_update_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-19 00:35:17.000000 eldonationtracker-7.5.0/eldonationtracker/utils/update_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:35:34.602238 eldonationtracker-7.5.0/eldonationtracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-19 00:35:34.000000 eldonationtracker-7.5.0/eldonationtracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-19 00:35:34.000000 eldonationtracker-7.5.0/eldonationtracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 00:35:34.000000 eldonationtracker-7.5.0/eldonationtracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-19 00:35:34.000000 eldonationtracker-7.5.0/eldonationtracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-19 00:35:34.000000 eldonationtracker-7.5.0/eldonationtracker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-19 00:35:34.606238 eldonationtracker-7.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-19 00:35:18.000000 eldonationtracker-7.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.699575 eldonationtracker-8.0.0/eldonationtracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.703575 eldonationtracker-8.0.0/eldonationtracker/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/donation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/donor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9293 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/api/team_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53391 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.703575 eldonationtracker-8.0.0/eldonationtracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/test_donation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/test_donor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/test_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21155 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/tests/test_team_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/eldonationtracker/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/call_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/call_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/call_main_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/call_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/call_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20314 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/main_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/ui/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/eldonationtracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21212 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/utils/extralife_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/eldonationtracker/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24415 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/utils/tests/test_extralife_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/utils/tests/test_update_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/eldonationtracker/utils/update_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/eldonationtracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-20 20:16:28.000000 eldonationtracker-8.0.0/eldonationtracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-20 20:16:28.000000 eldonationtracker-8.0.0/eldonationtracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:16:28.000000 eldonationtracker-8.0.0/eldonationtracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 20:16:28.000000 eldonationtracker-8.0.0/eldonationtracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 20:16:28.000000 eldonationtracker-8.0.0/eldonationtracker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-20 20:16:28.707575 eldonationtracker-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 20:16:20.000000 eldonationtracker-8.0.0/setup.py
```

### Comparing `eldonationtracker-7.5.0/LICENSE` & `eldonationtracker-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/PKG-INFO` & `eldonationtracker-8.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: eldonationtracker
-Version: 7.5.0
+Version: 8.0.0
 Summary: A Python-based donation tracker for Extra Life streams
 Home-page: http://djotaku.github.io/ELDonationTracker/
 Author: Eric Mesa
 Author-email: eric@ericmesa.com
 License: GPLv3
 Keywords: extra life,XSplit,obs,livestreaming,video games
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: xdgenvpy==2.3.5
+Requires-Dist: pyqt6==6.6.1
+Requires-Dist: semver==3.0.2
+Requires-Dist: requests==2.28.1
+Requires-Dist: rich==12.6.0
+Requires-Dist: donordrivepython==1.6.0
 
 =================
 eldonationtracker
 =================
```

### Comparing `eldonationtracker-7.5.0/README.md` & `eldonationtracker-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/api/badge.py` & `eldonationtracker-8.0.0/eldonationtracker/api/badge.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/api/donation.py` & `eldonationtracker-8.0.0/eldonationtracker/api/donation.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/api/donor.py` & `eldonationtracker-8.0.0/eldonationtracker/api/donor.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/api/participant.py` & `eldonationtracker-8.0.0/eldonationtracker/api/participant.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/api/team.py` & `eldonationtracker-8.0.0/eldonationtracker/api/team.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/api/team_participant.py` & `eldonationtracker-8.0.0/eldonationtracker/api/team_participant.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/cli.py` & `eldonationtracker-8.0.0/eldonationtracker/cli.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/icon.png` & `eldonationtracker-8.0.0/eldonationtracker/icon.png`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/tests/test_badge.py` & `eldonationtracker-8.0.0/eldonationtracker/tests/test_badge.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/tests/test_donation.py` & `eldonationtracker-8.0.0/eldonationtracker/tests/test_donation.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/tests/test_donor.py` & `eldonationtracker-8.0.0/eldonationtracker/tests/test_donor.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/tests/test_participant.py` & `eldonationtracker-8.0.0/eldonationtracker/tests/test_participant.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/tests/test_team.py` & `eldonationtracker-8.0.0/eldonationtracker/tests/test_team.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/tests/test_team_participant.py` & `eldonationtracker-8.0.0/eldonationtracker/tests/test_team_participant.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/about.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/about.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file '../QTdesignerfiles/about.ui'
+# Form implementation generated from reading ui file 'about.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.2
+# Created by: PyQt6 UI code generator 6.6.1
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Dialog(object):
+class Ui_Dialog:
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
         Dialog.resize(400, 300)
-        self.textBrowser = QtWidgets.QTextBrowser(Dialog)
+        self.textBrowser = QtWidgets.QTextBrowser(parent=Dialog)
         self.textBrowser.setGeometry(QtCore.QRect(10, 10, 381, 231))
         self.textBrowser.setAutoFillBackground(True)
         self.textBrowser.setStyleSheet("background-color: rgba(255, 255, 255, 0);")
-        self.textBrowser.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.textBrowser.setFrameShadow(QtWidgets.QFrame.Plain)
-        self.textBrowser.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-        self.textBrowser.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        self.textBrowser.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.textBrowser.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
+        self.textBrowser.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self.textBrowser.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         self.textBrowser.setReadOnly(True)
         self.textBrowser.setOpenExternalLinks(True)
         self.textBrowser.setObjectName("textBrowser")
-        self.pushButton_OK = QtWidgets.QPushButton(Dialog)
+        self.pushButton_OK = QtWidgets.QPushButton(parent=Dialog)
         self.pushButton_OK.setGeometry(QtCore.QRect(150, 260, 80, 22))
         self.pushButton_OK.setObjectName("pushButton_OK")
 
         self.retranslateUi(Dialog)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
 
     def retranslateUi(self, Dialog):
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/call_logs.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/call_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains the programming logic for the settings window in the GUI."""
 
 import logging
 
-from PyQt5.QtWidgets import QDialog
+from PyQt6.QtWidgets import QDialog
 
 from eldonationtracker import file_logging
 from eldonationtracker.ui.logs import *
 
 # logging
 call_logs_log = logging.getLogger("logs")
 call_logs_log.addHandler(file_logging)
@@ -31,15 +31,15 @@
         self.timer.timeout.connect(self.update_log)
         self.timer.start()
 
         self.ui.copy.clicked.connect(self.copy_clipboard)
 
     def update_log(self):
         try:
-            with open("eldonationtracker_log.txt", 'r') as file:
+            with open("eldonationtracker_log.txt") as file:
                 log = file.read()
                 self.ui.logs.setText(log)
         except FileNotFoundError:
             call_logs_log.error("Couldn't find log file.")
             self.ui.logs.setText("Log file not found")
 
     def copy_clipboard(self):
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/call_main_gui.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/call_main_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 """The main GUI window."""
 
 import logging
 import sys
 import webbrowser
 
-from PyQt5 import QtCore
-from PyQt5.QtWidgets import (QApplication, QInputDialog, QMainWindow,
+from PyQt6 import QtCore
+from PyQt6.QtWidgets import (QApplication, QInputDialog, QMainWindow,
                              QMessageBox)
 
 import eldonationtracker.api.participant as participant
 import eldonationtracker.utils.update_available
 from eldonationtracker import file_logging
 from eldonationtracker.ui import (call_about, call_logs, call_settings,
                                   call_tracker)
@@ -132,15 +132,15 @@
     @staticmethod
     def dead_button():
         GUI_log.info("[bold blue]not working yet[/bold blue]")
 
     @staticmethod
     def read_files(folders, files):
         try:
-            with open(f'{folders}/{files}', 'r', encoding='utf8') as f:
+            with open(f'{folders}/{files}', encoding='utf8') as f:
                 text = f.read()
             return text
         except FileNotFoundError:
             GUI_log.error(f"""[bold magenta]GUI Error:
                 {folders}/{files} does not exist.
                 Did you update the settings?
                 Did you hit the 'run' button?[/bold magenta]
@@ -154,20 +154,20 @@
         self.RecentDonations.setPlainText(self.read_files(self.folders, 'lastNDonationNameAmts.txt'))
         self.LastDonation.setPlainText(self.read_files(self.folders, 'LastDonationNameAmnt.txt'))
         self.TopDonation.setPlainText(self.read_files(self.folders, 'TopDonorNameAmnt.txt'))
         self.TotalRaised.setPlainText(self.read_files(self.folders, 'totalRaised.txt'))
         self.TotalNumDonations.setPlainText(self.read_files(self.folders, 'numDonations.txt'))
         self.Goal.setPlainText(self.read_files(self.folders, 'goal.txt'))
         self.AvgDonation.setPlainText(self.read_files(self.folders, 'averageDonation.txt'))
-        try:
-            avatar_url = QtCore.QUrl.fromLocalFile(f'{self.folders}/Participant_Avatar.html')
-
-            self.participant_avatar.setUrl(avatar_url)
-        except FileNotFoundError:
-            GUI_log.warning("[bold blue] Participant Avatar not found. After running you should have it.[/bold blue]")
+        # try:
+        #     avatar_url = QtCore.QUrl.fromLocalFile(f'{self.folders}/Participant_Avatar.html')
+        #
+        #     self.participant_avatar.setUrl(avatar_url)
+        # except FileNotFoundError:
+        #     GUI_log.warning("[bold blue] Participant Avatar not found. After running you should have it.[/bold blue]")
 
         # Team Info
         if self.participant_conf.get_if_in_team():
             self.label_TeamCaptain.setText(self.read_files(self.folders, 'Team_captain.txt'))
             self.label_TeamGoal.setText(self.read_files(self.folders, 'Team_goal.txt'))
             self.label_TeamNumDonations.setText(self.read_files(self.folders, 'Team_numDonations.txt'))
             self.label_TeamTotalRaised.setText(self.read_files(self.folders, 'Team_totalRaised.txt'))
@@ -210,12 +210,12 @@
         self.call_about.show()
 
 
 def main():
     app = QApplication(sys.argv)  # A new instance of QApplication
     form = ELDonationGUI()  # We set the form to be our ELDonationGUI (design)
     form.show()  # Show the form
-    app.exec_()  # and execute the app
+    app.exec()  # and execute the app
 
 
 if __name__ == '__main__':  # if we're running file directly and not importing it
     main()  # run the main function
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/call_settings.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/call_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Contains the programming logic for the settings window in the GUI."""
 
 import logging
 
-from PyQt5.QtGui import QColor, QFont
-from PyQt5.QtWidgets import (QColorDialog, QDialog, QFileDialog, QFontDialog,
+from PyQt6.QtGui import QColor, QFont
+from PyQt6.QtWidgets import (QColorDialog, QDialog, QFileDialog, QFontDialog,
                              QMessageBox)
 
 from eldonationtracker import base_api_url, file_logging
 from eldonationtracker.ui.settings import *
 from eldonationtracker.utils import extralife_io
 
 # logging
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/call_tracker.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/call_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """A window that displays the last donation. Useful during streaming."""
 
 
 import logging
 import pathlib
 
-from PyQt5.QtCore import QUrl
-from PyQt5.QtGui import QColor, QFont
-from PyQt5.QtMultimedia import QMediaContent, QMediaPlayer  # type: ignore
-from PyQt5.QtWidgets import QDialog, QGraphicsPixmapItem, QGraphicsScene
+from PyQt6.QtCore import QUrl
+from PyQt6.QtGui import QColor, QFont
+from PyQt6.QtMultimedia import QAudioOutput, QMediaPlayer  # type: ignore
+from PyQt6.QtWidgets import QDialog, QGraphicsPixmapItem, QGraphicsScene
 
 from eldonationtracker import file_logging
 from eldonationtracker.ui.tracker import *
 
 # logging
 call_tracker_log = logging.getLogger("Call_Tracker")
 call_tracker_log.setLevel(logging.INFO)
@@ -56,15 +56,20 @@
                                                  self.tracker_background_color_value[2],
                                                  self.tracker_background_color_value[3])
             self.ui.graphicsView.setBackgroundBrush(self.tracker_background_color)
         self.scene = QGraphicsScene(self)
         self.pixmap = QtGui.QPixmap()
         self._load_image()
         self.ui.graphicsView.setScene(self.scene)
+        # audio
         self.donation_player = QMediaPlayer()
+        self.audioOutput = QAudioOutput()
+        print()
+        self.donation_player.setAudioOutput(self.audioOutput)
+        self.audioOutput.setVolume(50)
         self._load_sound()
         # timer to update the main text
         self.timer = QtCore.QTimer(self)
         self.timer.setSingleShot(False)
         self.timer.setInterval(15000)  # milliseconds
         self.timer.timeout.connect(self._load_and_unload)
         self.timer.start()
@@ -72,16 +77,16 @@
     def _load_image(self):
         self.tracker_image = self.participant_conf.get_tracker_image()
         self.pixmap.load(self.tracker_image)
         self.item = QGraphicsPixmapItem(self.pixmap.scaledToHeight(131))
 
     def _load_sound(self):
         sound_to_play = self.participant_conf.get_tracker_sound()
-        self.donation_sound = QMediaContent(QUrl.fromLocalFile(sound_to_play))
-        self.donation_player.setMedia(self.donation_sound)
+        self.donation_sound = QUrl.fromLocalFile(sound_to_play)
+        self.donation_player.setSource(self.donation_sound)
 
     def _load_and_unload_helper(self):
         """Used both by the test code and the actual load and unload code."""
         call_tracker_log.debug("The load and unload helper was called.")
         self._load_image()
         self._load_elements()
         self._load_sound()
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/logs.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/logs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file 'QTdesignerfiles/logs.ui'
+# Form implementation generated from reading ui file 'logs.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.0
+# Created by: PyQt6 UI code generator 6.6.1
 #
-# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Form(object):
+class Ui_Form:
     def setupUi(self, Form):
         Form.setObjectName("Form")
         Form.resize(740, 777)
-        self.copy = QtWidgets.QPushButton(Form)
+        self.copy = QtWidgets.QPushButton(parent=Form)
         self.copy.setGeometry(QtCore.QRect(10, 10, 121, 31))
         self.copy.setObjectName("copy")
-        self.logs = QtWidgets.QTextBrowser(Form)
+        self.logs = QtWidgets.QTextBrowser(parent=Form)
         self.logs.setGeometry(QtCore.QRect(10, 50, 721, 721))
         self.logs.setObjectName("logs")
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
     def retranslateUi(self, Form):
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/main_gui.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/main_gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,260 +1,247 @@
-# -*- coding: utf-8 -*-
-
 # Form implementation generated from reading ui file 'QTdesignerfiles/design.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.0
+# Created by: PyQt6 UI code generator 6.6.1
 #
-# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_MainWindow(object):
+class Ui_MainWindow:
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
-        MainWindow.resize(789, 749)
+        MainWindow.resize(789, 778)
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap("QTdesignerfiles/icon.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon.addPixmap(QtGui.QPixmap("QTdesignerfiles/icon.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         MainWindow.setWindowIcon(icon)
-        self.centralwidget = QtWidgets.QWidget(MainWindow)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.centralwidget.sizePolicy().hasHeightForWidth())
         self.centralwidget.setSizePolicy(sizePolicy)
         self.centralwidget.setObjectName("centralwidget")
-        self.ParticipantInfo = QtWidgets.QGroupBox(self.centralwidget)
+        self.ParticipantInfo = QtWidgets.QGroupBox(parent=self.centralwidget)
         self.ParticipantInfo.setGeometry(QtCore.QRect(10, 60, 301, 301))
         self.ParticipantInfo.setObjectName("ParticipantInfo")
-        self.gridLayoutWidget_2 = QtWidgets.QWidget(self.ParticipantInfo)
+        self.gridLayoutWidget_2 = QtWidgets.QWidget(parent=self.ParticipantInfo)
         self.gridLayoutWidget_2.setGeometry(QtCore.QRect(10, 20, 281, 295))
         self.gridLayoutWidget_2.setObjectName("gridLayoutWidget_2")
         self.gridLayout = QtWidgets.QGridLayout(self.gridLayoutWidget_2)
-        self.gridLayout.setSizeConstraint(QtWidgets.QLayout.SetFixedSize)
+        self.gridLayout.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetFixedSize)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setVerticalSpacing(6)
         self.gridLayout.setObjectName("gridLayout")
-        self.label_avg_donations = QtWidgets.QLabel(self.gridLayoutWidget_2)
-        self.label_avg_donations.setAlignment(QtCore.Qt.AlignCenter)
-        self.label_avg_donations.setObjectName("label_avg_donations")
-        self.gridLayout.addWidget(self.label_avg_donations, 3, 1, 1, 1)
-        self.TotalRaised = QtWidgets.QTextBrowser(self.gridLayoutWidget_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.TotalRaised.sizePolicy().hasHeightForWidth())
-        self.TotalRaised.setSizePolicy(sizePolicy)
-        self.TotalRaised.setMaximumSize(QtCore.QSize(100, 50))
-        self.TotalRaised.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.TotalRaised.setObjectName("TotalRaised")
-        self.gridLayout.addWidget(self.TotalRaised, 4, 0, 1, 1)
-        self.label_totalraised = QtWidgets.QLabel(self.gridLayoutWidget_2)
-        self.label_totalraised.setAlignment(QtCore.Qt.AlignCenter)
-        self.label_totalraised.setObjectName("label_totalraised")
-        self.gridLayout.addWidget(self.label_totalraised, 3, 0, 1, 1)
-        self.participant_avatar = QtWebEngineWidgets.QWebEngineView(self.gridLayoutWidget_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.participant_avatar.sizePolicy().hasHeightForWidth())
-        self.participant_avatar.setSizePolicy(sizePolicy)
-        self.participant_avatar.setAutoFillBackground(False)
-        self.participant_avatar.setUrl(QtCore.QUrl("about:blank"))
-        self.participant_avatar.setZoomFactor(0.63)
-        self.participant_avatar.setObjectName("participant_avatar")
-        self.gridLayout.addWidget(self.participant_avatar, 0, 0, 1, 1)
-        self.AvgDonation = QtWidgets.QTextBrowser(self.gridLayoutWidget_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        self.label_total_num_donations = QtWidgets.QLabel(parent=self.gridLayoutWidget_2)
+        self.label_total_num_donations.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.label_total_num_donations.setObjectName("label_total_num_donations")
+        self.gridLayout.addWidget(self.label_total_num_donations, 1, 1, 1, 1)
+        self.AvgDonation = QtWidgets.QTextBrowser(parent=self.gridLayoutWidget_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.AvgDonation.sizePolicy().hasHeightForWidth())
         self.AvgDonation.setSizePolicy(sizePolicy)
         self.AvgDonation.setMaximumSize(QtCore.QSize(100, 50))
-        self.AvgDonation.setFrameShape(QtWidgets.QFrame.NoFrame)
+        self.AvgDonation.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.AvgDonation.setObjectName("AvgDonation")
         self.gridLayout.addWidget(self.AvgDonation, 4, 1, 1, 1)
-        self.label_total_num_donations = QtWidgets.QLabel(self.gridLayoutWidget_2)
-        self.label_total_num_donations.setAlignment(QtCore.Qt.AlignCenter)
-        self.label_total_num_donations.setObjectName("label_total_num_donations")
-        self.gridLayout.addWidget(self.label_total_num_donations, 1, 1, 1, 1)
-        self.label_goal = QtWidgets.QLabel(self.gridLayoutWidget_2)
-        self.label_goal.setAlignment(QtCore.Qt.AlignCenter)
-        self.label_goal.setObjectName("label_goal")
-        self.gridLayout.addWidget(self.label_goal, 1, 0, 1, 1)
-        self.TotalNumDonations = QtWidgets.QTextBrowser(self.gridLayoutWidget_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        self.TotalRaised = QtWidgets.QTextBrowser(parent=self.gridLayoutWidget_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.TotalNumDonations.sizePolicy().hasHeightForWidth())
-        self.TotalNumDonations.setSizePolicy(sizePolicy)
-        self.TotalNumDonations.setMaximumSize(QtCore.QSize(100, 50))
-        self.TotalNumDonations.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.TotalNumDonations.setObjectName("TotalNumDonations")
-        self.gridLayout.addWidget(self.TotalNumDonations, 2, 1, 1, 1)
-        self.Goal = QtWidgets.QTextBrowser(self.gridLayoutWidget_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHeightForWidth(self.TotalRaised.sizePolicy().hasHeightForWidth())
+        self.TotalRaised.setSizePolicy(sizePolicy)
+        self.TotalRaised.setMaximumSize(QtCore.QSize(100, 50))
+        self.TotalRaised.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.TotalRaised.setObjectName("TotalRaised")
+        self.gridLayout.addWidget(self.TotalRaised, 4, 0, 1, 1)
+        self.label_avg_donations = QtWidgets.QLabel(parent=self.gridLayoutWidget_2)
+        self.label_avg_donations.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.label_avg_donations.setObjectName("label_avg_donations")
+        self.gridLayout.addWidget(self.label_avg_donations, 3, 1, 1, 1)
+        self.Goal = QtWidgets.QTextBrowser(parent=self.gridLayoutWidget_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.Goal.sizePolicy().hasHeightForWidth())
         self.Goal.setSizePolicy(sizePolicy)
         self.Goal.setMaximumSize(QtCore.QSize(100, 50))
         self.Goal.setBaseSize(QtCore.QSize(0, 0))
-        self.Goal.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.Goal.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.Goal.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.Goal.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.Goal.setObjectName("Goal")
         self.gridLayout.addWidget(self.Goal, 2, 0, 1, 1)
-        spacerItem = QtWidgets.QSpacerItem(20, 115, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
+        spacerItem = QtWidgets.QSpacerItem(20, 115, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
         self.gridLayout.addItem(spacerItem, 0, 1, 1, 1)
-        self.DonationInfo = QtWidgets.QGroupBox(self.centralwidget)
+        self.label_goal = QtWidgets.QLabel(parent=self.gridLayoutWidget_2)
+        self.label_goal.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.label_goal.setObjectName("label_goal")
+        self.gridLayout.addWidget(self.label_goal, 1, 0, 1, 1)
+        self.label_totalraised = QtWidgets.QLabel(parent=self.gridLayoutWidget_2)
+        self.label_totalraised.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.label_totalraised.setObjectName("label_totalraised")
+        self.gridLayout.addWidget(self.label_totalraised, 3, 0, 1, 1)
+        self.TotalNumDonations = QtWidgets.QTextBrowser(parent=self.gridLayoutWidget_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.TotalNumDonations.sizePolicy().hasHeightForWidth())
+        self.TotalNumDonations.setSizePolicy(sizePolicy)
+        self.TotalNumDonations.setMaximumSize(QtCore.QSize(100, 50))
+        self.TotalNumDonations.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.TotalNumDonations.setObjectName("TotalNumDonations")
+        self.gridLayout.addWidget(self.TotalNumDonations, 2, 1, 1, 1)
+        self.DonationInfo = QtWidgets.QGroupBox(parent=self.centralwidget)
         self.DonationInfo.setGeometry(QtCore.QRect(330, 60, 451, 301))
         self.DonationInfo.setObjectName("DonationInfo")
-        self.label = QtWidgets.QLabel(self.DonationInfo)
+        self.label = QtWidgets.QLabel(parent=self.DonationInfo)
         self.label.setGeometry(QtCore.QRect(30, 140, 121, 16))
         self.label.setObjectName("label")
-        self.RecentDonations = QtWidgets.QTextBrowser(self.DonationInfo)
+        self.RecentDonations = QtWidgets.QTextBrowser(parent=self.DonationInfo)
         self.RecentDonations.setGeometry(QtCore.QRect(10, 160, 431, 101))
         self.RecentDonations.setAutoFillBackground(False)
         self.RecentDonations.setDocumentTitle("")
-        self.RecentDonations.setLineWrapMode(QtWidgets.QTextEdit.NoWrap)
+        self.RecentDonations.setLineWrapMode(QtWidgets.QTextEdit.LineWrapMode.NoWrap)
         self.RecentDonations.setObjectName("RecentDonations")
-        self.LastDonation = QtWidgets.QTextBrowser(self.DonationInfo)
+        self.LastDonation = QtWidgets.QTextBrowser(parent=self.DonationInfo)
         self.LastDonation.setGeometry(QtCore.QRect(10, 40, 431, 31))
         self.LastDonation.setAutoFillBackground(False)
-        self.LastDonation.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.LastDonation.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.LastDonation.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.LastDonation.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.LastDonation.setObjectName("LastDonation")
-        self.label_2 = QtWidgets.QLabel(self.DonationInfo)
+        self.label_2 = QtWidgets.QLabel(parent=self.DonationInfo)
         self.label_2.setGeometry(QtCore.QRect(10, 20, 81, 16))
         self.label_2.setObjectName("label_2")
-        self.label_3 = QtWidgets.QLabel(self.DonationInfo)
+        self.label_3 = QtWidgets.QLabel(parent=self.DonationInfo)
         self.label_3.setGeometry(QtCore.QRect(10, 80, 81, 16))
         self.label_3.setObjectName("label_3")
-        self.TopDonation = QtWidgets.QTextBrowser(self.DonationInfo)
+        self.TopDonation = QtWidgets.QTextBrowser(parent=self.DonationInfo)
         self.TopDonation.setGeometry(QtCore.QRect(10, 100, 431, 31))
-        self.TopDonation.setFrameShape(QtWidgets.QFrame.NoFrame)
+        self.TopDonation.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.TopDonation.setObjectName("TopDonation")
-        self.TeamGroupBox = QtWidgets.QGroupBox(self.centralwidget)
+        self.TeamGroupBox = QtWidgets.QGroupBox(parent=self.centralwidget)
         self.TeamGroupBox.setGeometry(QtCore.QRect(10, 370, 771, 291))
         self.TeamGroupBox.setObjectName("TeamGroupBox")
-        self.gridLayoutWidget = QtWidgets.QWidget(self.TeamGroupBox)
+        self.gridLayoutWidget = QtWidgets.QWidget(parent=self.TeamGroupBox)
         self.gridLayoutWidget.setGeometry(QtCore.QRect(10, 30, 751, 251))
         self.gridLayoutWidget.setObjectName("gridLayoutWidget")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.gridLayoutWidget)
         self.gridLayout_2.setContentsMargins(0, 0, 0, 0)
         self.gridLayout_2.setObjectName("gridLayout_2")
-        spacerItem1 = QtWidgets.QSpacerItem(62, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
+        spacerItem1 = QtWidgets.QSpacerItem(62, 20, QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout_2.addItem(spacerItem1, 0, 0, 1, 1)
-        self.label_TeamTotalRaised = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_TeamTotalRaised.setAlignment(QtCore.Qt.AlignHCenter|QtCore.Qt.AlignTop)
+        self.label_TeamTotalRaised = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_TeamTotalRaised.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter|QtCore.Qt.AlignmentFlag.AlignTop)
         self.label_TeamTotalRaised.setObjectName("label_TeamTotalRaised")
         self.gridLayout_2.addWidget(self.label_TeamTotalRaised, 1, 4, 1, 1)
-        self.textBrowser_TeamTop5 = QtWidgets.QTextBrowser(self.gridLayoutWidget)
+        self.textBrowser_TeamTop5 = QtWidgets.QTextBrowser(parent=self.gridLayoutWidget)
         self.textBrowser_TeamTop5.setObjectName("textBrowser_TeamTop5")
         self.gridLayout_2.addWidget(self.textBrowser_TeamTop5, 3, 2, 1, 4)
-        self.label_TeamGoal = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_TeamGoal.setAlignment(QtCore.Qt.AlignHCenter|QtCore.Qt.AlignTop)
+        self.label_TeamGoal = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_TeamGoal.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter|QtCore.Qt.AlignmentFlag.AlignTop)
         self.label_TeamGoal.setObjectName("label_TeamGoal")
         self.gridLayout_2.addWidget(self.label_TeamGoal, 1, 2, 1, 1)
-        self.label_11 = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_11.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignHCenter)
+        self.label_11 = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_11.setAlignment(QtCore.Qt.AlignmentFlag.AlignBottom|QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.label_11.setObjectName("label_11")
         self.gridLayout_2.addWidget(self.label_11, 0, 5, 1, 1)
-        self.label_10 = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_10.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignHCenter)
+        self.label_10 = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_10.setAlignment(QtCore.Qt.AlignmentFlag.AlignBottom|QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.label_10.setObjectName("label_10")
         self.gridLayout_2.addWidget(self.label_10, 0, 2, 1, 1)
-        self.label_TeamNumDonations = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_TeamNumDonations.setAlignment(QtCore.Qt.AlignHCenter|QtCore.Qt.AlignTop)
+        self.label_TeamNumDonations = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_TeamNumDonations.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter|QtCore.Qt.AlignmentFlag.AlignTop)
         self.label_TeamNumDonations.setObjectName("label_TeamNumDonations")
         self.gridLayout_2.addWidget(self.label_TeamNumDonations, 1, 5, 1, 1)
-        self.label_12 = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_12.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignHCenter)
+        self.label_12 = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_12.setAlignment(QtCore.Qt.AlignmentFlag.AlignBottom|QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.label_12.setObjectName("label_12")
         self.gridLayout_2.addWidget(self.label_12, 0, 4, 1, 1)
-        self.label_13 = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_13.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignHCenter)
+        self.label_13 = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_13.setAlignment(QtCore.Qt.AlignmentFlag.AlignBottom|QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.label_13.setObjectName("label_13")
         self.gridLayout_2.addWidget(self.label_13, 2, 6, 1, 1)
-        spacerItem2 = QtWidgets.QSpacerItem(254, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
+        spacerItem2 = QtWidgets.QSpacerItem(254, 20, QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout_2.addItem(spacerItem2, 0, 6, 1, 1)
-        self.label_TeamCaptain = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_TeamCaptain.setAlignment(QtCore.Qt.AlignHCenter|QtCore.Qt.AlignTop)
+        self.label_TeamCaptain = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_TeamCaptain.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter|QtCore.Qt.AlignmentFlag.AlignTop)
         self.label_TeamCaptain.setObjectName("label_TeamCaptain")
         self.gridLayout_2.addWidget(self.label_TeamCaptain, 1, 1, 1, 1)
-        self.label_14 = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_14.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignHCenter)
+        self.label_14 = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_14.setAlignment(QtCore.Qt.AlignmentFlag.AlignBottom|QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.label_14.setObjectName("label_14")
         self.gridLayout_2.addWidget(self.label_14, 2, 4, 1, 1)
-        self.label_9 = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_9.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignHCenter)
+        self.label_9 = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_9.setAlignment(QtCore.Qt.AlignmentFlag.AlignBottom|QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.label_9.setObjectName("label_9")
         self.gridLayout_2.addWidget(self.label_9, 0, 1, 1, 1)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
         self.gridLayout_2.addItem(spacerItem3, 2, 1, 1, 1)
-        self.label_TopTeamParticipant = QtWidgets.QLabel(self.gridLayoutWidget)
-        self.label_TopTeamParticipant.setAlignment(QtCore.Qt.AlignHCenter|QtCore.Qt.AlignTop)
+        self.label_TopTeamParticipant = QtWidgets.QLabel(parent=self.gridLayoutWidget)
+        self.label_TopTeamParticipant.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter|QtCore.Qt.AlignmentFlag.AlignTop)
         self.label_TopTeamParticipant.setObjectName("label_TopTeamParticipant")
         self.gridLayout_2.addWidget(self.label_TopTeamParticipant, 3, 6, 1, 1)
-        self.pushButtonRun = QtWidgets.QPushButton(self.centralwidget)
+        self.pushButtonRun = QtWidgets.QPushButton(parent=self.centralwidget)
         self.pushButtonRun.setGeometry(QtCore.QRect(570, 670, 84, 31))
         self.pushButtonRun.setObjectName("pushButtonRun")
-        self.pushButtonStop = QtWidgets.QPushButton(self.centralwidget)
+        self.pushButtonStop = QtWidgets.QPushButton(parent=self.centralwidget)
         self.pushButtonStop.setGeometry(QtCore.QRect(670, 670, 84, 31))
         self.pushButtonStop.setObjectName("pushButtonStop")
-        self.CopyrightLabel = QtWidgets.QLabel(self.centralwidget)
+        self.CopyrightLabel = QtWidgets.QLabel(parent=self.centralwidget)
         self.CopyrightLabel.setGeometry(QtCore.QRect(30, 680, 481, 31))
         self.CopyrightLabel.setObjectName("CopyrightLabel")
-        self.layoutWidget = QtWidgets.QWidget(self.centralwidget)
+        self.layoutWidget = QtWidgets.QWidget(parent=self.centralwidget)
         self.layoutWidget.setGeometry(QtCore.QRect(10, 10, 771, 33))
         self.layoutWidget.setObjectName("layoutWidget")
         self.horizontalLayout = QtWidgets.QHBoxLayout(self.layoutWidget)
         self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.SettingsButton = QtWidgets.QPushButton(self.layoutWidget)
+        self.SettingsButton = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.SettingsButton.setAutoDefault(False)
         self.SettingsButton.setDefault(False)
         self.SettingsButton.setFlat(False)
         self.SettingsButton.setObjectName("SettingsButton")
         self.horizontalLayout.addWidget(self.SettingsButton)
-        self.TrackerButton = QtWidgets.QPushButton(self.layoutWidget)
+        self.TrackerButton = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.TrackerButton.setObjectName("TrackerButton")
         self.horizontalLayout.addWidget(self.TrackerButton)
-        self.ProgressBarButton = QtWidgets.QPushButton(self.layoutWidget)
+        self.ProgressBarButton = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.ProgressBarButton.setObjectName("ProgressBarButton")
         self.horizontalLayout.addWidget(self.ProgressBarButton)
-        self.RefreshButton = QtWidgets.QPushButton(self.layoutWidget)
+        self.RefreshButton = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.RefreshButton.setObjectName("RefreshButton")
         self.horizontalLayout.addWidget(self.RefreshButton)
-        self.TestAlertButton = QtWidgets.QPushButton(self.layoutWidget)
+        self.TestAlertButton = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.TestAlertButton.setObjectName("TestAlertButton")
         self.horizontalLayout.addWidget(self.TestAlertButton)
         MainWindow.setCentralWidget(self.centralwidget)
-        self.statusbar = QtWidgets.QStatusBar(MainWindow)
+        self.statusbar = QtWidgets.QStatusBar(parent=MainWindow)
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
-        self.menuBar = QtWidgets.QMenuBar(MainWindow)
-        self.menuBar.setGeometry(QtCore.QRect(0, 0, 789, 30))
+        self.menuBar = QtWidgets.QMenuBar(parent=MainWindow)
+        self.menuBar.setGeometry(QtCore.QRect(0, 0, 789, 32))
         self.menuBar.setObjectName("menuBar")
-        self.menuFile = QtWidgets.QMenu(self.menuBar)
+        self.menuFile = QtWidgets.QMenu(parent=self.menuBar)
         self.menuFile.setObjectName("menuFile")
-        self.menuHelp = QtWidgets.QMenu(self.menuBar)
+        self.menuHelp = QtWidgets.QMenu(parent=self.menuBar)
         self.menuHelp.setObjectName("menuHelp")
         MainWindow.setMenuBar(self.menuBar)
-        self.actionQuit = QtWidgets.QAction(MainWindow)
+        self.actionQuit = QtGui.QAction(parent=MainWindow)
         self.actionQuit.setObjectName("actionQuit")
-        self.actionDocumentation = QtWidgets.QAction(MainWindow)
+        self.actionDocumentation = QtGui.QAction(parent=MainWindow)
         self.actionDocumentation.setObjectName("actionDocumentation")
-        self.actionCheck_for_Update = QtWidgets.QAction(MainWindow)
+        self.actionCheck_for_Update = QtGui.QAction(parent=MainWindow)
         self.actionCheck_for_Update.setObjectName("actionCheck_for_Update")
-        self.actionAbout = QtWidgets.QAction(MainWindow)
+        self.actionAbout = QtGui.QAction(parent=MainWindow)
         self.actionAbout.setObjectName("actionAbout")
-        self.actionShow_Logs = QtWidgets.QAction(MainWindow)
+        self.actionShow_Logs = QtGui.QAction(parent=MainWindow)
         self.actionShow_Logs.setObjectName("actionShow_Logs")
         self.menuFile.addAction(self.actionShow_Logs)
         self.menuFile.addAction(self.actionQuit)
         self.menuHelp.addAction(self.actionDocumentation)
         self.menuHelp.addAction(self.actionCheck_for_Update)
         self.menuHelp.addAction(self.actionAbout)
         self.menuBar.addAction(self.menuFile.menuAction())
@@ -263,18 +250,18 @@
         self.retranslateUi(MainWindow)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "EL Donation Tracker"))
         self.ParticipantInfo.setTitle(_translate("MainWindow", "Participant Info"))
-        self.label_avg_donations.setText(_translate("MainWindow", "Average Donation"))
-        self.label_totalraised.setText(_translate("MainWindow", "Total Raised"))
         self.label_total_num_donations.setText(_translate("MainWindow", "Total # of Donations"))
+        self.label_avg_donations.setText(_translate("MainWindow", "Average Donation"))
         self.label_goal.setText(_translate("MainWindow", "Goal"))
+        self.label_totalraised.setText(_translate("MainWindow", "Total Raised"))
         self.DonationInfo.setTitle(_translate("MainWindow", "Participant Donation Info"))
         self.label.setText(_translate("MainWindow", "Recent Donations"))
         self.RecentDonations.setPlaceholderText(_translate("MainWindow", "Recent Donations"))
         self.LastDonation.setPlaceholderText(_translate("MainWindow", "Last Donation"))
         self.label_2.setText(_translate("MainWindow", "Last Donation"))
         self.label_3.setText(_translate("MainWindow", "Top Donor"))
         self.TopDonation.setPlaceholderText(_translate("MainWindow", "Top Donor"))
@@ -288,24 +275,23 @@
         self.label_13.setText(_translate("MainWindow", "Top Team Participant"))
         self.label_TeamCaptain.setText(_translate("MainWindow", "Team Captain"))
         self.label_14.setText(_translate("MainWindow", "Top 5 Team Participants"))
         self.label_9.setText(_translate("MainWindow", "Team Captain"))
         self.label_TopTeamParticipant.setText(_translate("MainWindow", "Top Team Participant"))
         self.pushButtonRun.setText(_translate("MainWindow", "Run"))
         self.pushButtonStop.setText(_translate("MainWindow", "Stop"))
-        self.CopyrightLabel.setText(_translate("MainWindow", "© 2015-2022 Eric Mesa; Licensed GPLv3; http://extralife.ericmesa.com"))
+        self.CopyrightLabel.setText(_translate("MainWindow", "© 2015-2024 Eric Mesa; Licensed GPLv3; http://extralife.ericmesa.com"))
         self.SettingsButton.setToolTip(_translate("MainWindow", "<html><head/><body><p>Change folders, Extra Life ID, etc</p></body></html>"))
         self.SettingsButton.setText(_translate("MainWindow", "Settings"))
         self.TrackerButton.setText(_translate("MainWindow", "Tracker"))
         self.ProgressBarButton.setText(_translate("MainWindow", "Progress Bar"))
         self.RefreshButton.setText(_translate("MainWindow", "Force Refresh"))
         self.TestAlertButton.setText(_translate("MainWindow", "Test Alert"))
-        self.menuFile.setTitle(_translate("MainWindow", "File"))
+        self.menuFile.setTitle(_translate("MainWindow", "Fi&le"))
         self.menuHelp.setTitle(_translate("MainWindow", "Help"))
-        self.actionQuit.setText(_translate("MainWindow", "Quit"))
-        self.actionDocumentation.setText(_translate("MainWindow", "Documentation"))
+        self.actionQuit.setText(_translate("MainWindow", "&Quit"))
+        self.actionDocumentation.setText(_translate("MainWindow", "&Documentation"))
         self.actionDocumentation.setToolTip(_translate("MainWindow", "Open Documentation in your default browser"))
-        self.actionCheck_for_Update.setText(_translate("MainWindow", "Check for Update"))
+        self.actionCheck_for_Update.setText(_translate("MainWindow", "&Check for Update"))
         self.actionCheck_for_Update.setToolTip(_translate("MainWindow", "Checks for Updates"))
-        self.actionAbout.setText(_translate("MainWindow", "About ELDonationTracker"))
-        self.actionShow_Logs.setText(_translate("MainWindow", "Show Logs"))
-from PyQt5 import QtWebEngineWidgets
+        self.actionAbout.setText(_translate("MainWindow", "&About ELDonationTracker"))
+        self.actionShow_Logs.setText(_translate("MainWindow", "&Show Logs"))
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/settings.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file 'QTdesignerfiles/settings.ui'
+# Form implementation generated from reading ui file 'settings.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.2
+# Created by: PyQt6 UI code generator 6.6.1
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Dialog(object):
+class Ui_Dialog:
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
         Dialog.resize(805, 392)
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap("QTdesignerfiles/icon.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon.addPixmap(QtGui.QPixmap("icon.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         Dialog.setWindowIcon(icon)
-        self.layoutWidget = QtWidgets.QWidget(Dialog)
+        self.layoutWidget = QtWidgets.QWidget(parent=Dialog)
         self.layoutWidget.setGeometry(QtCore.QRect(10, 0, 791, 381))
         self.layoutWidget.setObjectName("layoutWidget")
         self.gridLayout = QtWidgets.QGridLayout(self.layoutWidget)
-        self.gridLayout.setSizeConstraint(QtWidgets.QLayout.SetDefaultConstraint)
+        self.gridLayout.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetDefaultConstraint)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setVerticalSpacing(2)
         self.gridLayout.setObjectName("gridLayout")
-        self.label_6 = QtWidgets.QLabel(self.layoutWidget)
+        self.label_6 = QtWidgets.QLabel(parent=self.layoutWidget)
         self.label_6.setObjectName("label_6")
         self.gridLayout.addWidget(self.label_6, 6, 0, 1, 1)
-        self.pushButtonSelectFolder = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButtonSelectFolder = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButtonSelectFolder.setToolTip("")
         self.pushButtonSelectFolder.setObjectName("pushButtonSelectFolder")
         self.gridLayout.addWidget(self.pushButtonSelectFolder, 1, 3, 1, 2)
-        self.label_4 = QtWidgets.QLabel(self.layoutWidget)
-        self.label_4.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_4 = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.label_4.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_4.setObjectName("label_4")
         self.gridLayout.addWidget(self.label_4, 3, 0, 1, 1)
-        self.label_2 = QtWidgets.QLabel(self.layoutWidget)
-        self.label_2.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_2 = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.label_2.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_2.setObjectName("label_2")
         self.gridLayout.addWidget(self.label_2, 1, 0, 1, 1)
-        self.lineEditTeamID = QtWidgets.QLineEdit(self.layoutWidget)
+        self.lineEditTeamID = QtWidgets.QLineEdit(parent=self.layoutWidget)
         self.lineEditTeamID.setObjectName("lineEditTeamID")
         self.gridLayout.addWidget(self.lineEditTeamID, 3, 1, 1, 1)
-        self.label_tracker_image = QtWidgets.QLabel(self.layoutWidget)
-        self.label_tracker_image.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_tracker_image = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.label_tracker_image.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_tracker_image.setObjectName("label_tracker_image")
         self.gridLayout.addWidget(self.label_tracker_image, 5, 1, 1, 1)
-        self.lineEditParticipantID = QtWidgets.QLineEdit(self.layoutWidget)
+        self.lineEditParticipantID = QtWidgets.QLineEdit(parent=self.layoutWidget)
         self.lineEditParticipantID.setToolTip("")
         self.lineEditParticipantID.setToolTipDuration(5)
         self.lineEditParticipantID.setObjectName("lineEditParticipantID")
         self.gridLayout.addWidget(self.lineEditParticipantID, 0, 1, 1, 1)
-        self.pushButton_persistentsave = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_persistentsave = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_persistentsave.setObjectName("pushButton_persistentsave")
         self.gridLayout.addWidget(self.pushButton_persistentsave, 11, 2, 1, 3)
-        self.label_3 = QtWidgets.QLabel(self.layoutWidget)
+        self.label_3 = QtWidgets.QLabel(parent=self.layoutWidget)
         self.label_3.setObjectName("label_3")
         self.gridLayout.addWidget(self.label_3, 2, 0, 1, 1)
-        self.label_5 = QtWidgets.QLabel(self.layoutWidget)
+        self.label_5 = QtWidgets.QLabel(parent=self.layoutWidget)
         self.label_5.setObjectName("label_5")
         self.gridLayout.addWidget(self.label_5, 5, 0, 1, 1)
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        self.pushButton_font = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_font = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_font.setObjectName("pushButton_font")
         self.horizontalLayout_2.addWidget(self.pushButton_font)
-        self.pushButton_font_color = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_font_color = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_font_color.setObjectName("pushButton_font_color")
         self.horizontalLayout_2.addWidget(self.pushButton_font_color)
         self.gridLayout.addLayout(self.horizontalLayout_2, 8, 1, 1, 1)
-        self.lineEditCurrencySymbol = QtWidgets.QLineEdit(self.layoutWidget)
+        self.lineEditCurrencySymbol = QtWidgets.QLineEdit(parent=self.layoutWidget)
         self.lineEditCurrencySymbol.setObjectName("lineEditCurrencySymbol")
         self.gridLayout.addWidget(self.lineEditCurrencySymbol, 2, 1, 1, 1)
-        self.label = QtWidgets.QLabel(self.layoutWidget)
-        self.label.setAlignment(QtCore.Qt.AlignCenter)
+        self.label = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label.setObjectName("label")
         self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
-        self.labelTextFolder = QtWidgets.QLabel(self.layoutWidget)
-        self.labelTextFolder.setAlignment(QtCore.Qt.AlignCenter)
+        self.labelTextFolder = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.labelTextFolder.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.labelTextFolder.setObjectName("labelTextFolder")
         self.gridLayout.addWidget(self.labelTextFolder, 1, 1, 1, 2)
-        self.pushButton_tracker_background = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_tracker_background = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_tracker_background.setObjectName("pushButton_tracker_background")
         self.gridLayout.addWidget(self.pushButton_tracker_background, 9, 1, 1, 1)
-        self.label_sound = QtWidgets.QLabel(self.layoutWidget)
-        self.label_sound.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_sound = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.label_sound.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_sound.setObjectName("label_sound")
         self.gridLayout.addWidget(self.label_sound, 6, 1, 1, 1)
-        self.label_donors_to_display = QtWidgets.QLabel(self.layoutWidget)
+        self.label_donors_to_display = QtWidgets.QLabel(parent=self.layoutWidget)
         self.label_donors_to_display.setObjectName("label_donors_to_display")
         self.gridLayout.addWidget(self.label_donors_to_display, 4, 0, 1, 1)
-        self.spinBox_DonorsToDisplay = QtWidgets.QSpinBox(self.layoutWidget)
+        self.spinBox_DonorsToDisplay = QtWidgets.QSpinBox(parent=self.layoutWidget)
         self.spinBox_DonorsToDisplay.setObjectName("spinBox_DonorsToDisplay")
         self.gridLayout.addWidget(self.spinBox_DonorsToDisplay, 4, 1, 1, 1)
-        self.pushButton_tracker_image = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_tracker_image = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_tracker_image.setObjectName("pushButton_tracker_image")
         self.gridLayout.addWidget(self.pushButton_tracker_image, 5, 2, 1, 1)
-        self.pushButton_sound = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_sound = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_sound.setObjectName("pushButton_sound")
         self.gridLayout.addWidget(self.pushButton_sound, 6, 2, 1, 1)
-        self.pushButton_grab_image = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_grab_image = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_grab_image.setObjectName("pushButton_grab_image")
         self.gridLayout.addWidget(self.pushButton_grab_image, 5, 4, 1, 1)
-        self.pushButton_grab_sound = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_grab_sound = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_grab_sound.setObjectName("pushButton_grab_sound")
         self.gridLayout.addWidget(self.pushButton_grab_sound, 6, 4, 1, 1)
-        self.pushButton_validate_participant_id = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_validate_participant_id = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_validate_participant_id.setObjectName("pushButton_validate_participant_id")
         self.gridLayout.addWidget(self.pushButton_validate_participant_id, 0, 2, 1, 1)
-        self.pushButton_validate_team_id = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButton_validate_team_id = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButton_validate_team_id.setObjectName("pushButton_validate_team_id")
         self.gridLayout.addWidget(self.pushButton_validate_team_id, 3, 2, 1, 1)
-        self.pushButtonRevert = QtWidgets.QPushButton(self.layoutWidget)
+        self.pushButtonRevert = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.pushButtonRevert.setObjectName("pushButtonRevert")
         self.gridLayout.addWidget(self.pushButtonRevert, 10, 2, 1, 3)
 
         self.retranslateUi(Dialog)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
 
     def retranslateUi(self, Dialog):
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/ui/tracker.py` & `eldonationtracker-8.0.0/eldonationtracker/ui/tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file 'QTdesignerfiles/tracker.ui'
+# Form implementation generated from reading ui file 'tracker.ui'
 #
-# Created by: PyQt5 UI code generator 5.13.1
+# Created by: PyQt6 UI code generator 6.6.1
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Dialog(object):
+class Ui_Dialog:
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
         Dialog.setEnabled(True)
         Dialog.resize(985, 137)
         Dialog.setAutoFillBackground(False)
         Dialog.setStyleSheet("background: rgba(255, 255, 255, 0)\n"
 "")
-        self.graphicsView = QtWidgets.QGraphicsView(Dialog)
+        self.graphicsView = QtWidgets.QGraphicsView(parent=Dialog)
         self.graphicsView.setEnabled(True)
         self.graphicsView.setGeometry(QtCore.QRect(0, -10, 991, 151))
         self.graphicsView.setAutoFillBackground(False)
-        self.graphicsView.setFrameShape(QtWidgets.QFrame.NoFrame)
+        self.graphicsView.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.graphicsView.setLineWidth(0)
-        self.graphicsView.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-        self.graphicsView.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        self.graphicsView.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self.graphicsView.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         brush = QtGui.QBrush(QtGui.QColor(0, 170, 0))
-        brush.setStyle(QtCore.Qt.SolidPattern)
+        brush.setStyle(QtCore.Qt.BrushStyle.SolidPattern)
         self.graphicsView.setBackgroundBrush(brush)
         brush = QtGui.QBrush(QtGui.QColor(0, 0, 0))
-        brush.setStyle(QtCore.Qt.NoBrush)
+        brush.setStyle(QtCore.Qt.BrushStyle.NoBrush)
         self.graphicsView.setForegroundBrush(brush)
         self.graphicsView.setInteractive(False)
-        self.graphicsView.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.graphicsView.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.graphicsView.setObjectName("graphicsView")
-        self.Donation_label = QtWidgets.QTextEdit(Dialog)
+        self.Donation_label = QtWidgets.QTextEdit(parent=Dialog)
         self.Donation_label.setGeometry(QtCore.QRect(180, 0, 801, 131))
         font = QtGui.QFont()
         font.setPointSize(56)
         self.Donation_label.setFont(font)
         self.Donation_label.setAutoFillBackground(False)
         self.Donation_label.setStyleSheet("background: rgba(255, 255, 255, 0)\n"
 "")
-        self.Donation_label.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.Donation_label.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.Donation_label.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.Donation_label.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.Donation_label.setLineWidth(0)
-        self.Donation_label.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-        self.Donation_label.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        self.Donation_label.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self.Donation_label.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         self.Donation_label.setUndoRedoEnabled(False)
         self.Donation_label.setReadOnly(True)
         self.Donation_label.setObjectName("Donation_label")
 
         self.retranslateUi(Dialog)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker/utils/extralife_io.py` & `eldonationtracker-8.0.0/eldonationtracker/utils/extralife_io.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/utils/tests/test_extralife_io.py` & `eldonationtracker-8.0.0/eldonationtracker/utils/tests/test_extralife_io.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/utils/tests/test_update_available.py` & `eldonationtracker-8.0.0/eldonationtracker/utils/tests/test_update_available.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker/utils/update_available.py` & `eldonationtracker-8.0.0/eldonationtracker/utils/update_available.py`

 * *Files identical despite different names*

### Comparing `eldonationtracker-7.5.0/eldonationtracker.egg-info/PKG-INFO` & `eldonationtracker-8.0.0/eldonationtracker.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: eldonationtracker
-Version: 7.5.0
+Version: 8.0.0
 Summary: A Python-based donation tracker for Extra Life streams
 Home-page: http://djotaku.github.io/ELDonationTracker/
 Author: Eric Mesa
 Author-email: eric@ericmesa.com
 License: GPLv3
 Keywords: extra life,XSplit,obs,livestreaming,video games
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: xdgenvpy==2.3.5
+Requires-Dist: pyqt6==6.6.1
+Requires-Dist: semver==3.0.2
+Requires-Dist: requests==2.28.1
+Requires-Dist: rich==12.6.0
+Requires-Dist: donordrivepython==1.6.0
 
 =================
 eldonationtracker
 =================
```

### Comparing `eldonationtracker-7.5.0/eldonationtracker.egg-info/SOURCES.txt` & `eldonationtracker-8.0.0/eldonationtracker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pypi.rst
 setup.cfg
 setup.py
 eldonationtracker/__init__.py
 eldonationtracker/cli.py
 eldonationtracker/gui.py
 eldonationtracker/icon.png
 eldonationtracker.egg-info/PKG-INFO
```

### Comparing `eldonationtracker-7.5.0/setup.cfg` & `eldonationtracker-8.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -14,21 +14,17 @@
 	Programming Language :: Python :: 3
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
 	xdgenvpy == 2.3.5
-	PyQt5 == 5.15.7
-	PyQt5-Qt5==5.15.2
-	PyQt5-sip == 12.11.0
-	PyQtWebEngine==5.15.6
-	PyQtWebEngine-Qt5==5.15.2
-	semver == 3.0.0.dev3
+	pyqt6 == 6.6.1
+	semver == 3.0.2
 	requests == 2.28.1
-	rich == 12.4.4
-	donordrivepython == 1.5.0
+	rich == 12.6.0
+	donordrivepython == 1.6.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

