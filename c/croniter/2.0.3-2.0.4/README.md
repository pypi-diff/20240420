# Comparing `tmp/croniter-2.0.3.tar.gz` & `tmp/croniter-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croniter-2.0.3.tar", last modified: Tue Mar 19 08:14:49 2024, max compression
+gzip compressed data, was "croniter-2.0.4.tar", last modified: Sat Apr 20 17:49:34 2024, max compression
```

## Comparing `croniter-2.0.3.tar` & `croniter-2.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:49.036622 croniter-2.0.3/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    12026 2024-03-19 08:14:48.000000 croniter-2.0.3/CHANGELOG.rst
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1064 2024-03-19 08:14:48.000000 croniter-2.0.3/LICENSE
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      144 2024-03-19 08:14:48.000000 croniter-2.0.3/MANIFEST.in
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    25407 2024-03-19 08:14:49.036622 croniter-2.0.3/PKG-INFO
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    12017 2024-03-19 08:14:48.000000 croniter-2.0.3/README.rst
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:49.036622 croniter-2.0.3/requirements/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       33 2024-03-19 08:14:48.000000 croniter-2.0.3/requirements/base.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       44 2024-03-19 08:14:48.000000 croniter-2.0.3/requirements/release.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      109 2024-03-19 08:14:48.000000 croniter-2.0.3/requirements/test.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      324 2024-03-19 08:14:49.036622 croniter-2.0.3/setup.cfg
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     2121 2024-03-19 08:14:48.000000 croniter-2.0.3/setup.py
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:49.036622 croniter-2.0.3/src/
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:49.036622 croniter-2.0.3/src/croniter/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      380 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/__init__.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    37798 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/croniter.py
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:49.036622 croniter-2.0.3/src/croniter/tests/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/__init__.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      282 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/base.py
--rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)    63307 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/test_croniter.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    17178 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/test_croniter_hash.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1705 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/test_croniter_random.py
--rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)     6786 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/test_croniter_range.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     5715 2024-03-19 08:14:48.000000 croniter-2.0.3/src/croniter/tests/test_speed.py
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-03-19 08:14:49.036622 croniter-2.0.3/src/croniter.egg-info/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    25407 2024-03-19 08:14:49.000000 croniter-2.0.3/src/croniter.egg-info/PKG-INFO
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      622 2024-03-19 08:14:49.000000 croniter-2.0.3/src/croniter.egg-info/SOURCES.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        1 2024-03-19 08:14:49.000000 croniter-2.0.3/src/croniter.egg-info/dependency_links.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       28 2024-03-19 08:14:49.000000 croniter-2.0.3/src/croniter.egg-info/requires.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        9 2024-03-19 08:14:49.000000 croniter-2.0.3/src/croniter.egg-info/top_level.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      625 2024-03-19 08:14:48.000000 croniter-2.0.3/tox.ini
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:34.153877 croniter-2.0.4/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    12231 2024-04-20 17:49:33.000000 croniter-2.0.4/CHANGELOG.rst
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1064 2024-04-20 17:49:33.000000 croniter-2.0.4/LICENSE
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      144 2024-04-20 17:49:33.000000 croniter-2.0.4/MANIFEST.in
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    25612 2024-04-20 17:49:34.153877 croniter-2.0.4/PKG-INFO
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    12017 2024-04-20 17:49:33.000000 croniter-2.0.4/README.rst
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:34.153877 croniter-2.0.4/requirements/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       33 2024-04-20 17:49:33.000000 croniter-2.0.4/requirements/base.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       44 2024-04-20 17:49:33.000000 croniter-2.0.4/requirements/release.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      109 2024-04-20 17:49:33.000000 croniter-2.0.4/requirements/test.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      324 2024-04-20 17:49:34.153877 croniter-2.0.4/setup.cfg
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     2121 2024-04-20 17:49:33.000000 croniter-2.0.4/setup.py
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:34.149877 croniter-2.0.4/src/
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:34.153877 croniter-2.0.4/src/croniter/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      380 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/__init__.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    38437 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/croniter.py
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:34.153877 croniter-2.0.4/src/croniter/tests/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/__init__.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      282 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/base.py
+-rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)    63715 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/test_croniter.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    17178 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/test_croniter_hash.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1705 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/test_croniter_random.py
+-rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)     6786 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/test_croniter_range.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     5715 2024-04-20 17:49:33.000000 croniter-2.0.4/src/croniter/tests/test_speed.py
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2024-04-20 17:49:34.153877 croniter-2.0.4/src/croniter.egg-info/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    25612 2024-04-20 17:49:34.000000 croniter-2.0.4/src/croniter.egg-info/PKG-INFO
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      622 2024-04-20 17:49:34.000000 croniter-2.0.4/src/croniter.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        1 2024-04-20 17:49:34.000000 croniter-2.0.4/src/croniter.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       28 2024-04-20 17:49:34.000000 croniter-2.0.4/src/croniter.egg-info/requires.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        9 2024-04-20 17:49:34.000000 croniter-2.0.4/src/croniter.egg-info/top_level.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      625 2024-04-20 17:49:33.000000 croniter-2.0.4/tox.ini
```

### Comparing `croniter-2.0.3/CHANGELOG.rst` & `croniter-2.0.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 ==============
 
