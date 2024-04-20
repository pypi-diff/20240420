# Comparing `tmp/fastsnake-1.4.6.tar.gz` & `tmp/fastsnake-1.4.7.tar.gz`

## Comparing `fastsnake-1.4.6.tar` & `fastsnake-1.4.7.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.6/requirements.txt
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/entries.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/application/application.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/application/config.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/application/contest.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/application/external.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/application/runner.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/external/__init__.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/structures/b_tree.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastsnake-1.4.6/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_codeforces_tools/test_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.6/tests/test_structures/test_b_tree.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.6/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.6/LICENSE
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 fastsnake-1.4.6/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastsnake-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 fastsnake-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.7/requirements.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/entries.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/application.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/config.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/contest.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/external.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/application/runner.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/external/__init__.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/util/atcoder.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastsnake-1.4.7/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/test_atcoder_problem_loader.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/0.in
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/0.out
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/1.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_atcoder_tools/sample_abc341_E/1.out
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/test_codeforces_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.7/tests/test_structures/test_b_tree.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.7/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.7/LICENSE
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 fastsnake-1.4.7/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastsnake-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 fastsnake-1.4.7/PKG-INFO
```

### Comparing `fastsnake-1.4.6/.github/workflows/python-package.yml` & `fastsnake-1.4.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/entries.py` & `fastsnake-1.4.7/fastsnake/entries.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.7/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.7/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/application/application.py` & `fastsnake-1.4.7/fastsnake/application/application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from fastsnake.application.arg_parser import main_parser
 from fastsnake.application.config import contest_config_filename
 from fastsnake.application.external import add_external_module, delete_external_module
 from fastsnake.application.contest import start_contest
 from fastsnake.application.runner import run_test, run_test_generator
-from fastsnake.util.codeforces import *
+from fastsnake.util import atcoder
+from fastsnake.util import codeforces
 from fastsnake.util.compiler import compile_code
 
+from typing import List
+
 import fastsnake
 import json
 import os
 
 
 project_path = os.path.join(os.path.dirname(__file__), "..")
 args = main_parser.parse_args()
@@ -31,19 +34,57 @@
     directory = os.path.dirname(filename)
 
     output_filename = os.path.join(directory, "compiled_" + base_name)
     
     compile_code(filename, output_filename)
 
 
-def load_codeforces_problem(contest_id: int, problem: str, directory: str, namespace: str = "contest") -> None:
+def load_atcoder_problem(contest_id: str, problem: str, directory: str, namespace: str) -> None:
+    """
+    Download test cases from AtCoder of a problem.
+    """
+    inputs, outputs = atcoder.get_problem_test_cases(contest_id, problem, namespace)
+
+    if directory != "." and not os.path.exists(directory):
+        os.mkdir(directory)
+
+    for id_ in range(len(inputs)):
+        filename = f"contest_{contest_id}_problem_{problem}_{id_}.in"
+        filename = os.path.join(directory, filename)
+
+        with open(filename, "w") as file:
+            file.write(inputs[id_].strip().strip("\n"))
+            file.flush()
+
+    for id_ in range(len(outputs)):
+        filename = f"contest_{contest_id}_problem_{problem}_{id_}.out"
+        filename = os.path.join(directory, filename)
+
+        with open(filename, "w") as file:
+            file.write(outputs[id_].strip().strip("\n"))
+            file.flush()
+
+
+def load_atcoder_problems(contest_id: str, directory: str, namespace: str) -> List[str]:
+    """
+    Download test cases from every problem of AtCoder contest.
+    """
+    problems = atcoder.get_problems(contest_id, namespace)
+
+    for problem in problems:
+        load_atcoder_problem(contest_id, problem, directory, namespace)
+
+    return problems
+
+
+def load_codeforces_problem(contest_id: int, problem: str, directory: str, namespace: str) -> None:
     """
     Download test cases from Codeforces of a problem.
     """
