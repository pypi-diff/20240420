# Comparing `tmp/timetree-exporter-0.2.3.tar.gz` & `tmp/timetree_exporter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetree-exporter-0.2.3.tar", last modified: Wed Apr 10 12:03:13 2024, max compression
+gzip compressed data, was "timetree_exporter-0.3.0.tar", last modified: Sat Apr 20 15:28:49 2024, max compression
```

## Comparing `timetree-exporter-0.2.3.tar` & `timetree_exporter-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.891560 timetree-exporter-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.891560 timetree-exporter-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/.github/workflows/release-please.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.891560 timetree-exporter-0.2.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.891560 timetree-exporter-0.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.891560 timetree-exporter-0.2.3/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/docs/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/docs/assets/images/copy-response.png
--rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/docs/assets/images/prepare-for-signin.png
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/responses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/timetree_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/timetree_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/timetree_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/timetree_exporter/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/timetree_exporter/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-10 12:03:08.000000 timetree-exporter-0.2.3/timetree_exporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:03:13.895560 timetree-exporter-0.2.3/timetree_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-10 12:03:13.000000 timetree-exporter-0.2.3/timetree_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-10 12:03:13.000000 timetree-exporter-0.2.3/timetree_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:03:13.000000 timetree-exporter-0.2.3/timetree_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 12:03:13.000000 timetree-exporter-0.2.3/timetree_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 12:03:13.000000 timetree-exporter-0.2.3/timetree_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 12:03:13.000000 timetree-exporter-0.2.3/timetree_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.928650 timetree_exporter-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.924650 timetree_exporter-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.924650 timetree_exporter-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-20 15:28:49.928650 timetree_exporter-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.924650 timetree_exporter-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.924650 timetree_exporter-0.3.0/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.924650 timetree_exporter-0.3.0/docs/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/docs/assets/images/copy-response.png
+-rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/docs/assets/images/prepare-for-signin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.924650 timetree_exporter-0.3.0/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/responses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:28:49.928650 timetree_exporter-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.928650 timetree_exporter-0.3.0/timetree_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/timetree_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/timetree_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/timetree_exporter/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/timetree_exporter/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-20 15:28:45.000000 timetree_exporter-0.3.0/timetree_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:49.928650 timetree_exporter-0.3.0/timetree_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-20 15:28:49.000000 timetree_exporter-0.3.0/timetree_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-20 15:28:49.000000 timetree_exporter-0.3.0/timetree_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:28:49.000000 timetree_exporter-0.3.0/timetree_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-20 15:28:49.000000 timetree_exporter-0.3.0/timetree_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:28:49.000000 timetree_exporter-0.3.0/timetree_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 15:28:49.000000 timetree_exporter-0.3.0/timetree_exporter.egg-info/top_level.txt
```

### Comparing `timetree-exporter-0.2.3/.github/workflows/pylint.yml` & `timetree_exporter-0.3.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.3/.github/workflows/python-publish.yml` & `timetree_exporter-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.3/CHANGELOG.md` & `timetree_exporter-0.3.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Changelog
 