+2.0.4 (2024-04-20)
+------------------
+
+- Support hashid strings in is_valid [george-kuanli-peng, kiorky]
+- Avoid over-optimization in crontab expansions [Cherie0125, liqirui <liqirui@baidu.com>, kiorky]
+
+
 2.0.3 (2024-03-19)
 ------------------
 
 - Add match_range function [salitaba]
 
 
 2.0.2 (2024-02-29)
```

### Comparing `croniter-2.0.3/LICENSE` & `croniter-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/PKG-INFO` & `croniter-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croniter
-Version: 2.0.3
+Version: 2.0.4
 Summary: croniter provides iteration for datetime object with cron like format
 Home-page: http://github.com/kiorky/croniter
 Author: Matsumoto Taichi, kiorky
 Author-email: taichino@gmail.com, kiorky@cryptelium.net
 License: MIT License
 Keywords: datetime,iterator,cron
 Platform: UNKNOWN
@@ -344,14 +344,21 @@
     - salitaba
 
 
 
 Changelog
 ==============
 
+2.0.4 (2024-04-20)
+------------------
+
+- Support hashid strings in is_valid [george-kuanli-peng, kiorky]
+- Avoid over-optimization in crontab expansions [Cherie0125, liqirui <liqirui@baidu.com>, kiorky]
+
+
 2.0.3 (2024-03-19)
 ------------------
 
 - Add match_range function [salitaba]
 
 
 2.0.2 (2024-02-29)
