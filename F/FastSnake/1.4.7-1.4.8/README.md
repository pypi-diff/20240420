# Comparing `tmp/fastsnake-1.4.7.tar.gz` & `tmp/fastsnake-1.4.8.tar.gz`

## Comparing `fastsnake-1.4.7.tar` & `fastsnake-1.4.8.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.7/requirements.txt
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.7/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/entries.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/application.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/config.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/contest.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/external.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/runner.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/external/__init__.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/structures/b_tree.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/util/atcoder.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/test_atcoder_problem_loader.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/0.in
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/0.out
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/1.in
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/1.out
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/test_codeforces_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_structures/test_b_tree.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.7/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.7/LICENSE
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 fastsnake-1.4.7/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastsnake-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 fastsnake-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.8/requirements.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/entries.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/application/application.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/application/config.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/application/contest.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/application/external.py
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/application/runner.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/external/__init__.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/util/atcoder.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 fastsnake-1.4.8/fastsnake/util/step_counter.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_atcoder_tools/test_atcoder_problem_loader.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_atcoder_tools/sample_abc341_E/0.in
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_atcoder_tools/sample_abc341_E/0.out
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_atcoder_tools/sample_abc341_E/1.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_atcoder_tools/sample_abc341_E/1.out
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_codeforces_tools/test_codeforces_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_step_counter/sample.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_step_counter/test_counter.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.8/tests/test_structures/test_b_tree.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.8/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.8/LICENSE
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 fastsnake-1.4.8/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastsnake-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 fastsnake-1.4.8/PKG-INFO
```

### Comparing `fastsnake-1.4.7/.github/workflows/python-package.yml` & `fastsnake-1.4.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/entries.py` & `fastsnake-1.4.8/fastsnake/entries.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.8/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.8/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/application/application.py` & `fastsnake-1.4.8/fastsnake/application/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,17 +224,17 @@
 
     # CLI Commands.
     elif args.command:
 
         # Test the solution.
         if args.command == "test":
             if args.generator:
-                result = run_test_generator(args.problem, args.generator)
+                result = run_test_generator(args.problem, args.generator, args.step_counter, debug=args.debug)
             else:
-                result = run_test(args.problem)
+                result = run_test(args.problem, args.step_counter, debug=args.debug)
 
             if result and args.test_and_compile: 
                 compile(args.problem, problem=True)
         
         # Compile a fastsnake solution.
         elif args.command == "compile":
             compile(args.filename)
```

### Comparing `fastsnake-1.4.7/fastsnake/application/arg_parser.py` & `fastsnake-1.4.8/fastsnake/application/arg_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 command_parser = main_parser.add_subparsers(title="Fastsnake CLI Commands", dest="command")
 
 # Testing Solutions.
 test_parser = command_parser.add_parser("test", help="Test a solution for a contest problem")
 test_parser.add_argument("problem", type=str, help="Problem of the contest")
 test_parser.add_argument("-c", "--compile", action="store_true", dest="test_and_compile", help="Test and compile the solution")
 test_parser.add_argument("-g", "--generator", type=int, metavar="n_tests", dest="generator", help="Use generator module to test the solution")
+test_parser.add_argument("-s", "--step-counter", action="store_true", dest="step_counter", help="Returns the approximate number of steps executed")
+test_parser.add_argument("--return-temp-module-for-debug", action="store_true", dest="debug")
 
 # Compiling Solutions.
 compile_parser = command_parser.add_parser("compile", help="Compile a python fastsnake solution")
 compile_parser.add_argument("filename", type=str, help="Python module")
 
 # Custom Contest.
 custom_contest_parser = command_parser.add_parser("start-custom-contest", help="Start a custom contest")
```

### Comparing `fastsnake-1.4.7/fastsnake/application/contest.py` & `fastsnake-1.4.8/fastsnake/application/contest.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/application/external.py` & `fastsnake-1.4.8/fastsnake/application/external.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/structures/b_tree.py` & `fastsnake-1.4.8/fastsnake/structures/b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/util/atcoder.py` & `fastsnake-1.4.8/fastsnake/util/atcoder.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/util/codeforces.py` & `fastsnake-1.4.8/fastsnake/util/codeforces.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/fastsnake/util/compiler.py` & `fastsnake-1.4.8/fastsnake/util/compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.8/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.8/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.8/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.8/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.8/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_atcoder_tools/test_atcoder_problem_loader.py` & `fastsnake-1.4.8/tests/test_atcoder_tools/test_atcoder_problem_loader.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_codeforces_tools/test_codeforces_problem_loader.py` & `fastsnake-1.4.8/tests/test_codeforces_tools/test_codeforces_problem_loader.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.8/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/tests/test_structures/test_b_tree.py` & `fastsnake-1.4.8/tests/test_structures/test_b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/.gitignore` & `fastsnake-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/LICENSE` & `fastsnake-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/README.md` & `fastsnake-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/pyproject.toml` & `fastsnake-1.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.7/PKG-INFO` & `fastsnake-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.4.7
+Version: 1.4.8
 Summary: A Python Helper CLI for Competitive Programming
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,cli,codeforces,competition,competitive programming,contest,helper,marathon,structures
 Classifier: Intended Audience :: Developers
```

