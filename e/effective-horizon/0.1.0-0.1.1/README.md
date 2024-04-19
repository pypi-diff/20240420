# Comparing `tmp/effective_horizon-0.1.0.tar.gz` & `tmp/effective_horizon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effective_horizon-0.1.0.tar", last modified: Fri Apr 19 22:28:03 2024, max compression
+gzip compressed data, was "effective_horizon-0.1.1.tar", last modified: Fri Apr 19 22:38:32 2024, max compression
```

## Comparing `effective_horizon-0.1.0.tar` & `effective_horizon-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:28:03.329425 effective_horizon-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-04-19 22:28:03.329425 effective_horizon-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:28:03.329425 effective_horizon-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:28:03.325425 effective_horizon-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:28:03.325425 effective_horizon-0.1.0/src/effective_horizon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-04-19 22:28:03.000000 effective_horizon-0.1.0/src/effective_horizon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 22:28:03.000000 effective_horizon-0.1.0/src/effective_horizon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:28:03.000000 effective_horizon-0.1.0/src/effective_horizon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 22:28:03.000000 effective_horizon-0.1.0/src/effective_horizon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 22:28:03.000000 effective_horizon-0.1.0/src/effective_horizon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:28:03.325425 effective_horizon-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/tests/test_deterministic_mdps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/tests/test_julia_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/tests/test_python_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/tests/test_training_rllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-19 22:27:59.000000 effective_horizon-0.1.0/tests/test_training_sb3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.589020 effective_horizon-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-04-19 22:38:32.589020 effective_horizon-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.581020 effective_horizon-0.1.1/effective_horizon/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/atari_head.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.585020 effective_horizon-0.1.1/effective_horizon/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/atari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/deterministic_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/procgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/envs/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/impala_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/mdp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/os_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.585020 effective_horizon-0.1.1/effective_horizon/rllib/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.585020 effective_horizon-0.1.1/effective_horizon/rllib/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/algorithms/bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/algorithms/dqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/algorithms/gorp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/algorithms/replay_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14625 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/train_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/rllib/training_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.585020 effective_horizon-0.1.1/effective_horizon/sb3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/sb3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.585020 effective_horizon-0.1.1/effective_horizon/sb3/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/sb3/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/sb3/algorithms/gorp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46070 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/sb3/algorithms/sqirl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/sb3/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/sb3/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.589020 effective_horizon-0.1.1/effective_horizon/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/scripts/construct_tabular_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/scripts/convert_atari_head_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/scripts/convert_atari_mdp_to_framestack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/effective_horizon/scripts/filter_to_minimal_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.589020 effective_horizon-0.1.1/effective_horizon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-04-19 22:38:32.000000 effective_horizon-0.1.1/effective_horizon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-19 22:38:32.000000 effective_horizon-0.1.1/effective_horizon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:38:32.000000 effective_horizon-0.1.1/effective_horizon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 22:38:32.000000 effective_horizon-0.1.1/effective_horizon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 22:38:32.000000 effective_horizon-0.1.1/effective_horizon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:38:32.589020 effective_horizon-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:38:32.589020 effective_horizon-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/tests/test_deterministic_mdps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/tests/test_julia_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/tests/test_python_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/tests/test_training_rllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-19 22:38:28.000000 effective_horizon-0.1.1/tests/test_training_sb3.py
```

### Comparing `effective_horizon-0.1.0/PKG-INFO` & `effective_horizon-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effective-horizon
-Version: 0.1.0
+Version: 0.1.1
 Summary: Code for the NeurIPS 2023 paper "Bridging RL Theory and Practice with the Effective horizon" and the ICLR 2024 paper "The Effective Horizon Explains Deep RL Performance in Stochastic Environments".
 Author-email: Cassidy Laidlaw <cassidy_laidlaw@berkeley.edu>
 Project-URL: Homepage, https://github.com/cassidylaidlaw/effective-horizon
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `effective_horizon-0.1.0/README.md` & `effective_horizon-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `effective_horizon-0.1.0/pyproject.toml` & `effective_horizon-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "effective-horizon"
-version = "0.1.0"
+version = "0.1.1"
 description = 'Code for the NeurIPS 2023 paper "Bridging RL Theory and Practice with the Effective horizon" and the ICLR 2024 paper "The Effective Horizon Explains Deep RL Performance in Stochastic Environments".'
 authors = [
     {name = "Cassidy Laidlaw", email = "cassidy_laidlaw@berkeley.edu"},
 ]
 dynamic = ["readme"]
 dependencies = [
     "sacred>=0.8.2",
@@ -39,14 +39,25 @@
 
 [project.urls]
 Homepage = "https://github.com/cassidylaidlaw/effective-horizon"
 
 [tool.setuptools.dynamic]
 readme = {file=["README.md"], content-type="text/markdown"}
 
+[tool.setuptools]
+packages = [
+    "effective_horizon",
+    "effective_horizon.envs",
+    "effective_horizon.scripts",
+    "effective_horizon.sb3",
+    "effective_horizon.sb3.algorithms",
+    "effective_horizon.rllib",
+    "effective_horizon.rllib.algorithms",
+]
+
 [project.optional-dependencies]
 dev = [
     "black",
     "flake8",
     "pep8-naming",
     "mypy",
     "pytest",
```

### Comparing `effective_horizon-0.1.0/src/effective_horizon.egg-info/PKG-INFO` & `effective_horizon-0.1.1/effective_horizon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effective-horizon
-Version: 0.1.0
+Version: 0.1.1
 Summary: Code for the NeurIPS 2023 paper "Bridging RL Theory and Practice with the Effective horizon" and the ICLR 2024 paper "The Effective Horizon Explains Deep RL Performance in Stochastic Environments".
 Author-email: Cassidy Laidlaw <cassidy_laidlaw@berkeley.edu>
 Project-URL: Homepage, https://github.com/cassidylaidlaw/effective-horizon
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `effective_horizon-0.1.0/tests/test_deterministic_mdps.py` & `effective_horizon-0.1.1/tests/test_deterministic_mdps.py`

 * *Files identical despite different names*

### Comparing `effective_horizon-0.1.0/tests/test_julia_scripts.py` & `effective_horizon-0.1.1/tests/test_julia_scripts.py`

 * *Files identical despite different names*

### Comparing `effective_horizon-0.1.0/tests/test_python_scripts.py` & `effective_horizon-0.1.1/tests/test_python_scripts.py`

 * *Files identical despite different names*

### Comparing `effective_horizon-0.1.0/tests/test_training_rllib.py` & `effective_horizon-0.1.1/tests/test_training_rllib.py`

 * *Files identical despite different names*

### Comparing `effective_horizon-0.1.0/tests/test_training_sb3.py` & `effective_horizon-0.1.1/tests/test_training_sb3.py`

 * *Files identical despite different names*

