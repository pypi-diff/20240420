# Comparing `tmp/flet_easy-0.2.0.dev14.tar.gz` & `tmp/flet_easy-0.2.0.dev15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy-0.2.0.dev14.tar", last modified: Fri Apr 19 00:15:36 2024, max compression
+gzip compressed data, was "flet_easy-0.2.0.dev15.tar", last modified: Fri Apr 19 17:22:55 2024, max compression
```

## Comparing `flet_easy-0.2.0.dev14.tar` & `flet_easy-0.2.0.dev15.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0.dev14/LICENSE
--rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0.dev14/LICENSE
--rw-r--r--   0        0        0     4215 2024-04-12 03:06:37.460321 flet_easy-0.2.0.dev14/README.md
--rw-r--r--   0        0        0     4215 2024-04-12 03:06:37.460321 flet_easy-0.2.0.dev14/README.md
--rw-r--r--   0        0        0     1733 2024-04-19 00:15:36.543040 flet_easy-0.2.0.dev14/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-12 03:14:22.077045 flet_easy-0.2.0.dev14/src/flet_easy/__init__.py
--rw-r--r--   0        0        0     1282 2024-04-19 00:12:26.486653 flet_easy-0.2.0.dev14/src/flet_easy/auto_route.py
--rw-r--r--   0        0        0     2356 2024-04-12 03:14:22.079042 flet_easy-0.2.0.dev14/src/flet_easy/cli/copy.py
--rw-r--r--   0        0        0     2099 2024-04-18 16:58:31.614890 flet_easy-0.2.0.dev14/src/flet_easy/cli/main.py
--rw-r--r--   0        0        0     3266 2024-04-12 03:14:22.080559 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/.gitignore
--rw-r--r--   0        0        0      213 2024-04-12 03:14:22.081589 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/README.md
--rw-r--r--   0        0        0     1020 2024-04-12 03:14:22.081589 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/favicon.png
--rw-r--r--   0        0        0    30189 2024-04-12 03:14:22.082609 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icon.png
--rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.083607 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-192.png
--rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.084612 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-512.png
--rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.085610 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.086618 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    56474 2024-04-12 03:14:22.087607 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/loading-animation.png
--rw-r--r--   0        0        0     3626 2024-04-12 03:14:22.088615 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/index.html
--rw-r--r--   0        0        0      932 2024-04-12 03:14:22.088615 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/manifest.json
--rw-r--r--   0        0        0       84 2024-04-12 03:14:22.090138 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/components/__init__.py
--rw-r--r--   0        0        0     2422 2024-04-12 03:14:22.090138 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/components/counter.py
--rw-r--r--   0        0        0      543 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/components/swoDrawer.py
--rw-r--r--   0        0        0       45 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/controllers/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/controllers/counter.py
--rw-r--r--   0        0        0        0 2024-04-12 03:14:22.092763 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/core/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-12 03:14:22.093720 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/core/config.py
--rw-r--r--   0        0        0      229 2024-04-18 23:23:02.832176 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/main.py
--rw-r--r--   0        0        0        0 2024-04-12 03:14:22.094724 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-12 03:14:22.096720 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/views/counter.py
--rw-r--r--   0        0        0      615 2024-04-16 23:25:58.330304 flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/views/index.py
--rw-r--r--   0        0        0    12208 2024-04-16 21:36:20.961519 flet_easy-0.2.0.dev14/src/flet_easy/datasy.py
--rw-r--r--   0        0        0      187 2024-04-12 03:14:22.098727 flet_easy-0.2.0.dev14/src/flet_easy/extra.py
--rw-r--r--   0        0        0     2483 2024-04-12 03:14:22.098727 flet_easy-0.2.0.dev14/src/flet_easy/extrasJwt.py
--rw-r--r--   0        0        0    18351 2024-04-18 15:59:12.014794 flet_easy-0.2.0.dev14/src/flet_easy/fletEasy.py
--rw-r--r--   0        0        0     9856 2024-04-16 17:27:34.348744 flet_easy-0.2.0.dev14/src/flet_easy/inheritance.py
--rw-r--r--   0        0        0     1191 2024-04-16 21:14:26.280232 flet_easy-0.2.0.dev14/src/flet_easy/job.py
--rw-r--r--   0        0        0     4024 2024-04-16 21:27:52.940346 flet_easy-0.2.0.dev14/src/flet_easy/jwt.py
--rw-r--r--   0        0        0     7512 2024-04-16 17:27:54.461988 flet_easy-0.2.0.dev14/src/flet_easy/pagesy.py
--rw-r--r--   0        0        0    11272 2024-04-19 00:10:05.143031 flet_easy-0.2.0.dev14/src/flet_easy/route.py
--rw-r--r--   0        0        0     1540 2024-04-12 03:14:22.105829 flet_easy-0.2.0.dev14/src/flet_easy/view_404.py
--rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 flet_easy-0.2.0.dev14/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0.dev15/LICENSE
+-rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0.dev15/LICENSE
+-rw-r--r--   0        0        0     4215 2024-04-12 03:06:37.460321 flet_easy-0.2.0.dev15/README.md
+-rw-r--r--   0        0        0     4215 2024-04-12 03:06:37.460321 flet_easy-0.2.0.dev15/README.md
+-rw-r--r--   0        0        0     1733 2024-04-19 17:22:55.080519 flet_easy-0.2.0.dev15/pyproject.toml
+-rw-r--r--   0        0        0      432 2024-04-12 03:14:22.077045 flet_easy-0.2.0.dev15/src/flet_easy/__init__.py
+-rw-r--r--   0        0        0     1282 2024-04-19 00:12:26.486653 flet_easy-0.2.0.dev15/src/flet_easy/auto_route.py
+-rw-r--r--   0        0        0     2356 2024-04-12 03:14:22.079042 flet_easy-0.2.0.dev15/src/flet_easy/cli/copy.py
+-rw-r--r--   0        0        0     2099 2024-04-18 16:58:31.614890 flet_easy-0.2.0.dev15/src/flet_easy/cli/main.py
+-rw-r--r--   0        0        0     3266 2024-04-12 03:14:22.080559 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/.gitignore
+-rw-r--r--   0        0        0      213 2024-04-12 03:14:22.081589 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/README.md
+-rw-r--r--   0        0        0     1020 2024-04-12 03:14:22.081589 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/favicon.png
+-rw-r--r--   0        0        0    30189 2024-04-12 03:14:22.082609 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icon.png
+-rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.083607 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-192.png
+-rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.084612 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-512.png
+-rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.085610 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.086618 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    56474 2024-04-12 03:14:22.087607 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/loading-animation.png
+-rw-r--r--   0        0        0     3626 2024-04-12 03:14:22.088615 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/index.html
+-rw-r--r--   0        0        0      932 2024-04-12 03:14:22.088615 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/manifest.json
+-rw-r--r--   0        0        0       84 2024-04-12 03:14:22.090138 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/components/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-12 03:14:22.090138 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/components/counter.py
+-rw-r--r--   0        0        0      543 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/components/swoDrawer.py
+-rw-r--r--   0        0        0       45 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/controllers/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-12 03:14:22.091176 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/controllers/counter.py
+-rw-r--r--   0        0        0        0 2024-04-12 03:14:22.092763 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/core/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-12 03:14:22.093720 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/core/config.py
+-rw-r--r--   0        0        0      246 2024-04-19 16:50:45.518416 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/main.py
+-rw-r--r--   0        0        0        0 2024-04-12 03:14:22.094724 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-12 03:14:22.096720 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/views/counter.py
+-rw-r--r--   0        0        0      615 2024-04-16 23:25:58.330304 flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/views/index.py
+-rw-r--r--   0        0        0    12208 2024-04-16 21:36:20.961519 flet_easy-0.2.0.dev15/src/flet_easy/datasy.py
+-rw-r--r--   0        0        0      187 2024-04-12 03:14:22.098727 flet_easy-0.2.0.dev15/src/flet_easy/extra.py
+-rw-r--r--   0        0        0     2483 2024-04-12 03:14:22.098727 flet_easy-0.2.0.dev15/src/flet_easy/extrasJwt.py
+-rw-r--r--   0        0        0    18351 2024-04-18 15:59:12.014794 flet_easy-0.2.0.dev15/src/flet_easy/fletEasy.py
+-rw-r--r--   0        0        0     9856 2024-04-16 17:27:34.348744 flet_easy-0.2.0.dev15/src/flet_easy/inheritance.py
+-rw-r--r--   0        0        0     1191 2024-04-16 21:14:26.280232 flet_easy-0.2.0.dev15/src/flet_easy/job.py
+-rw-r--r--   0        0        0     4024 2024-04-16 21:27:52.940346 flet_easy-0.2.0.dev15/src/flet_easy/jwt.py
+-rw-r--r--   0        0        0     7512 2024-04-16 17:27:54.461988 flet_easy-0.2.0.dev15/src/flet_easy/pagesy.py
+-rw-r--r--   0        0        0    11272 2024-04-19 16:32:26.352407 flet_easy-0.2.0.dev15/src/flet_easy/route.py
+-rw-r--r--   0        0        0     1540 2024-04-12 03:14:22.105829 flet_easy-0.2.0.dev15/src/flet_easy/view_404.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 flet_easy-0.2.0.dev15/PKG-INFO
```

### Comparing `flet_easy-0.2.0.dev14/LICENSE` & `flet_easy-0.2.0.dev15/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/README.md` & `flet_easy-0.2.0.dev15/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/pyproject.toml` & `flet_easy-0.2.0.dev15/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flet-easy"
-version = "0.2.0.dev14"
+version = "0.2.0.dev15"
 description = "Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features."
 authors = [
     { name = "Daxexs", email = "Daxexsdev@gmail.com" },
 ]
 dependencies = [
     "parse>=1.20.1",
     "pyJWT>=2.8.0",
```

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/auto_route.py` & `flet_easy-0.2.0.dev15/src/flet_easy/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/copy.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/copy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/main.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/main.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/.gitignore` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/favicon.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icon.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-192.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-512.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/icons/loading-animation.png` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/index.html` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/index.html`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/assets/manifest.json` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/components/counter.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/components/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/components/swoDrawer.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/components/swoDrawer.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/controllers/counter.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/controllers/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/core/config.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/core/config.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/views/counter.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/views/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/cli/templates/views/index.py` & `flet_easy-0.2.0.dev15/src/flet_easy/cli/templates/views/index.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/datasy.py` & `flet_easy-0.2.0.dev15/src/flet_easy/datasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/extrasJwt.py` & `flet_easy-0.2.0.dev15/src/flet_easy/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/fletEasy.py` & `flet_easy-0.2.0.dev15/src/flet_easy/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/inheritance.py` & `flet_easy-0.2.0.dev15/src/flet_easy/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/job.py` & `flet_easy-0.2.0.dev15/src/flet_easy/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/jwt.py` & `flet_easy-0.2.0.dev15/src/flet_easy/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/pagesy.py` & `flet_easy-0.2.0.dev15/src/flet_easy/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/route.py` & `flet_easy-0.2.0.dev15/src/flet_easy/route.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/src/flet_easy/view_404.py` & `flet_easy-0.2.0.dev15/src/flet_easy/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev14/PKG-INFO` & `flet_easy-0.2.0.dev15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-easy
-Version: 0.2.0.dev14
+Version: 0.2.0.dev15
 Summary: Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
 Keywords: flet easy,flet,python,flet router
 Author-Email: Daxexs <Daxexsdev@gmail.com>
 License: apache-2.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

