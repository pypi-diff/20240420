# Comparing `tmp/mo_testing-7.587.24110.tar.gz` & `tmp/mo_testing-8.589.24111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_testing-7.587.24110.tar", last modified: Fri Apr 19 03:13:34 2024, max compression
+gzip compressed data, was "mo_testing-8.589.24111.tar", last modified: Sat Apr 20 01:35:16 2024, max compression
```

## Comparing `mo_testing-7.587.24110.tar` & `mo_testing-8.589.24111.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 03:13:34.052117 mo_testing-7.587.24110/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-7.587.24110/LICENSE
--rw-rw-rw-   0        0        0     2047 2024-04-19 03:13:34.051107 mo_testing-7.587.24110/PKG-INFO
--rw-rw-rw-   0        0        0      946 2020-05-12 21:52:10.000000 mo_testing-7.587.24110/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 03:13:34.040584 mo_testing-7.587.24110/mo_testing/
--rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo_testing-7.587.24110/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    11849 2024-04-19 03:13:23.000000 mo_testing-7.587.24110/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:13:34.050107 mo_testing-7.587.24110/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2047 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 03:13:34.053117 mo_testing-7.587.24110/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-04-19 03:13:26.000000 mo_testing-7.587.24110/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:35:16.695352 mo_testing-8.589.24111/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.589.24111/LICENSE
+-rw-rw-rw-   0        0        0     2699 2024-04-20 01:35:16.695352 mo_testing-8.589.24111/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2024-04-20 01:35:09.000000 mo_testing-8.589.24111/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 01:35:16.687044 mo_testing-8.589.24111/mo_testing/
+-rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo_testing-8.589.24111/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    11643 2024-04-20 01:35:09.000000 mo_testing-8.589.24111/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:35:16.694354 mo_testing-8.589.24111/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2699 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 01:35:16.696634 mo_testing-8.589.24111/setup.cfg
+-rw-rw-rw-   0        0        0     2679 2024-04-20 01:35:12.000000 mo_testing-8.589.24111/setup.py
```

### Comparing `mo_testing-7.587.24110/LICENSE` & `mo_testing-8.589.24111/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_testing-7.587.24110/PKG-INFO` & `mo_testing-8.589.24111/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 7.587.24110
+Version: 8.589.24111
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -16,26 +16,35 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-collections==5.584.24095
 Requires-Dist: mo-dots==9.584.24095
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-logs==8.584.24095
-Requires-Dist: mo-math==7.584.24095
-Requires-Dist: mo-threads==6.585.24095
+Requires-Dist: mo-math==7.589.24111
+Requires-Dist: mo-threads==6.589.24111
 Provides-Extra: tests
+Requires-Dist: mo_times; extra == "tests"
+Requires-Dist: mo_logs; extra == "tests"
 
 # More Testing
 
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)
+[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)
+[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)
+[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)
+
+
 `FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.
 
 
 ## Details
 
-The primary method is the `assertEqual` method with the following parameters:
+The primary method is the `assertAlmostEqual` method with the following parameters:
 
 * `test_value` - the value, or structure being tested
 * `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.
 * `msg` - Detailed error message if there is no match
 * `digits` - number of decimal places of accuracy required to consider two values equal
 * `places` - number of significant digits used to compare values for accuracy
 * `delta` - maximum difference between values for them to be equal
```

### Comparing `mo_testing-7.587.24110/mo_testing/fuzzytestcase.py` & `mo_testing-8.589.24111/mo_testing/fuzzytestcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,56 +10,60 @@
 
 
 import datetime
 import types
 import unittest
 from unittest import SkipTest, TestCase
 
-import mo_dots
 import mo_math
 from mo_collections.unique_index import UniqueIndex
-from mo_dots import coalesce, is_list, literal_field, from_data, to_data, is_data, is_many
+from mo_dots import coalesce, is_list, literal_field, from_data, to_data, is_data, is_many,is_missing, get_attr
 from mo_future import is_text, zip_longest, first, get_function_name
 from mo_logs import Except, Log, suppress_exception
 from mo_logs.strings import expand_template, quote
