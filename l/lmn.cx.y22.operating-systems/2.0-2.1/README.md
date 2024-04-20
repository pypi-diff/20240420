# Comparing `tmp/lmn_cx_y22_operating_systems-2.0.tar.gz` & `tmp/lmn_cx_y22_operating_systems-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmn_cx_y22_operating_systems-2.0.tar", last modified: Fri Apr 19 01:10:02 2024, max compression
+gzip compressed data, was "lmn_cx_y22_operating_systems-2.1.tar", last modified: Sat Apr 20 19:09:25 2024, max compression
```

## Comparing `lmn_cx_y22_operating_systems-2.0.tar` & `lmn_cx_y22_operating_systems-2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.678043 lmn_cx_y22_operating_systems-2.0/
--rw-rw-rw-   0        0        0     3383 2024-04-17 15:36:16.000000 lmn_cx_y22_operating_systems-2.0/.gitignore
--rw-rw-rw-   0        0        0      761 2024-04-17 23:30:48.000000 lmn_cx_y22_operating_systems-2.0/COPYING
--rw-rw-rw-   0        0        0      681 2024-04-17 23:51:44.000000 lmn_cx_y22_operating_systems-2.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.649825 lmn_cx_y22_operating_systems-2.0/LICENSES/
--rw-rw-rw-   0        0        0      656 2024-04-17 23:47:39.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/0BSD.txt
--rw-rw-rw-   0        0        0    11558 2024-04-17 14:21:46.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0        0        0     7169 2024-04-17 15:09:19.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0        0        0     1099 2024-04-17 20:35:00.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/MIT.txt
--rw-rw-rw-   0        0        0     1045 2024-04-19 01:10:02.674028 lmn_cx_y22_operating_systems-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      123 2024-04-17 15:35:59.000000 lmn_cx_y22_operating_systems-2.0/README.md
--rw-rw-rw-   0        0        0     1397 2024-04-17 23:39:05.000000 lmn_cx_y22_operating_systems-2.0/REUSE
--rw-rw-rw-   0        0        0     1771 2024-04-17 23:44:16.000000 lmn_cx_y22_operating_systems-2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 01:10:02.678043 lmn_cx_y22_operating_systems-2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.545975 lmn_cx_y22_operating_systems-2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.545975 lmn_cx_y22_operating_systems-2.0/src/lmn/
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.545975 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.550404 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.672017 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/operating_systems/
--rw-rw-rw-   0        0        0      313 2024-04-18 00:33:46.000000 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/operating_systems/__init__.py
--rw-rw-rw-   0        0        0     2907 2024-04-19 01:08:37.000000 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/operating_systems/_operating_systems.py
-drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.674028 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/
--rw-rw-rw-   0        0        0     1045 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.254099 lmn_cx_y22_operating_systems-2.1/
+-rw-rw-rw-   0        0        0     3383 2024-04-17 15:36:16.000000 lmn_cx_y22_operating_systems-2.1/.gitignore
+-rw-rw-rw-   0        0        0     1754 2024-04-20 18:00:48.000000 lmn_cx_y22_operating_systems-2.1/COPYING
+-rw-rw-rw-   0        0        0      681 2024-04-20 17:26:29.000000 lmn_cx_y22_operating_systems-2.1/LICENSE-0BSD
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.213978 lmn_cx_y22_operating_systems-2.1/LICENSES/
+-rw-rw-rw-   0        0        0      656 2024-04-17 23:47:39.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/0BSD.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-17 14:21:46.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0        0        0     7169 2024-04-17 15:09:19.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0        0        0     1099 2024-04-17 20:35:00.000000 lmn_cx_y22_operating_systems-2.1/LICENSES/MIT.txt
+-rw-rw-rw-   0        0        0     1162 2024-04-20 19:09:25.250826 lmn_cx_y22_operating_systems-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2024-04-17 15:35:59.000000 lmn_cx_y22_operating_systems-2.1/README.md
+-rw-rw-rw-   0        0        0     1504 2024-04-20 18:03:19.000000 lmn_cx_y22_operating_systems-2.1/REUSE
+-rw-rw-rw-   0        0        0     1973 2024-04-20 18:44:09.000000 lmn_cx_y22_operating_systems-2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 19:09:25.254099 lmn_cx_y22_operating_systems-2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/lmn/
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.198555 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.247809 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/operating_systems/
+-rw-rw-rw-   0        0        0      313 2024-04-20 17:19:34.000000 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/operating_systems/__init__.py
+-rw-rw-rw-   0        0        0     3493 2024-04-20 19:09:04.000000 lmn_cx_y22_operating_systems-2.1/src/lmn/cx/y22/operating_systems/_operating_systems.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:09:25.250826 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/
+-rw-rw-rw-   0        0        0     1162 2024-04-20 19:09:24.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-20 19:09:25.000000 lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
```

### Comparing `lmn_cx_y22_operating_systems-2.0/.gitignore` & `lmn_cx_y22_operating_systems-2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.0/LICENSE` & `lmn_cx_y22_operating_systems-2.1/LICENSE-0BSD`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.0/LICENSES/0BSD.txt` & `lmn_cx_y22_operating_systems-2.1/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.0/LICENSES/Apache-2.0.txt` & `lmn_cx_y22_operating_systems-2.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.0/LICENSES/CC0-1.0.txt` & `lmn_cx_y22_operating_systems-2.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.0/LICENSES/MIT.txt` & `lmn_cx_y22_operating_systems-2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-2.0/PKG-INFO` & `lmn_cx_y22_operating_systems-2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: lmn.cx.y22.operating_systems
-Version: 2.0
+Version: 2.1
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.11
-License-File: LICENSE
+License-File: LICENSES\0BSD.txt
+License-File: LICENSES\Apache-2.0.txt
+License-File: LICENSES\CC0-1.0.txt
+License-File: LICENSES\MIT.txt
 License-File: COPYING
 Provides-Extra: dev
 Requires-Dist: pip; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: reuse; extra == "dev"
```