-    inputs, outputs = get_problem_test_cases(contest_id, problem, namespace)
+    inputs, outputs = codeforces.get_problem_test_cases(contest_id, problem, namespace)
 
     if directory != "." and not os.path.exists(directory):
         os.mkdir(directory)
 
     for id_ in range(len(inputs)):
         filename = f"contest_{contest_id}_problem_{problem}_{id_}.in"
         filename = os.path.join(directory, filename)
@@ -57,40 +98,57 @@
         filename = os.path.join(directory, filename)
 
         with open(filename, "w") as file:
             file.write(outputs[id_].strip().strip("\n"))
             file.flush()
 
 
-def load_codeforces_problems(contest_id: int, directory: str, namespace: str = "contest") -> List[str]:
+def load_codeforces_problems(contest_id: int, directory: str, namespace: str) -> List[str]:
     """
     Download test cases from every problem of Codeforces contest.
     """
-    problems = get_problems(contest_id, namespace)
+    problems = codeforces.get_problems(contest_id, namespace)
 
     for problem in problems:
         load_codeforces_problem(contest_id, problem, directory, namespace)
 
     return problems
 
 
+def start_atcoder_contest(contest_id: str) -> None:
+    """
+    Initialize a AtCoder contest.
+    """
+    directory = "atcoder_contest"
+
+    solutions = os.path.join(directory, "solutions")
+    test_cases = os.path.join(directory, "test_cases")
+    test_generators = os.path.join(directory, "test_generators")
+
+    if not os.path.exists(directory):
+        os.mkdir(directory)
+
+    problems = load_atcoder_problems(contest_id, test_cases, namespace="contests")
+    start_contest(solutions, test_cases, test_generators, contest_id, problems)
+
+
 def start_codeforces_contest(contest_id: int) -> None:
     """
     Initialize a Codeforces contest.
     """
     directory = "codeforces_contest"
 
     solutions = os.path.join(directory, "solutions")
     test_cases = os.path.join(directory, "test_cases")
     test_generators = os.path.join(directory, "test_generators")
 
     if not os.path.exists(directory):
         os.mkdir(directory)
 
-    problems = load_codeforces_problems(contest_id, test_cases)
+    problems = load_codeforces_problems(contest_id, test_cases, namespace="contest")
     start_contest(solutions, test_cases, test_generators, contest_id, problems)
 
 
 def start_codeforces_gym(gym_id: int) -> None:
     """
     Initialize a Codeforces contest.
     """
@@ -189,26 +247,38 @@
         elif args.command == "add-external":
             add_external_module(args.filename, args.name, bool(args.url))
 
         # Delete a external module.
         elif args.command == "delete-external":
             delete_external_module(args.module)
 
+        # Tools for AtCoder.
+        elif args.command == "atcoder":
+            if args.load:
+                contest_id, problem = args.load[0], args.load[1]
+                load_atcoder_problem(contest_id, problem, args.save, namespace="contests")
+
+            elif args.load_all:
+                load_atcoder_problems(args.load_all, args.save, namespace="contests")
+
+            elif args.start_contest:
+                start_atcoder_contest(args.start_contest)
+
         # Tools for Codeforces.
         elif args.command == "codeforces":
             if args.load:
                 try: 
                     contest_id, problem = int(args.load[0]), args.load[1]
                 except: 
                     contest_id, problem = int(args.load[1]), args.load[0]
 
-                load_codeforces_problem(contest_id, problem, args.save)
+                load_codeforces_problem(contest_id, problem, args.save, namespace="contest")
 
             elif args.load_all:
-                load_codeforces_problems(args.load_all, args.save)
+                load_codeforces_problems(args.load_all, args.save, namespace="contest")
 
             elif args.start_contest:
                 start_codeforces_contest(args.start_contest)
 
             elif args.start_gym:
                 start_codeforces_gym(args.start_gym)
