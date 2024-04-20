# Comparing `tmp/monisha-0.0.53.tar.gz` & `tmp/monisha-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.53.tar", last modified: Tue Apr 16 19:22:26 2024, max compression
+gzip compressed data, was "monisha-0.0.54.tar", last modified: Sat Apr 20 18:59:57 2024, max compression
```

## Comparing `monisha-0.0.53.tar` & `monisha-0.0.54.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.967886 monisha-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 19:22:19.000000 monisha-0.0.53/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.959886 monisha-0.0.53/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.963886 monisha-0.0.53/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/functions/function15.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.963886 monisha-0.0.53/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 19:22:19.000000 monisha-0.0.53/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 19:22:26.967886 monisha-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 19:22:19.000000 monisha-0.0.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:22:26.967886 monisha-0.0.53/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 19:22:26.000000 monisha-0.0.53/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:22:26.967886 monisha-0.0.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 19:22:19.000000 monisha-0.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.293885 monisha-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-20 18:59:52.000000 monisha-0.0.54/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.289885 monisha-0.0.54/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.289885 monisha-0.0.54/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function16.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.293885 monisha-0.0.54/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 18:59:57.293885 monisha-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-20 18:59:52.000000 monisha-0.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.293885 monisha-0.0.54/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:59:57.293885 monisha-0.0.54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 18:59:52.000000 monisha-0.0.54/setup.py
```

### Comparing `monisha-0.0.53/LICENSE` & `monisha-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/__init__.py` & `monisha-0.0.54/Monisha/functions/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .function14 import CDirectory, UDirectory, BDirectory
 from .function01 import timend, uptime, Timemod, Timesod
 from .function06 import Okeys, Ukeys, Bkeys, Mkeys
-from .function06 import Ykeys, Skeys, Uname
+from .function16 import filestype, filextype
 from .function03 import progress, Progress
 from .function04 import Rawexo, Extions
 from .function02 import Dbytes, Hbytes
+from .function06 import Skeys, Uname
 from .function07 import Cmd, Wosd
+from .function15 import Location
 from .function10 import Fonts
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
 from .function09 import Sage
 from .function08 import Num
-from .function15 import Location
```

### Comparing `monisha-0.0.53/Monisha/functions/function01.py` & `monisha-0.0.54/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function02.py` & `monisha-0.0.54/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function03.py` & `monisha-0.0.54/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function04.py` & `monisha-0.0.54/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function06.py` & `monisha-0.0.54/Monisha/functions/function06.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,31 +38,14 @@
 class Uname(object):
 
     DATA04 = "ＤＣ４ ＷＡＲＲＩＯＲ"
     DATA05 = "ＤＣ５ ＷＡＲＲＩＯＲ"
 
 #================================================================================
 
-class Ykeys(object):
-
-    DATA08 = str("ext")
-    DATA09 = str("login")
-    DATA05 = str("format")
-    DATA01 = str("formats")
-    DATA06 = str("filesize")
-    DATA02 = str("duration")
-    DATA10 = str("username")
-    DATA11 = str("password")
-    DATA03 = str("format_id")
-    DATA04 = str("format_note")
-    DATA07 = str("filesize_approx")
-    DATA12 = str("geo_bypass_country")
-
-#================================================================================
-
 class Skeys(object):
 
     DATA01 = "0123456789"
     DATA02 = "abcdefghijklmnopqrstuvwxyz"
     DATA03 = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
     DATA04 = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
```

### Comparing `monisha-0.0.53/Monisha/functions/function07.py` & `monisha-0.0.54/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function10.py` & `monisha-0.0.54/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function14.py` & `monisha-0.0.54/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/functions/function15.py` & `monisha-0.0.54/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/Monisha/scripts/es.py` & `monisha-0.0.54/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.53/PKG-INFO` & `monisha-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.53
+Version: 0.0.54
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.53 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.54 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.53/monisha.egg-info/PKG-INFO` & `monisha-0.0.54/monisha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.53
+Version: 0.0.54
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.53 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.54 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.53/monisha.egg-info/SOURCES.txt` & `monisha-0.0.54/monisha.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Monisha/functions/function09.py
 Monisha/functions/function10.py
 Monisha/functions/function11.py
 Monisha/functions/function12.py
 Monisha/functions/function13.py
 Monisha/functions/function14.py
 Monisha/functions/function15.py
+Monisha/functions/function16.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
```

### Comparing `monisha-0.0.53/setup.py` & `monisha-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
     description='ㅤ',
-    version='0.0.53',
+    version='0.0.54',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.10',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     url='https://github.com/Clinton-Abraham',
```

