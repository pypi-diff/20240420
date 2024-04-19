# Comparing `tmp/KOFFI-0.1.1.tar.gz` & `tmp/koffi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KOFFI-0.1.1.tar", last modified: Tue Dec  6 21:35:30 2022, max compression
+gzip compressed data, was "koffi-0.1.2.tar", last modified: Fri Apr 19 23:10:02 2024, max compression
```

## Comparing `KOFFI-0.1.1.tar` & `koffi-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,58 @@
-drwxr-xr-x   0 maxwest    (501) staff       (20)        0 2022-12-06 21:35:30.860948 KOFFI-0.1.1/
--rw-r--r--   0 maxwest    (501) staff       (20)      131 2022-12-06 04:16:42.000000 KOFFI-0.1.1/.gitignore
--rw-r--r--   0 maxwest    (501) staff       (20)     1524 2022-12-06 04:16:42.000000 KOFFI-0.1.1/LICENSE
--rw-r--r--   0 maxwest    (501) staff       (20)      205 2022-12-06 21:35:30.860793 KOFFI-0.1.1/PKG-INFO
--rw-r--r--   0 maxwest    (501) staff       (20)     3793 2022-12-06 04:16:42.000000 KOFFI-0.1.1/README.md
--rw-r--r--   0 maxwest    (501) staff       (20)      566 2022-12-06 21:33:36.000000 KOFFI-0.1.1/pyproject.toml
--rw-r--r--   0 maxwest    (501) staff       (20)       38 2022-12-06 21:35:30.860985 KOFFI-0.1.1/setup.cfg
--rw-r--r--   0 maxwest    (501) staff       (20)       38 2022-12-06 04:16:42.000000 KOFFI-0.1.1/setup.py
-drwxr-xr-x   0 maxwest    (501) staff       (20)        0 2022-12-06 21:35:30.858209 KOFFI-0.1.1/src/
-drwxr-xr-x   0 maxwest    (501) staff       (20)        0 2022-12-06 21:35:30.859526 KOFFI-0.1.1/src/KOFFI.egg-info/
--rw-r--r--   0 maxwest    (501) staff       (20)      205 2022-12-06 21:35:30.000000 KOFFI-0.1.1/src/KOFFI.egg-info/PKG-INFO
--rw-r--r--   0 maxwest    (501) staff       (20)      488 2022-12-06 21:35:30.000000 KOFFI-0.1.1/src/KOFFI.egg-info/SOURCES.txt
--rw-r--r--   0 maxwest    (501) staff       (20)        1 2022-12-06 21:35:30.000000 KOFFI-0.1.1/src/KOFFI.egg-info/dependency_links.txt
--rw-r--r--   0 maxwest    (501) staff       (20)       29 2022-12-06 21:35:30.000000 KOFFI-0.1.1/src/KOFFI.egg-info/requires.txt
--rw-r--r--   0 maxwest    (501) staff       (20)       18 2022-12-06 21:35:30.000000 KOFFI-0.1.1/src/KOFFI.egg-info/top_level.txt
-drwxr-xr-x   0 maxwest    (501) staff       (20)        0 2022-12-06 21:35:30.859762 KOFFI-0.1.1/src/koffi/
--rw-r--r--   0 maxwest    (501) staff       (20)       21 2022-12-06 21:33:36.000000 KOFFI-0.1.1/src/koffi/__init__.py
--rw-r--r--   0 maxwest    (501) staff       (20)    11505 2022-12-06 21:33:36.000000 KOFFI-0.1.1/src/koffi/koffi.py
-drwxr-xr-x   0 maxwest    (501) staff       (20)        0 2022-12-06 21:35:30.860111 KOFFI-0.1.1/src/koffi_tools/
--rw-r--r--   0 maxwest    (501) staff       (20)       61 2022-12-06 21:33:36.000000 KOFFI-0.1.1/src/koffi_tools/__init__.py
--rw-r--r--   0 maxwest    (501) staff       (20)     8069 2022-12-06 21:33:36.000000 KOFFI-0.1.1/src/koffi_tools/image_metadata.py
--rw-r--r--   0 maxwest    (501) staff       (20)     1907 2022-12-06 21:33:36.000000 KOFFI-0.1.1/src/koffi_tools/potential_source.py
-drwxr-xr-x   0 maxwest    (501) staff       (20)        0 2022-12-06 21:35:30.860627 KOFFI-0.1.1/tests/
--rw-r--r--   0 maxwest    (501) staff       (20)        0 2022-12-06 04:16:42.000000 KOFFI-0.1.1/tests/__init__.py
--rw-r--r--   0 maxwest    (501) staff       (20)     1244 2022-12-06 04:16:42.000000 KOFFI-0.1.1/tests/koffi_test_helpers.py
--rw-r--r--   0 maxwest    (501) staff       (20)     5841 2022-12-06 04:16:42.000000 KOFFI-0.1.1/tests/test_image_metadata.py
--rw-r--r--   0 maxwest    (501) staff       (20)     8060 2022-12-06 04:16:42.000000 KOFFI-0.1.1/tests/test_koffi_search.py
--rw-r--r--   0 maxwest    (501) staff       (20)     2168 2022-12-06 04:16:42.000000 KOFFI-0.1.1/tests/test_potential_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.608631 koffi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 23:09:56.000000 koffi-0.1.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 23:09:56.000000 koffi-0.1.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-19 23:09:56.000000 koffi-0.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.600631 koffi-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.604631 koffi-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.604631 koffi-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 23:09:56.000000 koffi-0.1.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-19 23:09:56.000000 koffi-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-19 23:09:56.000000 koffi-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 23:09:56.000000 koffi-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-19 23:09:56.000000 koffi-0.1.2/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-19 23:09:56.000000 koffi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-19 23:10:02.608631 koffi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-19 23:09:56.000000 koffi-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.604631 koffi-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-19 23:09:56.000000 koffi-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-19 23:09:56.000000 koffi-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-19 23:09:56.000000 koffi-0.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.604631 koffi-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 23:09:56.000000 koffi-0.1.2/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 23:09:56.000000 koffi-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-19 23:09:56.000000 koffi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:10:02.608631 koffi-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 23:09:56.000000 koffi-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.600631 koffi-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.604631 koffi-0.1.2/src/koffi/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 23:09:56.000000 koffi-0.1.2/src/koffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 23:10:02.000000 koffi-0.1.2/src/koffi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-19 23:09:56.000000 koffi-0.1.2/src/koffi/koffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 23:09:56.000000 koffi-0.1.2/src/koffi/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.608631 koffi-0.1.2/src/koffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-19 23:10:02.000000 koffi-0.1.2/src/koffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-19 23:10:02.000000 koffi-0.1.2/src/koffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:10:02.000000 koffi-0.1.2/src/koffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 23:10:02.000000 koffi-0.1.2/src/koffi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 23:10:02.000000 koffi-0.1.2/src/koffi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.604631 koffi-0.1.2/src/koffi_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 23:09:56.000000 koffi-0.1.2/src/koffi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-19 23:09:56.000000 koffi-0.1.2/src/koffi_tools/image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-19 23:09:56.000000 koffi-0.1.2/src/koffi_tools/potential_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.608631 koffi-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:09:56.000000 koffi-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:10:02.608631 koffi-0.1.2/tests/koffi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:09:56.000000 koffi-0.1.2/tests/koffi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 23:09:56.000000 koffi-0.1.2/tests/koffi_test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-19 23:09:56.000000 koffi-0.1.2/tests/test_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-19 23:09:56.000000 koffi-0.1.2/tests/test_koffi_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-19 23:09:56.000000 koffi-0.1.2/tests/test_potential_source.py
```

### Comparing `KOFFI-0.1.1/LICENSE` & `koffi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `KOFFI-0.1.1/src/koffi/koffi.py` & `koffi-0.1.2/src/koffi/koffi.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     base_url = "https://ssd-api.jpl.nasa.gov/sb_ident.api?sb-kind=a&mag-required=true&req-elem=false"
 
     # Format the time query and MPC string.
     t_str = "obs-time=%f" % image.get_epoch().jd
 
     # Create a string of data for the observatory.
     if image.obs_code:
-        obs_str = "mpc-code=%s" % self.obs_code
+        obs_str = "mpc-code=%s" % image.obs_code
     else:
         obs_str = "lat=%f&lon=%f&alt=%f" % (image.obs_lat, image.obs_long, image.obs_alt)
 
     # Format the RA query including half width.
     if image.center.ra.degree < 0:
         image.center.ra.degree += 360.0
     ra_hms_L = Angle(image.center.ra - image.ra_radius()).hms
@@ -185,15 +185,15 @@
     dec_dms_L = Angle(image.center.dec - image.dec_radius()).dms
     if dec_dms_L[0] >= 0:
         dec_str = "fov-dec-lim=%02i-%02i-%05.2f" % (dec_dms_L[0], dec_dms_L[1], dec_dms_L[2])
     else:
         dec_str = "fov-dec-lim=M%02i-%02i-%05.2f" % (-dec_dms_L[0], -dec_dms_L[1], -dec_dms_L[2])
     dec_dms_H = Angle(image.center.dec + image.dec_radius()).dms
     if dec_dms_H[0] >= 0:
-        dec_str = "%s,02i-%02i-%05.2f" % (dec_str, dec_dms_H[0], dec_dms_H[1], dec_dms_H[2])
+        dec_str = "%s,%02i-%02i-%05.2f" % (dec_str, dec_dms_H[0], dec_dms_H[1], dec_dms_H[2])
     else:
         dec_str = "%s,M%02i-%02i-%05.2f" % (dec_str, -dec_dms_H[0], -dec_dms_H[1], -dec_dms_H[2])
 
     # Only do the second (more accurate) pass.
     pass_str = "two-pass=true&suppress-first-pass=true"
 
     # Complete the full query.
@@ -219,14 +219,17 @@
 
     objects = []
 
     with libreq.urlopen(query_string) as url:
         feed = url.read().decode("utf-8")
         results = json.loads(feed)
 
+        if "warning" in results.keys() and results["warning"] == "no matching records":
+            return []
+
         num_results = results["n_second_pass"]
         for item in results["data_second_pass"]:
             name = item[0]
             ra_str = item[1]
             dec_str = item[2].replace("'", " ").replace('"', "")
             sc = SkyCoord(ra_str, dec_str, unit=(u.hourangle, u.deg))
             objects.append([name, sc])
```

