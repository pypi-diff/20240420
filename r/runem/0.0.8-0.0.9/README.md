# Comparing `tmp/runem-0.0.8.tar.gz` & `tmp/runem-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runem-0.0.8.tar", last modified: Tue Nov 28 18:14:56 2023, max compression
+gzip compressed data, was "runem-0.0.9.tar", last modified: Wed Nov 29 07:37:13 2023, max compression
```

## Comparing `runem-0.0.8.tar` & `runem-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:56.175856 runem-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-28 18:14:46.000000 runem-0.0.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2023-11-28 18:14:46.000000 runem-0.0.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-11-28 18:14:46.000000 runem-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-28 18:14:46.000000 runem-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2023-11-28 18:14:56.175856 runem-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13651 2023-11-28 18:14:46.000000 runem-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:56.171856 runem-0.0.8/runem/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-28 18:14:46.000000 runem-0.0.8/runem/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:46.000000 runem-0.0.8/runem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-11-28 18:14:46.000000 runem-0.0.8/runem/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-28 18:14:46.000000 runem-0.0.8/runem/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-28 18:14:46.000000 runem-0.0.8/runem/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:46.000000 runem-0.0.8/runem/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-11-28 18:14:46.000000 runem-0.0.8/runem/run_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34589 2023-11-28 18:14:46.000000 runem-0.0.8/runem/runem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:56.175856 runem-0.0.8/runem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2023-11-28 18:14:56.000000 runem-0.0.8/runem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-28 18:14:56.000000 runem-0.0.8/runem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:14:56.000000 runem-0.0.8/runem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-28 18:14:56.000000 runem-0.0.8/runem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-28 18:14:56.000000 runem-0.0.8/runem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-28 18:14:56.000000 runem-0.0.8/runem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:56.171856 runem-0.0.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:46.000000 runem-0.0.8/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 18:14:56.175856 runem-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-11-28 18:14:46.000000 runem-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:56.175856 runem-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:14:46.000000 runem-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-11-28 18:14:46.000000 runem-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-28 18:14:46.000000 runem-0.0.8/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:13.090159 runem-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-29 07:37:01.000000 runem-0.0.9/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2023-11-29 07:37:01.000000 runem-0.0.9/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-11-29 07:37:01.000000 runem-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-29 07:37:01.000000 runem-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2023-11-29 07:37:13.090159 runem-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2023-11-29 07:37:01.000000 runem-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:13.086159 runem-0.0.9/runem/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-29 07:37:01.000000 runem-0.0.9/runem/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:01.000000 runem-0.0.9/runem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2023-11-29 07:37:01.000000 runem-0.0.9/runem/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-29 07:37:01.000000 runem-0.0.9/runem/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-29 07:37:01.000000 runem-0.0.9/runem/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:01.000000 runem-0.0.9/runem/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-11-29 07:37:01.000000 runem-0.0.9/runem/run_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34784 2023-11-29 07:37:01.000000 runem-0.0.9/runem/runem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:13.086159 runem-0.0.9/runem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2023-11-29 07:37:13.000000 runem-0.0.9/runem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-29 07:37:13.000000 runem-0.0.9/runem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 07:37:13.000000 runem-0.0.9/runem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-29 07:37:13.000000 runem-0.0.9/runem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-29 07:37:13.000000 runem-0.0.9/runem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-29 07:37:13.000000 runem-0.0.9/runem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:13.086159 runem-0.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:01.000000 runem-0.0.9/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 07:37:13.090159 runem-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-11-29 07:37:01.000000 runem-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:13.086159 runem-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 07:37:01.000000 runem-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2023-11-29 07:37:01.000000 runem-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-29 07:37:01.000000 runem-0.0.9/tests/test_base.py
```

### Comparing `runem-0.0.8/HISTORY.md` & `runem-0.0.9/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Merge branch 'fix/remove_lursight_env_refs' [Frank Harrison]
+- Fix(lursight-envs): removes lursight envs from runem. [Frank Harrison]
+
+
+0.0.8 (2023-11-28)
+------------------
+- Release: version 0.0.8 🚀 [Frank Harrison]
 - Merge branch 'chore/add_spell_check' [Frank Harrison]
 - Chore(spell-check): disallows adolescent word. [Frank Harrison]
 - Chore(spell-check): adds spell-check job for runem. [Frank Harrison]
 - Merge branch 'chore/minor_improvement_of_log_output_and_report' [Frank
   Harrison]
 - Chore(report): puts the runem times first in the report and indents.
   [Frank Harrison]