```

### Comparing `croniter-2.0.3/README.rst` & `croniter-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/setup.py` & `croniter-2.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         read('README.rst'),
         read('CHANGELOG.rst'),
     ]
 )
 
 setup(
     name='croniter',
-    version='2.0.3',
+    version='2.0.4',
     py_modules=['croniter', ],
     description=(
         'croniter provides iteration for datetime '
         'object with cron like format'
     ),
     long_description=long_description,
     author="Matsumoto Taichi, kiorky",
```

### Comparing `croniter-2.0.3/src/croniter/croniter.py` & `croniter-2.0.4/src/croniter/croniter.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,26 +783,32 @@
                         if t not in nth_weekday_of_month:
                             nth_weekday_of_month[t] = set()
                         nth_weekday_of_month[t].add(nth)
 
             res = set(res)
             res = sorted(res, key=lambda i: "{:02}".format(i) if isinstance(i, int) else i)
             if len(res) == cls.LEN_MEANS_ALL[i]:
-                res = ['*']
+                # Make sure the wildcard is used in the correct way (avoid over-optimization)
+                if ((i == 2 and '*' not in expressions[4]) or
+                    (i == 4 and '*' not in expressions[2])):
+                    pass
+                else:
+                    res = ['*']
 
             expanded.append(['*'] if (len(res) == 1
                                       and res[0] == '*')
                             else res)
 
         # Check to make sure the dow combo in use is supported
         if nth_weekday_of_month:
             dow_expanded_set = set(expanded[4])
             dow_expanded_set = dow_expanded_set.difference(nth_weekday_of_month.keys())
             dow_expanded_set.discard("*")
-            if dow_expanded_set:
+            # Skip: if it's all weeks instead of wildcard
+            if dow_expanded_set and len(set(expanded[4])) != cls.LEN_MEANS_ALL[4]:
                 raise CroniterUnsupportedSyntaxError(
                     "day-of-week field does not support mixing literal values and nth day of week syntax.  "
                     "Cron: '{}'    dow={} vs nth={}".format(expr_format, dow_expanded_set, nth_weekday_of_month))
 
         EXPRESSIONS[(expr_format, hash_id)] = expressions
         return expanded, nth_weekday_of_month
 
@@ -819,15 +825,20 @@
                 trace = _traceback.format_exc()
                 globs, locs = _get_caller_globals_and_locals()
                 raise CroniterBadCronError(trace)
             else:
                 raise CroniterBadCronError("{0}".format(exc))
 
     @classmethod
-    def is_valid(cls, expression, hash_id=None):
+    def is_valid(cls, expression, hash_id=None, encoding='UTF-8'):
+        if hash_id:
+            if not isinstance(hash_id, (bytes, str)):
+                raise TypeError('hash_id must be bytes or UTF-8 string')
+            if not isinstance(hash_id, bytes):
+                hash_id = hash_id.encode(encoding)
         try:
             cls.expand(expression, hash_id=hash_id)
         except CroniterError:
             return False
         else:
             return True
```

### Comparing `croniter-2.0.3/src/croniter/tests/test_croniter.py` & `croniter-2.0.4/src/croniter/tests/test_croniter.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,19 +340,23 @@
     def testOptimizeCronExpressions(self):
         """ Non-optimal cron expressions that can be simplified."""
         wildcard = ['*']
         m, h, d, mon, dow, s = range(6)
         # Test each field individually
         self.assertEqual(croniter('0-59 0 1 1 0').expanded[m], wildcard)
         self.assertEqual(croniter('0 0-23 1 1 0').expanded[h], wildcard)
-        self.assertEqual(croniter('0 0 1-31 1 0').expanded[d], wildcard)
+        self.assertEqual(croniter('0 0 1-31 1 0').expanded[dow], [0])
+        self.assertEqual(croniter('0 0 1-31 1 *').expanded[d], wildcard)
         self.assertEqual(croniter('0 0 1 1-12 0').expanded[mon], wildcard)
-        self.assertEqual(croniter('0 0 1 1 0-6').expanded[dow], wildcard)
-        self.assertEqual(croniter('0 0 1 1 1-7').expanded[dow], wildcard)
-        self.assertEqual(croniter('0 0 1 1 1-7,sat#3').expanded[dow], wildcard)
+        self.assertEqual(croniter('0 0 1 1 0-6').expanded[dow], [0, 1, 2, 3, 4, 5, 6])
+        self.assertEqual(croniter('0 0 * 1 0-6').expanded[dow], wildcard)
+        self.assertEqual(croniter('0 0 1 1 1-7').expanded[dow], [0, 1, 2, 3, 4, 5, 6])
+        self.assertEqual(croniter('0 0 1 1 1-7,sat#3').expanded[dow], [0, 1, 2, 3, 4, 5, 6])
+        self.assertEqual(croniter('0 0 * 1 1-7').expanded[dow], wildcard)
+        self.assertEqual(croniter('0 0 * 1 1-7,sat#3').expanded[dow], wildcard)
         self.assertEqual(croniter('0 0 1 1 0 0-59').expanded[s], wildcard)
         # Real life examples
         self.assertEqual(croniter('30 1-12,0,10-23 15-21 * fri').expanded[h], wildcard)
         self.assertEqual(croniter('30 1-23,0 15-21 * fri').expanded[h], wildcard)
 
     def testBlockDupRanges(self):
         """ Ensure that duplicate/overlapping ranges are squashed """
@@ -892,14 +896,15 @@
         self.assertRaises(CroniterBadCronError, croniter.expand,
                           '* * * * * * *')
 
     def test_is_valid(self):
         self.assertTrue(croniter.is_valid('0 * * * *'))
         self.assertFalse(croniter.is_valid('0 * *'))
         self.assertFalse(croniter.is_valid('* * * janu-jun *'))
+        self.assertTrue(croniter.is_valid('H 0 * * *', hash_id='abc'))
 
     def test_exactly_the_same_minute(self):
         base = datetime(2018, 3, 5, 12, 30, 50)
         itr = croniter('30 7,12,17 * * *', base)
         n1 = itr.get_prev(datetime)
         self.assertEqual(12, n1.hour)
```

### Comparing `croniter-2.0.3/src/croniter/tests/test_croniter_hash.py` & `croniter-2.0.4/src/croniter/tests/test_croniter_hash.py`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/src/croniter/tests/test_croniter_random.py` & `croniter-2.0.4/src/croniter/tests/test_croniter_random.py`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/src/croniter/tests/test_croniter_range.py` & `croniter-2.0.4/src/croniter/tests/test_croniter_range.py`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/src/croniter/tests/test_speed.py` & `croniter-2.0.4/src/croniter/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/src/croniter.egg-info/PKG-INFO` & `croniter-2.0.4/src/croniter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croniter
-Version: 2.0.3
+Version: 2.0.4
 Summary: croniter provides iteration for datetime object with cron like format
 Home-page: http://github.com/kiorky/croniter
 Author: Matsumoto Taichi, kiorky
 Author-email: taichino@gmail.com, kiorky@cryptelium.net
 License: MIT License
 Keywords: datetime,iterator,cron
 Platform: UNKNOWN
@@ -344,14 +344,21 @@
     - salitaba
 
 
 
 Changelog
 ==============
 
+2.0.4 (2024-04-20)
+------------------
+
+- Support hashid strings in is_valid [george-kuanli-peng, kiorky]
+- Avoid over-optimization in crontab expansions [Cherie0125, liqirui <liqirui@baidu.com>, kiorky]
+
+
 2.0.3 (2024-03-19)
 ------------------
 
 - Add match_range function [salitaba]
 
 
 2.0.2 (2024-02-29)
```

### Comparing `croniter-2.0.3/src/croniter.egg-info/SOURCES.txt` & `croniter-2.0.4/src/croniter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croniter-2.0.3/tox.ini` & `croniter-2.0.4/tox.ini`

 * *Files identical despite different names*

