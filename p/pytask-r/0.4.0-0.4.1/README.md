# Comparing `tmp/pytask_r-0.4.0.tar.gz` & `tmp/pytask_r-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytask_r-0.4.0.tar", last modified: Sat Oct  7 23:15:50 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytask_r-0.4.0.tar` & `pytask_r-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.580892 pytask_r-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.572892 pytask_r-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.576892 pytask_r-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.576892 pytask_r-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-07 23:15:39.000000 pytask_r-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-07 23:15:39.000000 pytask_r-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-07 23:15:39.000000 pytask_r-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2023-10-07 23:15:50.580892 pytask_r-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2023-10-07 23:15:39.000000 pytask_r-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-10-07 23:15:39.000000 pytask_r-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-07 23:15:50.580892 pytask_r-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.572892 pytask_r-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.576892 pytask_r-0.4.0/src/pytask_r/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-10-07 23:15:39.000000 pytask_r-0.4.0/src/pytask_r/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 23:15:50.580892 pytask_r-0.4.0/src/pytask_r.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-07 23:15:50.000000 pytask_r-0.4.0/src/pytask_r.egg-info/top_level.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/_version.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/collect.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/config.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/execute.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/py.typed
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/serialization.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pytask_r-0.4.1/src/pytask_r/shared.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytask_r-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytask_r-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 pytask_r-0.4.1/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 pytask_r-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 pytask_r-0.4.1/PKG-INFO
```

### Comparing `pytask_r-0.4.0/LICENSE` & `pytask_r-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytask_r-0.4.0/PKG-INFO` & `pytask_r-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pytask_r
-Version: 0.4.0
+Version: 0.4.1
 Summary: Run R scripts with pytask.
-Home-page: https://github.com/pytask-dev/pytask-r
-Author: Tobias Raabe
-Author-email: raabe@posteo.de
-License: MIT
+Project-URL: Homepage, https://github.com/pytask-dev/pytask-r
 Project-URL: Changelog, https://github.com/pytask-dev/pytask-r/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/pytask-dev/pytask-r
 Project-URL: Github, https://github.com/pytask-dev/pytask-r
 Project-URL: Tracker, https://github.com/pytask-dev/pytask-r/issues