+## [0.3.0](https://github.com/eoleedi/TimeTree-Exporter/compare/v0.2.3...v0.3.0) (2024-04-20)
+
+
+### Features
+
+* parse category and skip memo ([#33](https://github.com/eoleedi/TimeTree-Exporter/issues/33)) ([0166f6f](https://github.com/eoleedi/TimeTree-Exporter/commit/0166f6f53284927b89a9a830e830f9d8318877e9))
+
+
+### Bug Fixes
+
+* add __version__ attribute in the package ([d3ed38f](https://github.com/eoleedi/TimeTree-Exporter/commit/d3ed38f67cf73c9f15025f2078d5454b4c372132))
+
+
+### Reverts
+
+* add version in attribute in package ([ec0960b](https://github.com/eoleedi/TimeTree-Exporter/commit/ec0960b686b8e290209f89427a4d815911ac139b))
+
 ## [0.2.3](https://github.com/eoleedi/TimeTree-exporter/compare/v0.2.2...v0.2.3) (2024-04-10)
 
 
 ### Documentation
 
 * move assets into docs folder ([2931fb2](https://github.com/eoleedi/TimeTree-exporter/commit/2931fb212f2e78f89ba849ee6510b237c5372db3))
```

### Comparing `timetree-exporter-0.2.3/LICENSE` & `timetree_exporter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.3/PKG-INFO` & `timetree_exporter-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
 Project-URL: Changelog, https://github.com/eoleedi/TimeTree-exporter/blob/main/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
@@ -72,15 +72,15 @@
 Currently, TimeTree data can only be downloaded manually through a web browser.
 
 # Roadmap of the properties mapping to iCal
 - [ ] **ID**
 - [ ] **Primary ID**
 - [ ] **Calendar ID**
 - [x] **UUID**
-- [ ] **Category**
+- [x] **Category**
 - [x] **Type**
 - [ ] **Author ID**
 - [ ] **Author Type**
 - [x] **Title**
 - [x] **All Day**
 - [x] **Start At**
 - [x] **Start Timezone**
```

### Comparing `timetree-exporter-0.2.3/README.md` & `timetree_exporter-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 Currently, TimeTree data can only be downloaded manually through a web browser.
 
 # Roadmap of the properties mapping to iCal
 - [ ] **ID**
 - [ ] **Primary ID**
 - [ ] **Calendar ID**
 - [x] **UUID**
-- [ ] **Category**
+- [x] **Category**
 - [x] **Type**
 - [ ] **Author ID**
 - [ ] **Author Type**
 - [x] **Title**
 - [x] **All Day**
 - [x] **Start At**
 - [x] **Start Timezone**
```

### Comparing `timetree-exporter-0.2.3/docs/assets/images/copy-response.png` & `timetree_exporter-0.3.0/docs/assets/images/copy-response.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.3/docs/assets/images/prepare-for-signin.png` & `timetree_exporter-0.3.0/docs/assets/images/prepare-for-signin.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.3/pyproject.toml` & `timetree_exporter-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,29 @@
 
 [tool.setuptools.packages.find]
 include = ["timetree_exporter"]
 
 [project]
 name = "timetree-exporter"
 dynamic = ["version"]
-authors = [
-  { name="Fong-Chun Tsai", email="eoleedimin@gmail.com" },
-]
+authors = [{ name = "Fong-Chun Tsai", email = "eoleedimin@gmail.com" }]
 description = "A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)"
 keywords = ["timetree", "exporter", "icalendar", "ics"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "icalendar",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
+dependencies = ["icalendar"]
 
 [project.urls]
 Homepage = "https://github.com/eoleedi/TimeTree-Exporter"
 Repository = "https://github.com/eoleedi/TimeTree-Exporter"
 Issues = "https://github.com/eoleedi/TimeTree-Exporter/issues"
 Changelog = "https://github.com/eoleedi/TimeTree-exporter/blob/main/CHANGELOG.md"
 
 [project.scripts]
 timetree-exporter = "timetree_exporter.__main__:main"
 
-[tool.setuptools_scm]
+[tool.setuptools_scm]
```

### Comparing `timetree-exporter-0.2.3/responses/README.md` & `timetree_exporter-0.3.0/responses/README.md`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.3/timetree_exporter/__main__.py` & `timetree_exporter-0.3.0/timetree_exporter/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """
 This module converts Timetree events to iCal format.
 It is intended to be used with the Timetree API response files.
 https://timetreeapp.com/api/v1/calendar/{calendar_id}/events/sync
 """
 
 import argparse
+import logging
+import os
 from icalendar import Calendar
 from timetree_exporter import TimeTreeEvent, ICalEventFormatter
 from timetree_exporter.utils import get_events_from_file, paths_to_filelist
 
 
+logger = logging.getLogger(__name__)
+package_logger = logging.getLogger(__package__)
+
+
 def main():
     """Main function for the Timetree Exporter."""
     # Parse arguments
     parser = argparse.ArgumentParser(
         description="Convert Timetree events to iCal format",
         prog="timetree_exporter",
     )
@@ -26,40 +32,61 @@
     parser.add_argument(
         "-o",
         "--output",
         type=str,
         help="Path to the output iCal file",
         default="timetree.ics",
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        help="Increase output verbosity",
+        action="store_true",
+    )
     args = parser.parse_args()
 
+    # Set logging level
+    if args.verbose:
+        package_logger.setLevel(logging.DEBUG)
+
     cal = Calendar()
     filenames = paths_to_filelist(args.input)
+    imported_events_count = 0
 
     for filename in filenames:
         # Skip non-JSON files
         if not filename.endswith(".json"):
-            print(f"Skipping {filename} (Invalid file type, should be .json)")
+            logger.warning("Skipping %s (Invalid file type, should be .json)", filename)
             continue
-        print(f"Parsing {filename}")
+        logger.info("Parsing %s", filename)
 
         # Get events from file
         events = get_events_from_file(filename)
         if events is None:
             continue
 
+        imported_events_count += len(events)
+
         # Add events to calendar
         for event in events:
             time_tree_event = TimeTreeEvent.from_dict(event)
             formatter = ICalEventFormatter(time_tree_event)
             ical_event = formatter.to_ical()
             if ical_event is None:
                 continue
             cal.add_component(ical_event)
+    logger.info(
+        "A Total of %d/%d events added to the calendar",
+        len(cal.subcomponents),
+        imported_events_count,
+    )
 
     # Write calendar to file
     with open(args.output, "wb") as f:  # Path Traversal Vulnerability if on a server
         f.write(cal.to_ical())
+        logger.info(
+            "The .ics calendar file is saved to %s", os.path.abspath(args.output)
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `timetree-exporter-0.2.3/timetree_exporter/event.py` & `timetree_exporter-0.3.0/timetree_exporter/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         start_timezone: str,
         end_timezone: str,
         location_lat: str,
         location_lon: str,
         location: str,
         parent_id: str,
         event_type: int,
+        category: int,
     ):
         # pylint: disable=too-many-arguments
         # pylint: disable=too-many-locals
         self.uuid = uuid
         self.title = title
         self.created_at = created_at
         self.updated_at = updated_at
@@ -45,14 +46,15 @@
         self.end_at = end_at
         self.end_timezone = end_timezone
         self.all_day = all_day
         self.alerts = alerts
         self.recurrences = recurrences
         self.parent_id = parent_id
         self.event_type = event_type
+        self.category =  category
 
     @classmethod
     def from_dict(cls, event_data: dict):
         """Create TimeTreeEvent object from JSON data"""
         return cls(
             uuid=event_data.get("uuid"),
             title=event_data.get("title"),
@@ -68,19 +70,28 @@
             end_at=event_data.get("end_at"),
             end_timezone=event_data.get("end_timezone"),
             all_day=event_data.get("all_day"),
             alerts=event_data.get("alerts"),
             recurrences=event_data.get("recurrences"),
             parent_id=event_data.get("parent_id"),
             event_type=event_data.get("type"),
+            category=event_data.get("category"),
         )
 
     def __str__(self):
         return self.title
 
 
 @dataclasses.dataclass
 class TimeTreeEventType(enumerate):
     """TimeTree event type enumeration"""
 
     NORMAL = 0
     BIRTHDAY = 1
+
+
+@dataclasses.dataclass
+class TimeTreeEventCategory(enumerate):
+    """TimeTree event category enumeration"""
+
+    NORMAL = 1
+    MEMO = 2
```

### Comparing `timetree-exporter-0.2.3/timetree_exporter/formatter.py` & `timetree_exporter-0.3.0/timetree_exporter/formatter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """
 This module provides the ICalEventFormatter class 
 for formatting TimeTree events into iCalendar format.
 """
 
+import logging
 from datetime import datetime, timedelta
 from icalendar import Event, vRecur, vDate, vDatetime, vGeo
 from icalendar.prop import vDDDLists
 from icalendar.parser import Contentline
 from dateutil import tz
-from timetree_exporter.event import TimeTreeEvent, TimeTreeEventType
+from timetree_exporter.event import (
+    TimeTreeEvent,
+    TimeTreeEventType,
+    TimeTreeEventCategory,
+)
 from timetree_exporter.utils import convert_timestamp_to_datetime
 
 
+logger = logging.getLogger(__name__)
+
+
 class ICalEventFormatter:
     """
     Class for formatting TimeTree events into iCalendar format.
     """
 
     def __init__(self, time_tree_event: TimeTreeEvent):
         self.time_tree_event = time_tree_event
@@ -135,21 +143,49 @@
             contentline = Contentline(recurrence)
             name, parameters, value = contentline.parts()
             if name.lower() == "rrule":
                 event.add(name, vRecur.from_ical(value), parameters)
             elif name.lower() == "exdate" or name.lower() == "rdate":
                 event.add(name, vDDDLists.from_ical(value), parameters)
             else:
+                logger.error("Unknown recurrence type: %s", name)
                 raise ValueError(f"Unknown recurrence type: {name}")
 
     def to_ical(self) -> Event:
         """Return the iCal event."""
         if (
             self.time_tree_event.event_type == TimeTreeEventType.BIRTHDAY
         ):  # Skip if event is a birthday
+            logger.debug(
+                "Skipping birthday event\n \
+                    uid: %s \n \
+                    summary: '%s' \n \
+                    time: %s ~ %s \n \
+                    ",
+                self.uid,
+                self.summary,
+                self.dtstart.dt.strftime("%Y-%m-%d %H:%M:%S"),
+                self.dtend.dt.strftime("%Y-%m-%d %H:%M:%S"),
+            )
+
+            return None
+        if self.time_tree_event.category == TimeTreeEventCategory.MEMO:
+            # Skip if event is a memo
+            logger.debug(
+                "Skipping memo event\n \
+                    uid: %s \n \
+                    summary: '%s' \n \
+                    time: %s ~ %s \n \
+                    ",
+                self.uid,
+                self.summary,
+                self.dtstart.dt.strftime("%Y-%m-%d %H:%M:%S"),
+                self.dtend.dt.strftime("%Y-%m-%d %H:%M:%S"),
+            )
+
             return None
 
         event = Event()
 
         event.add("uid", self.uid)
         event.add("summary", self.summary)
         event.add("dtstamp", datetime.now(tz.tzutc()))
```

### Comparing `timetree-exporter-0.2.3/timetree_exporter/utils.py` & `timetree_exporter-0.3.0/timetree_exporter/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """Utility functions for Timetree Exporter"""
 
 import json
 import os
+import logging
 from datetime import datetime, timedelta
 from dateutil import tz
 
+logger = logging.getLogger(__name__)
+
 
 def get_events_from_file(file_path) -> list:
     """Fetch events from Timetree response file"""
     try:
         with open(file_path, "r", encoding="UTF-8") as response_file:
             response_data = json.load(response_file)
             return response_data["events"]
     except FileNotFoundError:
-        print(f"File not found: {file_path}")
+        logger.error("File not found: %s", file_path)
         return None
 
 
 def paths_to_filelist(paths: list) -> list:
     """Converts a list of paths to a list of files"""
     filenames = []
     for path in paths:
         if os.path.isdir(path):
             filenames += [os.path.join(path, file) for file in os.listdir(path)]
         elif os.path.isfile(path):
             filenames.append(path)
         else:
-            print(f"Invalid path: {path}")
+            logger.error("Invalid path: %s", path)
     return filenames
 
 
 def convert_timestamp_to_datetime(timestamp, tzinfo=tz.tzutc()):
     """
     Convert timestamp to datetime for both positive and negative timestamps on different platforms.
     """
```

### Comparing `timetree-exporter-0.2.3/timetree_exporter.egg-info/PKG-INFO` & `timetree_exporter-0.3.0/timetree_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
 Project-URL: Changelog, https://github.com/eoleedi/TimeTree-exporter/blob/main/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
@@ -72,15 +72,15 @@
 Currently, TimeTree data can only be downloaded manually through a web browser.
 
 # Roadmap of the properties mapping to iCal
 - [ ] **ID**
 - [ ] **Primary ID**
 - [ ] **Calendar ID**
 - [x] **UUID**
-- [ ] **Category**
+- [x] **Category**
 - [x] **Type**
 - [ ] **Author ID**
 - [ ] **Author Type**
 - [x] **Title**
 - [x] **All Day**
 - [x] **Start At**
 - [x] **Start Timezone**
```

### Comparing `timetree-exporter-0.2.3/timetree_exporter.egg-info/SOURCES.txt` & `timetree_exporter-0.3.0/timetree_exporter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 pyproject.toml
 requirements.txt
 .github/dependabot.yml
 .github/workflows/pylint.yml
 .github/workflows/python-publish.yml
 .github/workflows/release-please.yml
-.vscode/settings.json
 docs/assets/images/copy-response.png
 docs/assets/images/prepare-for-signin.png
 responses/README.md
 timetree_exporter/__init__.py
 timetree_exporter/__main__.py
 timetree_exporter/event.py
 timetree_exporter/formatter.py
```

