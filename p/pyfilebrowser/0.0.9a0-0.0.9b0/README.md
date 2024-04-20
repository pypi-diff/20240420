# Comparing `tmp/pyfilebrowser-0.0.9a0-py3-none-any.whl.zip` & `tmp/pyfilebrowser-0.0.9b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18123 bytes, number of entries: 14
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-08 17:44 pyfilebrowser/__init__.py
--rw-r--r--  2.0 unx     8709 b- defN 24-Apr-08 02:42 pyfilebrowser/main.py
--rw-r--r--  2.0 unx      133 b- defN 24-Apr-08 05:24 pyfilebrowser/requirements.txt
--rw-r--r--  2.0 unx     5452 b- defN 24-Mar-30 22:39 pyfilebrowser/modals/config.py
--rw-r--r--  2.0 unx     1765 b- defN 24-Mar-24 04:18 pyfilebrowser/modals/models.py
--rw-r--r--  2.0 unx     1603 b- defN 24-Mar-24 04:18 pyfilebrowser/modals/users.py
--rw-r--r--  2.0 unx    10178 b- defN 24-Mar-29 23:16 pyfilebrowser/squire/download.py
--rw-r--r--  2.0 unx     4525 b- defN 24-Apr-01 03:38 pyfilebrowser/squire/steward.py
--rw-r--r--  2.0 unx     3056 b- defN 24-Mar-30 14:30 pyfilebrowser/squire/struct.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-08 17:45 pyfilebrowser-0.0.9a0.dist-info/LICENSE
--rw-r--r--  2.0 unx    11035 b- defN 24-Apr-08 17:45 pyfilebrowser-0.0.9a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 17:45 pyfilebrowser-0.0.9a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-08 17:45 pyfilebrowser-0.0.9a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1197 b- defN 24-Apr-08 17:45 pyfilebrowser-0.0.9a0.dist-info/RECORD
-14 files, 48934 bytes uncompressed, 16123 bytes compressed:  67.1%
+Zip file size: 17167 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-06 16:56 pyfilebrowser/__init__.py
+-rw-r--r--  2.0 unx     8656 b- defN 24-Apr-05 10:33 pyfilebrowser/main.py
+-rw-r--r--  2.0 unx       89 b- defN 24-Mar-31 04:11 pyfilebrowser/requirements.txt
+-rw-r--r--  2.0 unx     5452 b- defN 24-Mar-31 04:11 pyfilebrowser/modals/config.py
+-rw-r--r--  2.0 unx     1765 b- defN 24-Mar-27 22:22 pyfilebrowser/modals/models.py
+-rw-r--r--  2.0 unx     1603 b- defN 24-Mar-27 22:22 pyfilebrowser/modals/users.py
+-rw-r--r--  2.0 unx    10178 b- defN 24-Apr-05 10:58 pyfilebrowser/squire/download.py
+-rw-r--r--  2.0 unx     4525 b- defN 24-Apr-03 01:54 pyfilebrowser/squire/steward.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-Mar-31 04:11 pyfilebrowser/squire/struct.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8493 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1195 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/RECORD
+14 files, 46296 bytes uncompressed, 15167 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pyfilebrowser/squire/steward.py
 Comment: 
 
 Filename: pyfilebrowser/squire/struct.py
 Comment: 
 
-Filename: pyfilebrowser-0.0.9a0.dist-info/LICENSE
+Filename: pyfilebrowser-0.0.9b0.dist-info/LICENSE
 Comment: 
 
-Filename: pyfilebrowser-0.0.9a0.dist-info/METADATA
+Filename: pyfilebrowser-0.0.9b0.dist-info/METADATA
 Comment: 
 
-Filename: pyfilebrowser-0.0.9a0.dist-info/WHEEL
+Filename: pyfilebrowser-0.0.9b0.dist-info/WHEEL
 Comment: 
 