-from mo_math import is_number, log10
+from mo_math import is_number, log10, COUNT
 from mo_times import dates
 
 
 class FuzzyTestCase(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         unittest.TestCase.__init__(self, *args, **kwargs)
-        self.default_places=15
-
+        self.default_places = 15
 
     def set_default_places(self, places):
         """
         WHEN COMPARING float, HOW MANY DIGITS ARE SIGNIFICANT BY DEFAULT
         """
-        self.default_places=places
+        self.default_places = places
 
-    def assertAlmostEqual(self, test_value, expected, msg=None, digits=None, places=None, delta=None):
+    def assertAlmostEqual(self, test_value, expected, *, msg=None, digits=None, places=None, delta=None):
         if delta or digits:
             assertAlmostEqual(test_value, expected, msg=msg, digits=digits, places=places, delta=delta)
         else:
-            assertAlmostEqual(test_value, expected, msg=msg, digits=digits, places=coalesce(places, self.default_places), delta=delta)
+            assertAlmostEqual(
+                test_value,
+                expected,
+                msg=msg,
+                digits=digits,
+                places=coalesce(places, self.default_places),
+                delta=delta
+            )
 
-    def assertEqual(self, test_value, expected, msg=None, digits=None, places=None, delta=None):
+    def assertEqual(self, test_value, expected, *, msg=None, digits=None, places=None, delta=None):
         self.assertAlmostEqual(test_value, expected, msg=msg, digits=digits, places=places, delta=delta)
 
     def assertRaises(self, problem=None, function=None, *args, **kwargs):
         if function is None:
             return RaiseContext(self, problem=problem or Exception)
 
         with RaiseContext(self, problem=problem):
             function(*args, **kwargs)
 
 
 class RaiseContext(object):
-
     def __init__(self, testcase, problem=Exception):
         self.testcase = testcase
         self.problem = problem
 
     def __enter__(self):
         pass
 
@@ -71,95 +75,110 @@
         if isinstance(self.problem, (list, tuple)):
             problems = self.problem
         else:
             problems = [self.problem]
 
         causes = []
         for problem in problems:
-            if isinstance(problem, object.__class__) and issubclass(problem, BaseException) and isinstance(exc_val, problem):
+            if (
+                isinstance(problem, object.__class__)
+                and issubclass(problem, BaseException)
+                and isinstance(exc_val, problem)
+            ):
                 return True
             try:
                 self.testcase.assertIn(problem, f)
                 return True
             except Exception as cause:
                 causes.append(cause)
         Log.error("problem is not raised", cause=first(causes))
 
 
-def assertAlmostEqual(test, expected, digits=None, places=None, msg=None, delta=None):
+def assertAlmostEqual(test, expected, *, digits=None, places=None, msg=None, delta=None):
     """
-    COMPARE STRUCTURE AND NUMBERS!
+    COMPARE STRUCTURE AND NUMBERS
 
-    ONLY THE ATTRIBUTES IN THE expected STRUCTURE ARE TESTED TO EXIST
-    EXTRA ATTRIBUTES ARE IGNORED.
+    STRUCTURE IS COMPARED BY ...
+    * PROPERTIES IN THE expected STRUCTURE ARE TESTED TO EXIST IN test
+    * PROPERTIES IN test THAT ARE NOT FOUND IN expected ARE IGNORED
+    * IF expected IS A FUNCTION, THEN IT IS CALLED WITH test AS ARGUMENT
+    * IF expected IS A SET, THEN ORDER DOES NOT MATTER
+    * SINGLETON LIST MATCHES THE SINGLETON
+    * IF expected IS AN EMPTY LIST, THEN test MUST BE MISSING (None, or empty list)
 
     NUMBERS ARE MATCHED BY ...
     * places (UP TO GIVEN SIGNIFICANT DIGITS)
     * digits (UP TO GIVEN DECIMAL PLACES, WITH NEGATIVE MEANING LEFT-OF-UNITS)
     * delta (MAXIMUM ABSOLUTE DIFFERENCE FROM expected)
     """
     show_detail = True
     test = from_data(test)
     expected = from_data(expected)
     try:
-        if test is None and (is_null_op(expected) or expected is None):
+        if test is expected:
             return
-        elif test is expected:
+        elif test is None and (is_null_op(expected) or is_missing(expected)):
             return
         elif is_text(expected):
             assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
         elif isinstance(test, UniqueIndex):
             if test ^ expected:
                 Log.error("Sets do not match")
+        elif not is_many(test) and is_list(expected) and len(expected)==1:
+            assertAlmostEqual(test, expected[0], msg=msg, digits=digits, places=places, delta=delta)
         elif is_data(expected) and is_data(test):
             for k, e in from_data(expected).items():
                 t = test.get(k)
                 try:
-                    assertAlmostEqual(t, e, msg=coalesce(msg, "")+"key "+quote(k)+": ", digits=digits, places=places, delta=delta)
+                    assertAlmostEqual(
+                        t,
+                        e,
+                        msg=coalesce(msg, "") + "key " + quote(k) + ": ",
+                        digits=digits,
+                        places=places,
+                        delta=delta,
+                    )
                 except Exception as cause:
                     Log.error("key {k}={t} does not match expected {k}={e}", k=k, t=t, e=e, cause=cause)
         elif is_data(expected):
             if is_many(test):
                 test = list(test)
                 if len(test) != 1:
                     Log.error("Expecting data, not a list")
                 test = test[0]
             for k, e in expected.items():
+                t = get_attr(test, literal_field(k))
                 try:
-                    t = test[k]
                     assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
-                    continue
-                except:
-                    pass
-
-                t = mo_dots.get_attr(test, literal_field(k))
-                assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
+                except Exception as cause:
+                    Log.error("key {k}={t} does not match expected {k}={e}", k=k, t=t, e=e, cause=cause)
         elif is_many(test) and isinstance(expected, set):
             test = set(to_data(t) for t in test)
             if len(test) != len(expected):
                 Log.error(
-                    "Sets do not match, element count different:\n{{test|json|indent}}\nexpecting{{expectedtest|json|indent}}",
+                    "Sets do not match, element count"
+                    " different:\n{{test|json|indent}}\nexpecting{{expectedtest|json|indent}}",
                     test=test,
-                    expected=expected
+                    expected=expected,
                 )
 
             try:
-                if len(test|expected) != len(test):
+                if len(test | expected) != len(test):
                     raise Exception()
             except:
                 for e in expected:
                     for t in test:
                         try:
                             assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
                             break
                         except Exception as _:
                             pass
                     else:
                         Log.error("Sets do not match. {{value|json}} not found in {{test|json}}", value=e, test=test)
-            return   # ok
+            return  # ok
         elif isinstance(expected, types.FunctionType):
             return expected(test)
         elif hasattr(test, "__iter__") and hasattr(expected, "__iter__"):
             if test.__class__.__name__ == "ndarray":  # numpy
                 test = test.tolist()
             elif test.__class__.__name__ == "DataFrame":  # pandas
                 test = test[test.columns[0]].values.tolist()
@@ -175,81 +194,52 @@
         else:
             assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
     except Exception as cause:
         Log.error(
             "{{test|json|limit(10000)}} does not match expected {{expected|json|limit(10000)}}",
             test=test if show_detail else "[can not show]",
             expected=expected if show_detail else "[can not show]",
-            cause=cause
+            cause=cause,
         )
 
 
 def assertAlmostEqualValue(test, expected, digits=None, places=None, msg=None, delta=None):
     """
     Snagged from unittest/case.py, then modified (Aug2014)
     """
-    if is_null_op(expected):
-        if test == None:  # pandas dataframes reject any comparision with an exception!
-            return
-        else:
-            raise AssertionError(expand_template("{{test|json}} != NULL", locals()))
-
-    if expected == None:  # None has no expectations
-        return
     if test == expected:
-        # shortcut
         return
     if isinstance(expected, (dates.Date, datetime.datetime, datetime.date)):
         return assertAlmostEqualValue(
-            dates.Date(test).unix,
-            dates.Date(expected).unix,
-            msg=msg,
-            digits=digits,
-            places=places,
-            delta=delta
+            dates.Date(test).unix, dates.Date(expected).unix, msg=msg, digits=digits, places=places, delta=delta
         )
-
-    if not is_many(expected) and is_list(test) and len(test) == 1:
-        try:
-            return assertAlmostEqual(test[0], expected, msg=msg, digits=digits, places=places, delta=delta)
-        except:
-            pass
-
+    if is_list(test) and len(test) == 1:
+        return assertAlmostEqual(test[0], expected, msg=msg, digits=digits, places=places, delta=delta)
     if not is_number(expected):
-        # SOME SPECIAL CASES, EXPECTING EMPTY CONTAINERS IS THE SAME AS EXPECTING NULL
-        if is_list(expected) and len(expected) == 0 and test == None:
-            return
-        if is_data(expected) and not expected.keys() and test == None:
-            return
-        if test != expected:
-            raise AssertionError(expand_template("{{test|json}} != {{expected|json}}", locals()))
-        return
-    elif not is_number(test):
+        raise AssertionError(expand_template("{{test|json}} != {{expected|json}}", locals()))
+
+    expected = float(expected)
+    if not is_number(test):
         try:
             # ASSUME IT IS A UTC DATE
             test = dates.parse(test).unix
         except Exception as e:
             raise AssertionError(expand_template("{{test|json}} != {{expected}}", locals()))
 
     # WE NOW ASSUME test IS A NUMBER
     test = float(test)
+    if test == expected:
+        return
 
-    num_param = 0
-    if digits != None:
-        num_param += 1
-    if places != None:
-        num_param += 1
-    if delta != None:
-        num_param += 1
-    if num_param > 1:
+    if COUNT([digits, places, delta]) > 1:
         raise TypeError("specify only one of digits, places or delta")
 
     if digits is not None:
         with suppress_exception:
-            diff = round(abs(test-expected)*pow(10, digits))
+            diff = round(abs(test - expected) * pow(10, digits))
             if diff == 0:
                 return
 
         standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{digits}} decimal places", locals())
     elif delta is not None:
         if abs(test - expected) <= delta:
             return