```

### Comparing `runem-0.0.8/LICENSE` & `runem-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `runem-0.0.8/PKG-INFO` & `runem-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runem
-Version: 0.0.8
+Version: 0.0.9
 Summary: Awesome runem created by lursight
 Home-page: https://github.com/lursight/runem/
 Author: lursight
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
 Requires-Dist: black==23.11.0; extra == "test"
```

### Comparing `runem-0.0.8/README.md` & `runem-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `runem-0.0.8/runem/run_command.py` & `runem-0.0.9/runem/run_command.py`

 * *Files identical despite different names*

### Comparing `runem-0.0.8/runem/runem.py` & `runem-0.0.9/runem/runem.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,22 +149,24 @@
     jobs: PhaseGroupedJobs  # the jobs to be run ordered by phase
     job_names: JobNames  # the set of job-names
     job_phases: JobPhases  # the set of job-phases (should be subset of 'phases')
     job_tags: JobTags  # the set of job-tags (used for filtering)
 
     def __init__(
         self,
+        cfg_filepath: pathlib.Path,
         phases: OrderedPhases,
         options: OptionConfigs,
         file_filters: TagFileFilters,
         jobs: PhaseGroupedJobs,
         job_names: JobNames,
         job_phases: JobPhases,
         job_tags: JobTags,
     ) -> None:
+        self.cfg_filepath = cfg_filepath
         self.phases = phases
         self.options = options
         self.file_filters = file_filters
         self.jobs = jobs
         self.job_names = job_names
         self.job_phases = job_phases
         self.job_tags = job_tags
@@ -341,20 +343,22 @@
             "the number of concurrent test jobs to run, -1 runs all test jobs at the same time "
             f"({os.cpu_count()} cores available)"
         ),
         required=False,
         type=int,
     )
 
+    config_dir: pathlib.Path = config_metadata.cfg_filepath.parent
     parser.add_argument(
         "--root",
         dest="root_dir",
-        default=os.environ["LANG_CHECKOUT"],
+        default=config_dir,
         help=(
-            "which dir to use as the base-dir for testing, " "defaults to checkout root"
+            "which dir to use as the base-dir for testing, "
+            f"defaults to directory containing the config '{config_dir}'"
         ),
         required=False,
     )
 
     parser.add_argument(
         "--verbose",
         "-v",
@@ -910,14 +914,15 @@
 
     if not phase_order:
         print("WARNING: phase ordering not configured! Runs will be non-deterministic!")
         phase_order = tuple(job_phases)
 
     # tags = tags.union(("python", "es", "firebase_funcs"))
     return ConfigMetadata(
+        cfg_filepath,
         phase_order,
         options,
         file_filters,
         jobs_by_phase,
         job_names,
         job_phases,
         tags,
```

### Comparing `runem-0.0.8/runem.egg-info/PKG-INFO` & `runem-0.0.9/runem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runem
-Version: 0.0.8
+Version: 0.0.9
 Summary: Awesome runem created by lursight
 Home-page: https://github.com/lursight/runem/
 Author: lursight
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
 Requires-Dist: black==23.11.0; extra == "test"
```

### Comparing `runem-0.0.8/setup.py` & `runem-0.0.9/setup.py`

 * *Files identical despite different names*