### Comparing `lmn_cx_y22_operating_systems-2.0/REUSE` & `lmn_cx_y22_operating_systems-2.1/REUSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 The copyright and licensing for the contents of this project are
 tracked using the REUSE Specification. For more information on this
 standard, see <https://reuse.software/spec/>.
 
 For most files, this means we keep track of copyright and licensing
-using SPDX headers. For example, the SPDX headers for this COPYING
+using SPDX headers. For example, the SPDX headers for this REUSE
 file are:
 
     SPDX-FileCopyrightText: 2024 Alex Lemna
     SPDX-License-Identifier: CC0-1.0
 
-For all other files in this project, the SPDX headers will generally
+For all other significant files in this project, the SPDX headers will
 be in the first lines of the file. Any exceptions to this rule will
 have their copyright and licensing information stored in one of the
 alternate methods discussed at <https://reuse.software/spec/>, i.e.,
 
   - comment headers in an adjacent file of the same name plus the 
     `.license` extension (e.g., `dog.png` and `dog.png.license`), 
     or
@@ -26,7 +26,10 @@
 instance, if I have directly copied code from other open source 
 projects or from blogs, StackOverflow posts, et cetera. In these
 cases, the section will be clearly associated with additional SPDX
 tags to indicate that section's copyrights and licensing.
 
 You can review the full text of any license relevant to any of the
 contents of this project in the LICENSES directory.
+
+You can also review an informal explanation of this software's 
+licensing options in the COPYING file.
```

### Comparing `lmn_cx_y22_operating_systems-2.0/pyproject.toml` & `lmn_cx_y22_operating_systems-2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -68,8 +68,13 @@
 ]
 
 [tool.pip-tools]
 allow-unsafe = true
 generate-hashes = true
 resolver = "backtracking"
 
+[tool.setuptools]
+# For more on including license files with package distributions,
+#   see: https://stackoverflow.com/q/75634466
+license-files = ["LICENSES/*", "COPYING*", "NOTICE*", "AUTHORS*"]
+
 [tool.setuptools_scm]
```

### Comparing `lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO` & `lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: lmn.cx.y22.operating_systems
-Version: 2.0
+Version: 2.1
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.11
-License-File: LICENSE
+License-File: LICENSES\0BSD.txt
+License-File: LICENSES\Apache-2.0.txt
+License-File: LICENSES\CC0-1.0.txt
+License-File: LICENSES\MIT.txt
 License-File: COPYING
 Provides-Extra: dev
 Requires-Dist: pip; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: reuse; extra == "dev"
```

### Comparing `lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt` & `lmn_cx_y22_operating_systems-2.1/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .gitignore
 COPYING
-LICENSE
+LICENSE-0BSD
 README.md
 REUSE
 pyproject.toml
 LICENSES/0BSD.txt
 LICENSES/Apache-2.0.txt
 LICENSES/CC0-1.0.txt
 LICENSES/MIT.txt
```