@@ -257,60 +247,52 @@
         standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{delta}} delta", locals())
     else:
         if places is None:
             places = 15
 
         with suppress_exception:
             factor = mo_math.ceiling(log10(abs(test)))
-            diff = log10(abs(test-expected))-factor + places
+            diff = log10(abs(test - expected)) - factor + places
             if diff < -0.3:
                 return
 
         standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{places}} places", locals())
 
     raise AssertionError(coalesce(msg, "") + ": (" + standardMsg + ")")
 
 
 def is_null_op(v):
     return v.__class__.__name__ == "NullOp"
 
 
-_original_assertEqual = TestCase.assertEqual
-
-
-def assertEqual(self, test, expected, *args, **kwargs):
-    return _original_assertEqual(self, expected, test, *args, **kwargs)
-
-
-TestCase.assertEqual = assertEqual
-
-
 def add_error_reporting(suite):
     """
     Both unittest and pytest have become sophisticated enough to hide
     the problems cause by a test failure. Making debugging difficult.
     This method ensures a detailed error message is logged
     :param suite: The TestCase class (as @decorator)
     """
+
     def add_handler(function):
         test_name = get_function_name(function)
+
         def error_hanlder(*args, **kwargs):
             try:
                 return function(*args, **kwargs)
             except SkipTest as cause:
                 raise cause
             except Exception as cause:
                 Log.warning("{test_name} failed", cause=cause, test_name=test_name, static_template=False)
                 raise cause
 
         return error_hanlder
 
     if not hasattr(suite, "FuzzyTestCase.__modified__"):
         setattr(suite, "FuzzyTestCase.__modified__", True)