### Comparing `KOFFI-0.1.1/src/koffi_tools/image_metadata.py` & `koffi-0.1.2/src/koffi_tools/image_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from astropy.io import fits
-from astropy.time import Time
+from astropy.time import Time, TimeDelta
 from astropy.wcs import WCS
+from astroquery.mpc import MPC
 
 
 class ImageMetadata:
     def __init__(self, file=None, mjd_key="MJD_OBS", mjd_val=None):
         """
         Arguments:
             file : a string containing a file path for a .fits file.
@@ -53,35 +54,41 @@
             # get the time and set the epoch
             if mjd_val is not None:
                 self.set_epoch(Time(mjd_val, format="mjd"))
             else:
                 # Patch for DECam data
                 if "DATE-AVG" in hdu_list[0].header:
                     self.set_epoch(Time(hdu_list[0].header["DATE-AVG"], format="isot"))
+                elif "DATE-OBS" in hdu_list[0].header and "EXPTIME" in hdu_list[0].header:
+                    self.set_epoch(
+                        Time(hdu_list[0].header["DATE-OBS"], format="isot")
+                        + TimeDelta(hdu_list[0].header["EXPTIME"], format="sec") / 2
+                    )
                 elif self.get_header_element(mjd_key) is not None:
                     self.set_epoch(Time(self.get_header_element(mjd_key), format="mjd"))
 
             # Extract information about the location of the observatory.
             # Since this doesn't seem to be standardized, we try some
             # documented versions.
             observat = self.get_header_element("OBSERVAT")
+            observatories = MPC.get_observatory_codes()  # get list of MPC-defined observatory codes
             obs_lat = self.get_header_element("OBS-LAT")
-            lat_obs = self.get_header_element("LAT_OBS")
-            if observat is not None:
+            lat_obs = self.get_header_element("LAT-OBS")
+            if observat is not None and observat in observatories["Code"]:
                 self.obs_code = observat
                 self.obs_loc_set = True
             elif obs_lat is not None:
                 self.obs_lat = float(obs_lat)
                 self.obs_long = float(self.get_header_element("OBS-LONG"))
                 self.obs_alt = float(self.get_header_element("OBS-ELEV"))
                 self.obs_loc_set = True
             elif lat_obs is not None:
                 self.obs_lat = float(lat_obs)
-                self.obs_long = float(self.get_header_element("LONG_OBS"))
-                self.obs_alt = float(self.get_header_element("ALT_OBS"))
+                self.obs_long = float(self.get_header_element("LONG-OBS"))
+                self.obs_alt = float(self.get_header_element("ALT-OBS"))
                 self.obs_loc_set = True
             else:
                 self.obs_loc_set = False
 
             # Compute the center of the image in sky coordinates.
             self.center = self.wcs.pixel_to_world(self.width / 2, self.height / 2)
```

### Comparing `KOFFI-0.1.1/src/koffi_tools/potential_source.py` & `koffi-0.1.2/src/koffi_tools/potential_source.py`

 * *Files identical despite different names*

### Comparing `KOFFI-0.1.1/tests/koffi_test_helpers.py` & `koffi-0.1.2/tests/koffi_test_helpers.py`

 * *Files identical despite different names*

### Comparing `KOFFI-0.1.1/tests/test_image_metadata.py` & `koffi-0.1.2/tests/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `KOFFI-0.1.1/tests/test_koffi_search.py` & `koffi-0.1.2/tests/test_koffi_search.py`

 * *Files identical despite different names*

### Comparing `KOFFI-0.1.1/tests/test_potential_source.py` & `koffi-0.1.2/tests/test_potential_source.py`

 * *Files identical despite different names*