```

### Comparing `fastsnake-1.4.6/fastsnake/application/arg_parser.py` & `fastsnake-1.4.7/fastsnake/application/arg_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from argparse import ArgumentParser
 
 
+__all__ = ["main_parser"]
+
+
 main_parser = ArgumentParser(prog="FastSnake", description="CLI Tools for Competitive Programming")
 
 main_parser.add_argument("-l", "--list", type=str, choices=["algorithms", "structures", "external"], help="List algorithm, structure or external modules")
 main_parser.add_argument("-v", "--version", action="store_true", help="Print the fastsnake's version")
 main_parser.add_argument("--author", action="store_true", help="Print the author name")
 main_parser.add_argument("--credits", action="store_true", help="Print the credits of the project")
 
@@ -30,14 +33,21 @@
 add_external_contest_parser.add_argument("-n", "--name", type=str, required=True, dest="name", help="External module name")
 add_external_contest_parser.add_argument("-u", "--url", action="store_true", dest="url", help="Indicates to download the code from the URL")
 
 # Delete External Module.
 delete_external_contest_parser = command_parser.add_parser("delete-external", help="Delete an external module")
 delete_external_contest_parser.add_argument("module", type=str, help="External module name")
 
+# Tools for AtCoder Platforms.
+atcoder_parser = command_parser.add_parser("atcoder", help="Tools for Atcoder platform")
+atcoder_parser.add_argument("--load-all", metavar="contest_id", type=str, dest="load_all", help="Download test cases from every problem of a contest")
+atcoder_parser.add_argument("--load", metavar=("contest_id", "problem"), type=str, nargs=2, dest="load", help="Download test cases from a problem")
+atcoder_parser.add_argument("--save", metavar="directory", type=str, default="atcoder", dest="save", help="Directory for saving downloaded files")
+atcoder_parser.add_argument("-sc", "--start-contest", metavar="contest_id", type=str, dest="start_contest", help="Initialize a Codeforces contest")
+
 # Tools for Contest Platforms.
 codeforces_parser = command_parser.add_parser("codeforces", help="Tools for Codeforces platform")
 codeforces_parser.add_argument("--load-all", metavar="contest_id", type=int, dest="load_all", help="Download test cases from every problem of a contest")
 codeforces_parser.add_argument("--load", metavar=("contest_id", "problem"), type=str, nargs=2, dest="load", help="Download test cases from a problem")
 codeforces_parser.add_argument("--save", metavar="directory", type=str, default="codeforces", dest="save", help="Directory for saving downloaded files")
 codeforces_parser.add_argument("-sc", "--start-contest", metavar="contest_id", type=int, dest="start_contest", help="Initialize a Codeforces contest")
 codeforces_parser.add_argument("-sg", "--start-gym", metavar="gym_id", type=int, dest="start_gym", help="Initialize a Codeforces gym")
```

### Comparing `fastsnake-1.4.6/fastsnake/application/contest.py` & `fastsnake-1.4.7/fastsnake/application/contest.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/application/external.py` & `fastsnake-1.4.7/fastsnake/application/external.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/application/runner.py` & `fastsnake-1.4.7/fastsnake/application/runner.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/structures/b_tree.py` & `fastsnake-1.4.7/fastsnake/structures/b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/fastsnake/util/codeforces.py` & `fastsnake-1.4.7/fastsnake/util/codeforces.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def get_problems(id_: int, namespace: str = "contest") -> List[str]:
     url = f"https://codeforces.com/{namespace}/{id_}"
 
     response = requests.get(url, headers=headers)
 
     if response.status_code >= 300:
-        raise ValueError(f"{namespace.capitalize()} not found")
+        raise ValueError(f"{namespace.capitalize()} not found. Status Code: {response.status_code}")
 
     problems = []
 
     soup = BeautifulSoup(response.content, "html.parser")
 
     table = soup.find("table", class_="problems")
 
