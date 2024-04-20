# Comparing `tmp/casepy-0.0.4a1.tar.gz` & `tmp/casepy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.4a1.tar", last modified: Fri Apr 19 07:46:33 2024, max compression
+gzip compressed data, was "casepy-0.0.5.tar", last modified: Fri Apr 19 19:37:15 2024, max compression
```

## Comparing `casepy-0.0.4a1.tar` & `casepy-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.486967 casepy-0.0.4a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 07:46:27.000000 casepy-0.0.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:46:33.486967 casepy-0.0.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 07:46:27.000000 casepy-0.0.4a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:46:33.486967 casepy-0.0.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 07:46:27.000000 casepy-0.0.4a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.482967 casepy-0.0.4a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.486967 casepy-0.0.4a1/src/casepy/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 07:46:27.000000 casepy-0.0.4a1/src/casepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 07:46:27.000000 casepy-0.0.4a1/src/casepy/combination_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 07:46:27.000000 casepy-0.0.4a1/src/casepy/simple_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.486967 casepy-0.0.4a1/src/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:15.882095 casepy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 19:37:09.000000 casepy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-19 19:37:15.882095 casepy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-19 19:37:09.000000 casepy-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:37:15.882095 casepy-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 19:37:09.000000 casepy-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:15.882095 casepy-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:15.882095 casepy-0.0.5/src/casepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 19:37:09.000000 casepy-0.0.5/src/casepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 19:37:09.000000 casepy-0.0.5/src/casepy/combination_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-19 19:37:09.000000 casepy-0.0.5/src/casepy/permutation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 19:37:09.000000 casepy-0.0.5/src/casepy/simple_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:15.882095 casepy-0.0.5/src/casepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-19 19:37:15.000000 casepy-0.0.5/src/casepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 19:37:15.000000 casepy-0.0.5/src/casepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:37:15.000000 casepy-0.0.5/src/casepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 19:37:15.000000 casepy-0.0.5/src/casepy.egg-info/top_level.txt
```

### Comparing `casepy-0.0.4a1/LICENSE` & `casepy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.4a1/PKG-INFO` & `casepy-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.4a1
+Version: 0.0.5
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -34,33 +34,45 @@
 With casepy, you can easily generate a combination of elements in a list.
 
 - Example
 
 Initialize generator
 
 ``` Python
-generator = CombinationGenerator()
-generator.set_parameters(4, [1,2,3,4,5])
+import casepy
+generator_combination = casepy.CombinationGenerator()
+# generating combination cases
+generator_permutation = casepy.PermutationGenerator()
+# generating permutation cases
+
+generator_combination.set_parameters(4, [1,2,3,4,5])
+generator_permutation.set_parameters(4, [1,2,3,4,5])
 ```
 
 all_case()
 
 ``` Python
-all_case_list = generator.all_case()
+all_case_list = generator_combination.all_case()
 # [[1, 2, 3, 4], [1, 2, 3, 5], [1, 2, 4, 5], [1, 3, 4, 5], [2, 3, 4, 5]]
+all_case_list = generator_permutation.all_case()
+# [[1, 2, 3, 4], [1, 2, 3, 5], [1, 2, 4, 3], [1, 2, 4, 5], ...] total 120 cases
 ```
 random_case()
 ``` Python
-random_case = generator.random_case()
+random_case = generator_combination.random_case()
 # [1, 2, 4, 5] // It can be difference
+random_case = generator_permutation.random_case()
+# [2, 4, 3, 5] // It can be difference
 ```
 i_case
 ``` Python
-i_case_3 = generator.i_case(3)
+i_case_3 = generator_combination.i_case(3)
 # [1,3,4,5]
+i_case_3 = generator_permutation.i_case(3)
+# [1,2,4,5]
 ```
 
 ------------
 
 This is my first own made Python package.
 
 Please feel free to let me know any feedback or suggestions.