-Platform: any
+Author-email: Tobias Raabe <raabe@posteo.de>
+License: MIT
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: R
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: pluggy>=1.0.0
-Requires-Dist: pytask>=0.4.0
+Requires-Dist: pytask>=0.4.5
+Provides-Extra: test
+Requires-Dist: pytask-parallel; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-xdist; extra == 'test'
+Requires-Dist: pyyaml; extra == 'test'
+Description-Content-Type: text/markdown
 
 # pytask-r
 
 [![PyPI](https://img.shields.io/pypi/v/pytask-r?color=blue)](https://pypi.org/project/pytask-r)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytask-r)](https://pypi.org/project/pytask-r)
 [![image](https://img.shields.io/conda/vn/conda-forge/pytask-r.svg)](https://anaconda.org/conda-forge/pytask-r)
 [![image](https://img.shields.io/conda/pn/conda-forge/pytask-r.svg)](https://anaconda.org/conda-forge/pytask-r)
@@ -53,55 +57,50 @@
 $ conda install -c conda-forge pytask-r
 ```
 
 You also need to have R installed and `Rscript` on your command line. Test it by typing
 the following on the command line
 
 ```console
-$ Rscript --help
+Rscript --help
 ```
 
-If an error is shown instead of a help page, you can install R with `conda` by choosing
-either R or Microsoft R Open (MRO). Choose one of the two following commands. (See
-[here](https://docs.anaconda.com/anaconda/user-guide/tasks/%20using-r-language) for
-further explanation on Anaconda, R, and MRO.)
+If an error is shown instead of a help page, you can install R with `conda`.
 
 ```console
-$ conda install -c r r-base     # For normal R.
-$ conda install -c r mro-base   # For MRO.
+conda install -c conda-forge r-base
 ```
 
 Or install install R from the official [R Project](https://www.r-project.org/).
 
 ## Usage
 
-To create a task which runs a R script, define a task function with the `@pytask.mark.r`
-decorator. The `script` keyword provides an absolute path or path relative to the task
-module to the R script.
+To create a task that runs an R script, define a task function with the `@mark.r`
+decorator. The `script` keyword provides an absolute path or a path relative to the task
+module.
 
 ```python
-import pytask
+from pathlib import Path
+from pytask import mark
 
 
-@pytask.mark.r(script="script.r")
-@pytask.mark.produces("out.rds")
-def task_run_r_script():
+@mark.r(script=Path("script.r"))
+def task_run_r_script(produces: Path = Path("out.rds")):
     pass
 ```
 
 If you are wondering why the function body is empty, know that pytask-r replaces the
 body with a predefined internal function. See the section on implementation details for
 more information.
 
 ### Dependencies and Products
 
-Dependencies and products can be added as with a normal pytask task using the
-`@pytask.mark.depends_on` and `@pytask.mark.produces` decorators. which is explained in
-this
-[tutorial](https://pytask-dev.readthedocs.io/en/stable/tutorials/defining_dependencies_products.html).
+Dependencies and products can be added as usual. See this
+[tutorial](https://pytask-dev.readthedocs.io/en/stable/tutorials/defining_dependencies_products.html)
+for some help.
 
 ### Accessing dependencies and products in the script
 
 To access the paths of dependencies and products in the script, pytask-r stores the
 information by default in a `.json` file. The path to this file is passed as a
 positional argument to the script. Inside the script, you can read the information.
 
@@ -121,46 +120,48 @@
 
 To parse the JSON file, you need to install
 [jsonlite](https://github.com/jeroen/jsonlite).
 
 You can also pass any other information to your script by using the `@task` decorator.
 
 ```python
+from pathlib import Path
+from pytask import mark, task
+
+
 @task(kwargs={"number": 1})
-@pytask.mark.r(script="script.r")
-@pytask.mark.produces("out.rds")
-def task_run_r_script():
+@mark.r(script=Path("script.r"))
+def task_run_r_script(produces: Path = Path("out.rds")):
     pass
 ```
 
 and inside the script use
 
 ```r
 config$number  # Is 1.
 ```
 
 ### Debugging
 
 In case a task throws an error, you might want to execute the script independently from
-pytask. After a failed execution, you see the command which executed the R script in the
+pytask. After a failed execution, you see the command that executed the R script in the
 report of the task. It looks roughly like this
 
 ```console
-$ Rscript <options> script.r <path-to>/.pytask/task_py_task_example.json
+Rscript <options> script.r <path-to>/.pytask/task_py_task_example.json
 ```
 
 ### Command Line Arguments
 
 The decorator can be used to pass command line arguments to `Rscript`. See the following
 example.
 
 ```python
-@pytask.mark.r(script="script.r", options="--vanilla")
-@pytask.mark.produces("out.rds")
-def task_run_r_script():
+@mark.r(script=Path("script.r"), options="--vanilla")
+def task_run_r_script(produces: Path = Path("out.rds")):
     pass
 ```
 
 ### Repeating tasks with different scripts or inputs
 
 You can also repeat the execution of tasks, meaning executing multiple R scripts or
 passing different command line arguments to the same R script.
@@ -168,30 +169,28 @@
 The following task executes two R scripts, `script_1.r` and `script_2.r`, which produce
 different outputs.
 
 ```python
 for i in range(2):
 
     @task
-    @pytask.mark.r(script=f"script_{i}.r")
-    @pytask.mark.produces(f"out_{i}.csv")
-    def task_execute_r_script():
+    @mark.r(script=Path(f"script_{i}.r"))
+    def task_execute_r_script(produces: Path = Path(f"out_{i}.csv")):
         pass
 ```
 
 If you want to pass different inputs to the same R script, pass these arguments with the
 `kwargs` keyword of the `@task` decorator.
 
 ```python
 for i in range(2):
 
     @task(kwargs={"i": i})
-    @pytask.mark.r(script="script.r")
-    @pytask.mark.produces(f"output_{i}.csv")
-    def task_execute_r_script():
+    @mark.r(script=Path("script.r"))
+    def task_execute_r_script(produces: Path = Path(f"output_{i}.csv")):
         pass
 ```
 
 and inside the task access the argument `i` with
 
 ```r
 library(jsonlite)
@@ -211,46 +210,44 @@
 
 You can also serialize your data with any other tool you like. By default, pytask-r also
 supports YAML (if PyYaml is installed).
 
 Use the `serializer` keyword arguments of the `@pytask.mark.r` decorator with
 
 ```python
-@pytask.mark.r(script="script.r", serializer="yaml")
-def task_example():
-    ...
+@mark.r(script=Path("script.r"), serializer="yaml")
+def task_example(): ...
 ```
 
-And in your R script use
+And, in your R script use
 
 ```r
 library(yaml)
 args <- commandArgs(trailingOnly=TRUE)
 config <- read_yaml(args[length(args)])
 ```
 
 Note that the `YAML` package needs to be installed.
 
-If you need a custom serializer, you can also provide any callable to `serializer` which
-transforms data to a string. Use `suffix` to set the correct file ending.
+If you need a custom serializer, you can also provide any callable `serializer` which
+transforms data into a string. Use `suffix` to set the correct file ending.
 
 Here is a replication of the JSON example.
 
 ```python
 import json
 
 
-@pytask.mark.r(script="script.r", serializer=json.dumps, suffix=".json")
-def task_example():
-    ...
+@mark.r(script=Path("script.r"), serializer=json.dumps, suffix=".json")
+def task_example(): ...
 ```
 
 ### Configuration
 
-You can influence the default behavior of pytask-r with some configuration values.
+You can influence the default behavior of pytask-r with configuration values.
 
 **`r_serializer`**
 
 Use this option to change the default serializer.
 
 ```toml
 [tool.pytask.ini_options]
```

### Comparing `pytask_r-0.4.0/README.md` & `pytask_r-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,55 +27,50 @@
 $ conda install -c conda-forge pytask-r
 ```
 
 You also need to have R installed and `Rscript` on your command line. Test it by typing
 the following on the command line
 
 ```console
-$ Rscript --help
+Rscript --help
 ```
 
-If an error is shown instead of a help page, you can install R with `conda` by choosing
-either R or Microsoft R Open (MRO). Choose one of the two following commands. (See
-[here](https://docs.anaconda.com/anaconda/user-guide/tasks/%20using-r-language) for
-further explanation on Anaconda, R, and MRO.)
+If an error is shown instead of a help page, you can install R with `conda`.
 
 ```console
-$ conda install -c r r-base     # For normal R.
-$ conda install -c r mro-base   # For MRO.
+conda install -c conda-forge r-base
 ```
 
 Or install install R from the official [R Project](https://www.r-project.org/).
 
 ## Usage
 
-To create a task which runs a R script, define a task function with the `@pytask.mark.r`
-decorator. The `script` keyword provides an absolute path or path relative to the task
-module to the R script.
+To create a task that runs an R script, define a task function with the `@mark.r`
+decorator. The `script` keyword provides an absolute path or a path relative to the task
+module.
 
 ```python
-import pytask
+from pathlib import Path
+from pytask import mark
 
 
-@pytask.mark.r(script="script.r")
-@pytask.mark.produces("out.rds")
-def task_run_r_script():
+@mark.r(script=Path("script.r"))
+def task_run_r_script(produces: Path = Path("out.rds")):
     pass
 ```
 
 If you are wondering why the function body is empty, know that pytask-r replaces the
 body with a predefined internal function. See the section on implementation details for
 more information.
 
 ### Dependencies and Products
 
-Dependencies and products can be added as with a normal pytask task using the
-`@pytask.mark.depends_on` and `@pytask.mark.produces` decorators. which is explained in
-this
-[tutorial](https://pytask-dev.readthedocs.io/en/stable/tutorials/defining_dependencies_products.html).
+Dependencies and products can be added as usual. See this
+[tutorial](https://pytask-dev.readthedocs.io/en/stable/tutorials/defining_dependencies_products.html)
+for some help.
 
 ### Accessing dependencies and products in the script
 
 To access the paths of dependencies and products in the script, pytask-r stores the
 information by default in a `.json` file. The path to this file is passed as a
 positional argument to the script. Inside the script, you can read the information.
 
@@ -95,46 +90,48 @@
 
 To parse the JSON file, you need to install
 [jsonlite](https://github.com/jeroen/jsonlite).
 
 You can also pass any other information to your script by using the `@task` decorator.
 
 ```python
+from pathlib import Path
+from pytask import mark, task
+
+
 @task(kwargs={"number": 1})
-@pytask.mark.r(script="script.r")
-@pytask.mark.produces("out.rds")
-def task_run_r_script():
+@mark.r(script=Path("script.r"))
+def task_run_r_script(produces: Path = Path("out.rds")):
     pass
 ```
 
 and inside the script use
 
 ```r
 config$number  # Is 1.
 ```
 
 ### Debugging
 
 In case a task throws an error, you might want to execute the script independently from
-pytask. After a failed execution, you see the command which executed the R script in the
+pytask. After a failed execution, you see the command that executed the R script in the
 report of the task. It looks roughly like this
 
 ```console
-$ Rscript <options> script.r <path-to>/.pytask/task_py_task_example.json
+Rscript <options> script.r <path-to>/.pytask/task_py_task_example.json
 ```
 
 ### Command Line Arguments
 
 The decorator can be used to pass command line arguments to `Rscript`. See the following
 example.
 
 ```python
-@pytask.mark.r(script="script.r", options="--vanilla")
-@pytask.mark.produces("out.rds")
-def task_run_r_script():
+@mark.r(script=Path("script.r"), options="--vanilla")
+def task_run_r_script(produces: Path = Path("out.rds")):
     pass
 ```
 
 ### Repeating tasks with different scripts or inputs
 
 You can also repeat the execution of tasks, meaning executing multiple R scripts or
 passing different command line arguments to the same R script.
@@ -142,30 +139,28 @@
 The following task executes two R scripts, `script_1.r` and `script_2.r`, which produce
 different outputs.
 
 ```python
 for i in range(2):
 
     @task
-    @pytask.mark.r(script=f"script_{i}.r")
-    @pytask.mark.produces(f"out_{i}.csv")
-    def task_execute_r_script():
+    @mark.r(script=Path(f"script_{i}.r"))
+    def task_execute_r_script(produces: Path = Path(f"out_{i}.csv")):
         pass
 ```
 
 If you want to pass different inputs to the same R script, pass these arguments with the
 `kwargs` keyword of the `@task` decorator.
 
 ```python
 for i in range(2):
 
     @task(kwargs={"i": i})
-    @pytask.mark.r(script="script.r")
-    @pytask.mark.produces(f"output_{i}.csv")
-    def task_execute_r_script():
+    @mark.r(script=Path("script.r"))
+    def task_execute_r_script(produces: Path = Path(f"output_{i}.csv")):
         pass
 ```
 
 and inside the task access the argument `i` with
 
 ```r
 library(jsonlite)
@@ -185,46 +180,44 @@
 
 You can also serialize your data with any other tool you like. By default, pytask-r also
 supports YAML (if PyYaml is installed).
 
 Use the `serializer` keyword arguments of the `@pytask.mark.r` decorator with
 
 ```python
-@pytask.mark.r(script="script.r", serializer="yaml")
-def task_example():
-    ...
+@mark.r(script=Path("script.r"), serializer="yaml")
+def task_example(): ...
 ```
 
-And in your R script use
+And, in your R script use
 
 ```r
 library(yaml)
 args <- commandArgs(trailingOnly=TRUE)
 config <- read_yaml(args[length(args)])
 ```
 
 Note that the `YAML` package needs to be installed.
 
-If you need a custom serializer, you can also provide any callable to `serializer` which
-transforms data to a string. Use `suffix` to set the correct file ending.
+If you need a custom serializer, you can also provide any callable `serializer` which
+transforms data into a string. Use `suffix` to set the correct file ending.
 
 Here is a replication of the JSON example.
 
 ```python
 import json
 
 
-@pytask.mark.r(script="script.r", serializer=json.dumps, suffix=".json")
-def task_example():
-    ...
+@mark.r(script=Path("script.r"), serializer=json.dumps, suffix=".json")
+def task_example(): ...
 ```
 
 ### Configuration
 
-You can influence the default behavior of pytask-r with some configuration values.
+You can influence the default behavior of pytask-r with configuration values.
 
 **`r_serializer`**
 
 Use this option to change the default serializer.
 
 ```toml
 [tool.pytask.ini_options]
```

### Comparing `pytask_r-0.4.0/src/pytask_r/collect.py` & `pytask_r-0.4.1/src/pytask_r/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 """Collect tasks."""
+
 from __future__ import annotations
 
 import subprocess
 import warnings
 from pathlib import Path
 from typing import Any
 
-from pytask import has_mark
-from pytask import hookimpl
-from pytask import is_task_function
 from pytask import Mark
 from pytask import NodeInfo
-from pytask import parse_dependencies_from_task_function
-from pytask import parse_products_from_task_function
 from pytask import PathNode
 from pytask import PTask
 from pytask import PythonNode
-from pytask import remove_marks
 from pytask import Session
 from pytask import Task
 from pytask import TaskWithoutPath
-from pytask_r.serialization import create_path_to_serialized
+from pytask import has_mark
+from pytask import hookimpl
+from pytask import is_task_function
+from pytask import parse_dependencies_from_task_function
+from pytask import parse_products_from_task_function
+from pytask import remove_marks
+
 from pytask_r.serialization import SERIALIZERS
+from pytask_r.serialization import create_path_to_serialized
 from pytask_r.shared import r
 
 
 def run_r_script(
-    _script: Path, _options: list[str], _serialized: Path, **kwargs: Any  # noqa: ARG001
+    _script: Path,
+    _options: list[str],
+    _serialized: Path,
+    **kwargs: Any,  # noqa: ARG001
 ) -> None:
     """Run an R script."""
     cmd = ["Rscript", _script.as_posix(), *_options, str(_serialized)]
     print("Executing " + " ".join(cmd) + ".")  # noqa: T201
     subprocess.run(cmd, check=True)  # noqa: S603
 
 
@@ -45,30 +50,31 @@
         (name.startswith("task_") or has_mark(obj, "task"))
         and is_task_function(obj)
         and has_mark(obj, "r")
     ):
         # Parse @pytask.mark.r decorator.
         obj, marks = remove_marks(obj, "r")
         if len(marks) > 1:
-            raise ValueError(
+            msg = (
                 f"Task {name!r} has multiple @pytask.mark.r marks, but only one is "
                 "allowed."
             )
+            raise ValueError(msg)
 
         mark = _parse_r_mark(
             mark=marks[0],
             default_options=session.config["r_options"],
             default_serializer=session.config["r_serializer"],
             default_suffix=session.config["r_suffix"],
         )
-        script, options, _, suffix = r(**marks[0].kwargs)
+        script, options, _, suffix = r(**mark.kwargs)
 
         obj.pytask_meta.markers.append(mark)
 
-        # Collect the nodes in @pytask.mark.julia and validate them.
+        # Collect the nodes in @pytask.mark.r and validate them.
         path_nodes = Path.cwd() if path is None else path.parent
 
         if isinstance(script, str):
             warnings.warn(
                 "Passing a string to the @pytask.mark.r parameter 'script' is "
                 "deprecated. Please, use a pathlib.Path instead.",
                 stacklevel=1,
@@ -83,19 +89,23 @@
                 path=(),
                 value=script,
                 task_path=path,
                 task_name=name,
             ),
         )
 
-        if not (isinstance(script_node, PathNode) and script_node.path.suffix == ".r"):
-            raise ValueError(
+        if not (
+            isinstance(script_node, PathNode)
+            and script_node.path.suffix in (".r", ".R")
+        ):
+            msg = (
                 "The 'script' keyword of the @pytask.mark.r decorator must point "
-                f"to Julia file with the .r suffix, but it is {script_node}."
+                f"to an R file with the .r or .R extension, but it is {script_node}."
             )
+            raise ValueError(msg)
 
         options_node = session.hook.pytask_collect_node(
             session=session,
             path=path_nodes,
             node_info=NodeInfo(
                 arg_name="_options",
                 path=(),
@@ -158,15 +168,15 @@
 
 def _parse_r_mark(
     mark: Mark,
     default_options: list[str] | None,
     default_serializer: str,
     default_suffix: str,
 ) -> Mark:
-    """Parse a Julia mark."""
+    """Parse an R mark."""
     script, options, serializer, suffix = r(**mark.kwargs)
 
     parsed_kwargs = {}
     for arg_name, value, default in (
         ("script", script, None),
         ("options", options, default_options),
         ("serializer", serializer, default_serializer),
@@ -177,9 +187,8 @@
         SERIALIZERS[parsed_kwargs["serializer"]]["suffix"]
         if isinstance(parsed_kwargs["serializer"], str)
         and parsed_kwargs["serializer"] in SERIALIZERS
         else default_suffix
     )
     parsed_kwargs["suffix"] = suffix or proposed_suffix  # type: ignore[assignment]
 
-    mark = Mark("r", (), parsed_kwargs)
-    return mark
+    return Mark("r", (), parsed_kwargs)
```

### Comparing `pytask_r-0.4.0/src/pytask_r/config.py` & `pytask_r-0.4.1/src/pytask_r/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Configure pytask."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from pytask import hookimpl
+
 from pytask_r.serialization import SERIALIZERS
 
 
 @hookimpl
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Register the r marker."""
     config["markers"]["r"] = "Tasks which are executed with Rscript."
     config["r_serializer"] = config.get("r_serializer", "json")
     if config["r_serializer"] not in SERIALIZERS:
-        raise ValueError(
+        msg = (
             f"'r_serializer' is {config['r_serializer']} and not one of "
             f"{list(SERIALIZERS)}."
         )
-    config["r_suffix"] = config.get("r_suffix", "")
+        raise ValueError(msg)
+    config["r_suffix"] = config.get("r_suffix", ".json")
     config["r_options"] = _parse_value_or_whitespace_option(config.get("r_options"))
 
 
 def _parse_value_or_whitespace_option(value: Any) -> list[str] | None:
     """Parse option which can hold a single value or values separated by new lines."""
     if value is None:
         return None
     if isinstance(value, list):
         return list(map(str, value))
-    raise ValueError(f"'r_options' is {value} and not a list.")
+    msg = f"'r_options' is {value} and not a list."
+    raise ValueError(msg)
```

### Comparing `pytask_r-0.4.0/src/pytask_r/execute.py` & `pytask_r-0.4.1/src/pytask_r/execute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 """Execute tasks."""
+
 from __future__ import annotations
 
 import shutil
 from typing import Any
 
-from pytask import get_marks
-from pytask import hookimpl
 from pytask import PPathNode
 from pytask import PTask
 from pytask import PythonNode
+from pytask import get_marks
+from pytask import hookimpl
 from pytask.tree_util import tree_map
+
 from pytask_r.serialization import serialize_keyword_arguments
 from pytask_r.shared import r
 
 
 @hookimpl
 def pytask_execute_task_setup(task: PTask) -> None:
     """Perform some checks when a task marked with the r marker is executed."""
     marks = get_marks(task, "r")
     if marks:
         if shutil.which("Rscript") is None:
-            raise RuntimeError(
+            msg = (
                 "Rscript is needed to run R scripts, but it is not found on your PATH."
             )
+            raise RuntimeError(msg)
 
-        assert len(marks) == 1
+        if len(marks) > 1:
+            msg = "Only one R marker is allowed per task."
+            raise ValueError(msg)
 
-        _, _, serializer, suffix = r(**marks[0].kwargs)
-        assert serializer
-        assert suffix
+        _, _, serializer, _ = r(**marks[0].kwargs)
 
         serialized_node: PythonNode = task.depends_on["_serialized"]  # type: ignore[assignment]
-        serialized_node.value.parent.mkdir(parents=True, exist_ok=True)
+        serialized_node.value.parent.mkdir(parents=True, exist_ok=True)  # type: ignore[union-attr]
         kwargs = collect_keyword_arguments(task)
-        serialize_keyword_arguments(serializer, serialized_node.value, kwargs)
+        serialize_keyword_arguments(serializer, serialized_node.value, kwargs)  # type: ignore[arg-type]
 
 
 def collect_keyword_arguments(task: PTask) -> dict[str, Any]:
     """Collect keyword arguments for function."""
     # Remove all kwargs from the task so that they are not passed to the function.
     kwargs: dict[str, Any] = {
         **tree_map(  # type: ignore[dict-item]
-            lambda x: str(x.path) if isinstance(x, PPathNode) else str(x.value),
+            lambda x: str(x.path) if isinstance(x, PPathNode) else x.value,
             task.depends_on,
         ),
         **tree_map(  # type: ignore[dict-item]
-            lambda x: str(x.path) if isinstance(x, PPathNode) else str(x.value),
+            lambda x: str(x.path) if isinstance(x, PPathNode) else x.value,
             task.produces,
         ),
     }
     kwargs.pop("_script")
     kwargs.pop("_options")
     kwargs.pop("_serialized")
     return kwargs
```

### Comparing `pytask_r-0.4.0/src/pytask_r/serialization.py` & `pytask_r-0.4.1/src/pytask_r/serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""This module contains the code to serialize keyword arguments to the task."""
+"""Contains the code to serialize keyword arguments to the task."""
+
 from __future__ import annotations
 
 import json
 from pathlib import Path
 from typing import Any
 from typing import Callable
 
 from pytask import PTask
 from pytask import PTaskWithPath
 
-
 _HIDDEN_FOLDER = ".pytask/pytask-r"
 
 
 SERIALIZERS = {"json": {"serializer": json.dumps, "suffix": ".json"}}
 
 
 try:
@@ -25,16 +25,15 @@
     SERIALIZERS["yml"] = {"serializer": yaml.dump, "suffix": ".yml"}
 
 
 def create_path_to_serialized(task: PTask, suffix: str) -> Path:
     """Create path to serialized."""
     parent = task.path.parent if isinstance(task, PTaskWithPath) else Path.cwd()
     file_name = create_file_name(task, suffix)
-    path = parent.joinpath(_HIDDEN_FOLDER, file_name).with_suffix(suffix)
-    return path
+    return parent.joinpath(_HIDDEN_FOLDER, file_name).with_suffix(suffix)
 
 
 def create_file_name(task: PTask, suffix: str) -> str:
     """Create the file name of the file containing the serialized kwargs.
 
     Some characters need to be escaped since they are not valid characters on file
     systems.
@@ -55,15 +54,14 @@
     path_to_serialized: Path,
     kwargs: dict[str, Any],
 ) -> None:
     """Serialize keyword arguments."""
     if callable(serializer):
         serializer_func = serializer
     elif isinstance(serializer, str) and serializer in SERIALIZERS:
-        serializer_func = SERIALIZERS[serializer][
-            "serializer"
-        ]  # type: ignore[assignment]
+        serializer_func = SERIALIZERS[serializer]["serializer"]  # type: ignore[assignment]
     else:
-        raise ValueError(f"Serializer {serializer!r} is not known.")
+        msg = f"Serializer {serializer!r} is not known."
+        raise ValueError(msg)
 
     serialized = serializer_func(kwargs)
     path_to_serialized.write_text(serialized)
```

### Comparing `pytask_r-0.4.0/src/pytask_r/shared.py` & `pytask_r-0.4.1/src/pytask_r/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-"""This module contains shared functions."""
+"""Contains shared functions."""
+
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Sequence
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def r(
     *,
     script: str | Path,
     options: str | Iterable[str] | None = None,
     serializer: str | Callable[..., str] | None = None,
     suffix: str | None = None,
```