-Filename: pyfilebrowser-0.0.9a0.dist-info/top_level.txt
+Filename: pyfilebrowser-0.0.9b0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfilebrowser-0.0.9a0.dist-info/RECORD
+Filename: pyfilebrowser-0.0.9b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyfilebrowser/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Module for packaging."""
 
 from pyfilebrowser.main import FileBrowser  # noqa: F401
 
-version = "0.0.9-a"
+version = "0.0.9-beta"
```

## pyfilebrowser/main.py

```diff
@@ -42,18 +42,18 @@
     def exit_process(self) -> None:
         """Deletes the database file, and all the subtitles that were created by this application."""
         if os.path.isfile(download.executable.filebrowser_db):
             self.logger.info("Removing database %s", download.executable.filebrowser_db)
             os.remove(download.executable.filebrowser_db)
         if self.proxy_engine:
             self.logger.info("Stopping proxy service")
-            self.proxy_engine.join(timeout=3)  # Gracefully terminate the proxy server
-            for i in range(1, 6):
+            self.proxy_engine.terminate()
+            for i in range(5):
                 if self.proxy_engine.is_alive():
-                    self.proxy_engine.terminate()
+                    self.proxy_engine.kill()
                 else:
                     self.logger.info("Daemon process terminated in %s attempt", steward.ordinal(i))
                     self.proxy_engine.close()
                     break
                 time.sleep(1e-1)  # 0.1s
             else:
                 warnings.warn(
```

## pyfilebrowser/requirements.txt

```diff
@@ -1,8 +1,5 @@
 bcrypt==4.1.*
 fastapi==0.110.*
-httpx==0.27.*
-Jinja2==3.1.*
 pydantic==2.6.*
 pydantic-settings==2.2.*
 requests==2.31.*
-uvicorn==0.29.*
```

## Comparing `pyfilebrowser-0.0.9a0.dist-info/LICENSE` & `pyfilebrowser-0.0.9b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfilebrowser-0.0.9a0.dist-info/RECORD` & `pyfilebrowser-0.0.9b0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pyfilebrowser/__init__.py,sha256=6HyodL7CP1y4j0hCQ1hY5gv89kZZvhRi6BduuueVPbg,107
-pyfilebrowser/main.py,sha256=CvfHf9xs7f-8ESdEGfu6UsNAbuMTgwvYRn2eWG6L3qY,8709
-pyfilebrowser/requirements.txt,sha256=oY1UJoRWkFWO7JlQ4asLAcOiHlBsZX8LLAie9EpqLzc,133
+pyfilebrowser/__init__.py,sha256=Uu3IuPmX3NJtM2scQAqxqousy7cbzW1Q71vtLgsg044,110
+pyfilebrowser/main.py,sha256=QDkl11k7BY__8DAf8jjlIqkfzBC3fTWByrV1E_6P2gU,8656
+pyfilebrowser/requirements.txt,sha256=iqRgXyC9MTSdgB8LD5yJDMfc7c5Zmuf82M2AqTakh1w,89
 pyfilebrowser/modals/config.py,sha256=nMRWu1esluHosN3wUw3w5EooubJuBTzpxIoHWcDZB6M,5452
 pyfilebrowser/modals/models.py,sha256=1RVSZaNgWChLv8c0-zMXgSpLDonitMgrc9fYvlzEs3U,1765
 pyfilebrowser/modals/users.py,sha256=xKdpMrcbWTza2llFTRPkKJG3ySEVlvC03rSMA4KgK5s,1603
 pyfilebrowser/squire/download.py,sha256=FI_1GZrjcTtYBE3bXOSa4f-FSgjU9ejANW-NdEZq2KQ,10178
 pyfilebrowser/squire/steward.py,sha256=hVoWBrJWa2HSvR56JKnk_vXh0Qm0jPbEGwQ4dWtpXM8,4525
 pyfilebrowser/squire/struct.py,sha256=rg19tpW1iX17792uFWLQAhVZ2PLiHYETYc21GFulldE,3056
-pyfilebrowser-0.0.9a0.dist-info/LICENSE,sha256=xnHdLNCLt4RW3vtnE_TfN_cjViUHyIv0m8024fS4bws,1068
-pyfilebrowser-0.0.9a0.dist-info/METADATA,sha256=LawmeCln73Q7xUcgKHcZBz4_956mY_j_U4h61dcfK6o,11035
-pyfilebrowser-0.0.9a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyfilebrowser-0.0.9a0.dist-info/top_level.txt,sha256=RrwbvxqHTriDpUwaZC3F5o53eZtUKODCQQ0iRryM_Zo,14
-pyfilebrowser-0.0.9a0.dist-info/RECORD,,
+pyfilebrowser-0.0.9b0.dist-info/LICENSE,sha256=xnHdLNCLt4RW3vtnE_TfN_cjViUHyIv0m8024fS4bws,1068
+pyfilebrowser-0.0.9b0.dist-info/METADATA,sha256=hJ1d5qbuSczYUCkgFbOPKJ1gkTyZZYQXaNkaWOmvcCM,8493
+pyfilebrowser-0.0.9b0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyfilebrowser-0.0.9b0.dist-info/top_level.txt,sha256=RrwbvxqHTriDpUwaZC3F5o53eZtUKODCQQ0iRryM_Zo,14
+pyfilebrowser-0.0.9b0.dist-info/RECORD,,
```