@@ -50,15 +50,15 @@
 def get_problem_test_cases(id_: int, problem: str, namespace: str = "contest") -> Tuple[List[str], List[str]]:
     url = f"https://codeforces.com/{namespace}/{id_}/problem/{problem}"
 
     response = requests.get(url, headers=headers)
     inputs, outputs = [], []
 
     if response.status_code >= 300:
-        raise ValueError(f"{namespace.capitalize()} problem not found")
+        raise ValueError(f"{namespace.capitalize()} problem not found. Status Code: {response.status_code}")
     
     soup = BeautifulSoup(response.content, "html.parser")
 
     for input_data in soup.find_all("div", class_="input"):        
         pre = input_data.find("pre")
 
         if not pre: continue
```

### Comparing `fastsnake-1.4.6/fastsnake/util/compiler.py` & `fastsnake-1.4.7/fastsnake/util/compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.7/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.7/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.7/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.7/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.7/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_codeforces_tools/test_problem_loader.py` & `fastsnake-1.4.7/tests/test_codeforces_tools/test_codeforces_problem_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from fastsnake.util.codeforces import *
 import os
 
+
 def test_get_problems():
     problems = get_problems(1949)
     assert "".join(problems) == "ABCDEFGHIJK"
 
 
 def test_load_problem_test_cases():
     folder = os.path.join(os.path.dirname(__file__), "sample_1949_J")
```

### Comparing `fastsnake-1.4.6/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.7/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/tests/test_structures/test_b_tree.py` & `fastsnake-1.4.7/tests/test_structures/test_b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/.gitignore` & `fastsnake-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/LICENSE` & `fastsnake-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/README.md` & `fastsnake-1.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Pypi](https://img.shields.io/pypi/v/FastSnake?logo=pypi)](https://pypi.org/project/FastSnake/)
 [![License](https://img.shields.io/pypi/l/FastSnake)](https://github.com/JeanExtreme002/FastSnake)
 [![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20Linux-8A2BE2)](https://pypi.org/project/FastSnake/)
 [![Python Version](https://img.shields.io/badge/python-3.7+-yellow)](https://pypi.org/project/FastSnake/)
 
 Tired of having to copy-paste your library code into every solution you write? FastSnake is a command-line tool that allows you to easily create, expand, run and test Python solutions for competitive programming problems.
 
-This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces. But you will have to write your own code and library for the problems you want to solve.
+This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces and AtCoder platforms. But you will have to write your own code and library for the problems you want to solve.
 
 ## Installing FastSnake:
 ```
 $ pip install FastSnake
 ```
 
 ## Basic Usage:
```

### Comparing `fastsnake-1.4.6/pyproject.toml` & `fastsnake-1.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.6/PKG-INFO` & `fastsnake-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.4.6
+Version: 1.4.7
 Summary: A Python Helper CLI for Competitive Programming
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,cli,codeforces,competition,competitive programming,contest,helper,marathon,structures
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 [![Pypi](https://img.shields.io/pypi/v/FastSnake?logo=pypi)](https://pypi.org/project/FastSnake/)
 [![License](https://img.shields.io/pypi/l/FastSnake)](https://github.com/JeanExtreme002/FastSnake)
 [![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20Linux-8A2BE2)](https://pypi.org/project/FastSnake/)
 [![Python Version](https://img.shields.io/badge/python-3.7+-yellow)](https://pypi.org/project/FastSnake/)
 
 Tired of having to copy-paste your library code into every solution you write? FastSnake is a command-line tool that allows you to easily create, expand, run and test Python solutions for competitive programming problems.
 
-This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces. But you will have to write your own code and library for the problems you want to solve.
+This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces and AtCoder platforms. But you will have to write your own code and library for the problems you want to solve.
 
 ## Installing FastSnake:
 ```
 $ pip install FastSnake
 ```
 
 ## Basic Usage:
```