-        # find all methods, and wrap in exceptin handler
+        # find all methods, and wrap in exception handler
         for name, func in vars(suite).items():
             if name.startswith("test"):
                 h = add_handler(func)
                 h.__name__ = get_function_name(func)
                 setattr(suite, name, h)
     return suite
```

### Comparing `mo_testing-7.587.24110/mo_testing.egg-info/PKG-INFO` & `mo_testing-8.589.24111/mo_testing.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 7.587.24110
+Version: 8.589.24111
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -16,26 +16,35 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-collections==5.584.24095
 Requires-Dist: mo-dots==9.584.24095
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-logs==8.584.24095
-Requires-Dist: mo-math==7.584.24095
-Requires-Dist: mo-threads==6.585.24095
+Requires-Dist: mo-math==7.589.24111
+Requires-Dist: mo-threads==6.589.24111
 Provides-Extra: tests
+Requires-Dist: mo_times; extra == "tests"
+Requires-Dist: mo_logs; extra == "tests"
 
 # More Testing
 
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)
+[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)
+[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)
+[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)
+
+
 `FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.
 
 
 ## Details
 
-The primary method is the `assertEqual` method with the following parameters:
+The primary method is the `assertAlmostEqual` method with the following parameters:
 
 * `test_value` - the value, or structure being tested
 * `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.
 * `msg` - Detailed error message if there is no match
 * `digits` - number of decimal places of accuracy required to consider two values equal
 * `places` - number of significant digits used to compare values for accuracy
 * `delta` - maximum difference between values for them to be equal
```

### Comparing `mo_testing-7.587.24110/setup.py` & `mo_testing-8.589.24111/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons',
-    extras_require={"tests":[]},
+    extras_require={"tests":["mo_times","mo_logs"]},
     include_package_data=True,
-    install_requires=["mo-collections==5.584.24095","mo-dots==9.584.24095","mo-future==7.584.24095","mo-logs==8.584.24095","mo-math==7.584.24095","mo-threads==6.585.24095"],
+    install_requires=["mo-collections==5.584.24095","mo-dots==9.584.24095","mo-future==7.584.24095","mo-logs==8.584.24095","mo-math==7.589.24111","mo-threads==6.589.24111"],
     license='MPL 2.0',
-    long_description='# More Testing\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertEqual` method with the following parameters:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n\n',
+    long_description='# More Testing\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)\n[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)\n\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertAlmostEqual` method with the following parameters:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='7.587.24110'
+    version='8.589.24111'
 )
```