```

### Comparing `casepy-0.0.4a1/README.md` & `casepy-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,33 +22,45 @@
 With casepy, you can easily generate a combination of elements in a list.
 
 - Example
 
 Initialize generator
 
 ``` Python
-generator = CombinationGenerator()
-generator.set_parameters(4, [1,2,3,4,5])
+import casepy
+generator_combination = casepy.CombinationGenerator()
+# generating combination cases
+generator_permutation = casepy.PermutationGenerator()
+# generating permutation cases
+
+generator_combination.set_parameters(4, [1,2,3,4,5])
+generator_permutation.set_parameters(4, [1,2,3,4,5])
 ```
 
 all_case()
 
 ``` Python
-all_case_list = generator.all_case()
+all_case_list = generator_combination.all_case()
 # [[1, 2, 3, 4], [1, 2, 3, 5], [1, 2, 4, 5], [1, 3, 4, 5], [2, 3, 4, 5]]
+all_case_list = generator_permutation.all_case()
+# [[1, 2, 3, 4], [1, 2, 3, 5], [1, 2, 4, 3], [1, 2, 4, 5], ...] total 120 cases
 ```
 random_case()
 ``` Python
-random_case = generator.random_case()
+random_case = generator_combination.random_case()
 # [1, 2, 4, 5] // It can be difference
+random_case = generator_permutation.random_case()
+# [2, 4, 3, 5] // It can be difference
 ```
 i_case
 ``` Python
-i_case_3 = generator.i_case(3)
+i_case_3 = generator_combination.i_case(3)
 # [1,3,4,5]
+i_case_3 = generator_permutation.i_case(3)
+# [1,2,4,5]
 ```
 
 ------------
 
 This is my first own made Python package.
 
 Please feel free to let me know any feedback or suggestions.
```

### Comparing `casepy-0.0.4a1/setup.py` & `casepy-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="casepy",
     py_modules=["casepy"],
-    version="0.0.4a1",
+    version="0.0.5",
     description="A Python package for generating cases in a list.",
     url="https://github.com/DongHoon5793/casepy",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     author="DongHoon Kim",
     author_email="donghoon5793@gmail.com",
```

### Comparing `casepy-0.0.4a1/src/casepy/combination_generator.py` & `casepy-0.0.5/src/casepy/combination_generator.py`

 * *Files identical despite different names*

### Comparing `casepy-0.0.4a1/src/casepy/simple_methods.py` & `casepy-0.0.5/src/casepy/simple_methods.py`

 * *Files identical despite different names*

### Comparing `casepy-0.0.4a1/src/casepy.egg-info/PKG-INFO` & `casepy-0.0.5/src/casepy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.4a1
+Version: 0.0.5
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -34,33 +34,45 @@
 With casepy, you can easily generate a combination of elements in a list.
 
 - Example
 
 Initialize generator
 
 ``` Python
-generator = CombinationGenerator()
-generator.set_parameters(4, [1,2,3,4,5])
+import casepy
+generator_combination = casepy.CombinationGenerator()
+# generating combination cases
+generator_permutation = casepy.PermutationGenerator()
+# generating permutation cases
+
+generator_combination.set_parameters(4, [1,2,3,4,5])
+generator_permutation.set_parameters(4, [1,2,3,4,5])
 ```
 
 all_case()
 
 ``` Python
-all_case_list = generator.all_case()
+all_case_list = generator_combination.all_case()
 # [[1, 2, 3, 4], [1, 2, 3, 5], [1, 2, 4, 5], [1, 3, 4, 5], [2, 3, 4, 5]]
+all_case_list = generator_permutation.all_case()
+# [[1, 2, 3, 4], [1, 2, 3, 5], [1, 2, 4, 3], [1, 2, 4, 5], ...] total 120 cases
 ```
 random_case()
 ``` Python
-random_case = generator.random_case()
+random_case = generator_combination.random_case()
 # [1, 2, 4, 5] // It can be difference
+random_case = generator_permutation.random_case()
+# [2, 4, 3, 5] // It can be difference
 ```
 i_case
 ``` Python
-i_case_3 = generator.i_case(3)
+i_case_3 = generator_combination.i_case(3)
 # [1,3,4,5]
+i_case_3 = generator_permutation.i_case(3)
+# [1,2,4,5]
 ```
 
 ------------
 
 This is my first own made Python package.
 
 Please feel free to let me know any feedback or suggestions.
```

