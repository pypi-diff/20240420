# Comparing `tmp/pympipool-0.7.9.tar.gz` & `tmp/pympipool-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.7.9.tar", last modified: Mon Nov 27 14:37:12 2023, max compression
+gzip compressed data, was "pympipool-0.8.0.tar", last modified: Sat Apr 20 20:53:30 2024, max compression
```

## Comparing `pympipool-0.7.9.tar` & `pympipool-0.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.556038 pympipool-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-27 14:36:07.000000 pympipool-0.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 14:36:07.000000 pympipool-0.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-11-27 14:37:12.556038 pympipool-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2023-11-27 14:36:07.000000 pympipool-0.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.548038 pympipool-0.7.9/pympipool/
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 14:37:12.556038 pympipool-0.7.9/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/backend/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/backend/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/flux/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/flux/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/mpi/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/executorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shell/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shell/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/slurm/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.548038 pympipool-0.7.9/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-27 14:37:11.000000 pympipool-0.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:37:12.556038 pympipool-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 14:36:07.000000 pympipool-0.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.556038 pympipool-0.7.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_shell_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_subprocess_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_with_dynamic_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.993081 pympipool-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-20 20:52:45.000000 pympipool-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 20:52:45.000000 pympipool-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-04-20 20:53:30.993081 pympipool-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-20 20:52:45.000000 pympipool-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.989081 pympipool-0.8.0/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-20 20:53:30.993081 pympipool-0.8.0/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.989081 pympipool-0.8.0/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/backend/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/backend/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.989081 pympipool-0.8.0/pympipool/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/flux/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.989081 pympipool-0.8.0/pympipool/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/mpi/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.993081 pympipool-0.8.0/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15814 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/inputcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.993081 pympipool-0.8.0/pympipool/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shell/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/shell/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.993081 pympipool-0.8.0/pympipool/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-20 20:52:45.000000 pympipool-0.8.0/pympipool/slurm/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.993081 pympipool-0.8.0/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-04-20 20:53:30.000000 pympipool-0.8.0/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-20 20:53:30.000000 pympipool-0.8.0/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:53:30.000000 pympipool-0.8.0/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-20 20:53:30.000000 pympipool-0.8.0/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 20:53:30.000000 pympipool-0.8.0/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-20 20:53:28.000000 pympipool-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:53:30.993081 pympipool-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-20 20:52:45.000000 pympipool-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:30.993081 pympipool-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_backend_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_executor_backend_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_executor_backend_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_executor_backend_mpi_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_flux_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_integration_pyiron_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_mpi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_mpi_executor_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_shared_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_shared_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_shared_executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_shared_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-20 20:52:45.000000 pympipool-0.8.0/tests/test_shell_interactive.py
```

### Comparing `pympipool-0.7.9/LICENSE` & `pympipool-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.9/PKG-INFO` & `pympipool-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.7.9
+Version: 0.8.0
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
         
@@ -38,131 +38,100 @@
 Project-URL: Repository, https://github.com/pyiron/pympipool
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
-Requires-Dist: mpi4py<=3.1.5,>=3.1.4
-Requires-Dist: pyzmq<=25.1.1,>=25.0.0
-Requires-Dist: tqdm<=4.66.1,>=4.44.0
+Requires-Dist: mpi4py<=3.1.6,>=3.1.4
+Requires-Dist: pyzmq<=26.0.2,>=25.0.0
+Requires-Dist: tqdm<=4.66.2,>=4.44.0
 
 # pympipool - up-scale python functions for high performance computing
 [![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pympipool/HEAD?labpath=notebooks%2Fexamples.ipynb)
 
-Up-scaling python functions for high performance computing (HPC) can be challenging. While the python standard library
-provides interfaces for multiprocessing and asynchronous task execution, namely
-[multiprocessing](https://docs.python.org/3/library/multiprocessing.html) and
-[concurrent.futures](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures) both are
-limited to the execution on a single compute node. So a series of python libraries have been developed to address the
-up-scaling of python functions for HPC. Starting in the datascience and machine learning community with solutions
-like [dask](https://www.dask.org) over more HPC focused solutions like
-[fireworks](https://materialsproject.github.io/fireworks/) and [parsl](http://parsl-project.org) up to Python
-bindings for the message passing interface (MPI) named [mpi4py](https://mpi4py.readthedocs.io). Each of these
-solutions has their advantages and disadvantages, in particular scaling beyond serial python functions, including thread
-based parallelism, MPI parallel python application or assignment of GPUs to individual python function remains
-challenging.
-
-To address these challenges `pympipool` is developed with three goals in mind:
-
-* Extend the standard python library [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures) 
-  interface, to minimize the barrier of up-scaling an existing workflow to be used on HPC resources.
-* Integrate thread based parallelism, MPI parallel python functions based on [mpi4py](https://mpi4py.readthedocs.io) and 
-  GPU assignment. This allows the users to accelerate their workflows one function at a time.
-* Embrace [Jupyter](https://jupyter.org) notebooks for the interactive development of HPC workflows, as they allow the 
-  users to document their though process right next to the python code and their results all within one document.
-
-## HPC Context
-In contrast to frameworks like [dask](https://www.dask.org), [fireworks](https://materialsproject.github.io/fireworks/)
-and [parsl](http://parsl-project.org) which can be used to submit a number of worker processes directly the the HPC
-queuing system and then transfer tasks from either the login node or an interactive allocation to these worker processes
-to accelerate the execution, [mpi4py](https://mpi4py.readthedocs.io) and `pympipool` follow a different
-approach. Here the user creates their HPC allocation first and then [mpi4py](https://mpi4py.readthedocs.io) or
-`pympipool` can be used to distribute the tasks within this allocation. The advantage of this approach is that
-no central data storage is required as the workers and the scheduling task can communicate directly.
+## Challenges
+In high performance computing (HPC) the Python programming language is commonly used as high-level language to
+orchestrate the coupling of scientific applications. Still the efficient usage of highly parallel HPC clusters remains
+challenging, in primarily three aspects:
+
+* **Communication**: Distributing python function calls over hundreds of compute node and gathering the results on a
+  shared file system is technically possible, but highly inefficient. A socket-based communication approach is 
+  preferable.
+* **Resource Management**: Assigning Python functions to GPUs or executing Python functions on multiple CPUs using the 
+  message passing interface (MPI) requires major modifications to the python workflow.
+* **Integration**: Existing workflow libraries implement a secondary the job management on the Python level rather than
+  leveraging the existing infrastructure provided by the job scheduler of the HPC.
+
+### pympipool is ...
+In a given HPC allocation the `pympipool` library addresses these challenges by extending the Executor interface
+of the standard Python library to support the resource assignment in the HPC context. Computing resources can either be
+assigned on a per function call basis or as a block allocation on a per Executor basis. The `pympipool` library
+is built on top of the [flux-framework](https://flux-framework.org) to enable fine-grained resource assignment. In
+addition, [Simple Linux Utility for Resource Management (SLURM)](https://slurm.schedmd.com) is supported as alternative
+queuing system and for workstation installations `pympipool` can be installed without a job scheduler.
+
+### pympipool is not ...
+The pympipool library is not designed to request an allocation from the job scheduler of an HPC. Instead within a given
+allocation from the job scheduler the `pympipool` library can be employed to distribute a series of python
+function calls over the available computing resources to achieve maximum computing resource utilization.
 
-## Examples
+## Example
 The following examples illustrates how `pympipool` can be used to distribute a series of MPI parallel function calls 
 within a queuing system allocation. `example.py`:
-```
+```python
+import flux.job
 from pympipool import Executor
 
 def calc(i):
     from mpi4py import MPI
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
     return i, size, rank
 
-with Executor(max_workers=2, cores_per_worker=2) as exe:
-    fs_0 = exe.submit(calc, 0)
-    fs_1 = exe.submit(calc, 1)
-    print(fs_0.result(), fs_1.result())
+with flux.job.FluxExecutor() as flux_exe:
+    with Executor(max_cores=2, cores_per_worker=2, executor=flux_exe) as exe:
+        fs = exe.submit(calc, 3)
+        print(fs.result())
 ```
-This example can be executed using::
+This example can be executed using:
 ```
 python example.py
 ```
-Which returns::
+Which returns:
 ```
 >>> [(0, 2, 0), (0, 2, 1)], [(1, 2, 0), (1, 2, 1)]
 ```
 The important part in this example is that [mpi4py](https://mpi4py.readthedocs.io) is only used in the `calc()`
 function, not in the python script, consequently it is not necessary to call the script with `mpiexec` but instead
 a call with the regular python interpreter is sufficient. This highlights how `pympipool` allows the users to
 parallelize one function at a time and not having to convert their whole workflow to use [mpi4py](https://mpi4py.readthedocs.io).
 The same code can also be executed inside a jupyter notebook directly which enables an interactive development process.
 
-The standard [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
-interface is extended by adding the option `cores_per_worker=2` to assign multiple MPI ranks to each function call.
-To create two workers `max_workers=2` each with two cores each requires a total of four CPU cores to be available.
+The interface of the standard [concurrent.futures.Executor](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
+is extended by adding the option `cores_per_worker=2` to assign multiple MPI ranks to each function call. To create two 
+workers the maximum number of cores can be increased to `max_cores=4`. In this case each worker receives two cores
+resulting in a total of four CPU cores being utilized.
+
 After submitting the function `calc()` with the corresponding parameter to the executor `exe.submit(calc, 0)`
 a python [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) is
 returned. Consequently, the `pympipool.Executor` can be used as a drop-in replacement for the
 [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
 which allows the user to add parallelism to their workflow one function at a time.
 
-## Backends
-Depending on the availability of different resource schedulers in your HPC environment the `pympipool.Executor`
-uses a different backend, with the `pympipool.flux.PyFluxExecutor` being the preferred backend:
-
-* `pympipool.mpi.PyMpiExecutor`: The simplest executor of the three uses [mpi4py](https://mpi4py.readthedocs.io) as a 
-  backend. This simplifies the installation on all operating systems including Windows. Still at the same time it limits 
-  the up-scaling to a single compute node and serial or MPI parallel python functions. There is no support for thread 
-  based parallelism or GPU assignment. This interface is primarily used for testing and developing or as a fall-back 
-  solution. It is not recommended to use this interface in production.
-* `pympipool.slurm.PySlurmExecutor`: The [SLURM workload manager](https://www.schedmd.com) is commonly used on HPC 
-  systems to schedule and distribute tasks. `pympipool` provides a python interface for scheduling the execution of 
-  python functions as SLURM job steps which are typically created using the `srun` command. This executor supports 
-  serial python functions, thread based parallelism, MPI based parallelism and the assignment of GPUs to individual 
-  python functions. When the [SLURM workload manager](https://www.schedmd.com) is installed on your HPC cluster this 
-  interface can be a reasonable choice, still depending on the [SLURM workload manager](https://www.schedmd.com) 
-  configuration in can be limited in terms of the fine-grained scheduling or the responsiveness when working with 
-  hundreds of compute nodes in an individual allocation.
-* `pympipool.flux.PyFluxExecutor`: The [flux framework](https://flux-framework.org) is the preferred backend for 
-  `pympipool`. Just like the `pympipool.slurm.PySlurmExecutor` it supports serial python functions, thread based 
-  parallelism, MPI based parallelism and the assignment of GPUs to individual python functions. Still the advantages of 
-  using the [flux framework](https://flux-framework.org) as a backend are the easy installation, the faster allocation 
-  of resources as the resources are managed within the allocation and no central databases is used and the superior 
-  level of fine-grained resource assignment which is typically not available on HPC resource schedulers.
-
-Each of these backends consists of two parts a broker and a worker. When a new tasks is submitted from the user it is
-received by the broker and the broker identifies the first available worker. The worker then executes a task and returns
-it to the broker, who returns it to the user. While there is only one broker per `pympipool.Executor` the number
-of workers can be specified with the `max_workers` parameter.
-
 ## Disclaimer
 While we try to develop a stable and reliable software library, the development remains a opensource project under the
 BSD 3-Clause License without any warranties::
 ```
 BSD 3-Clause License
 
 Copyright (c) 2022, Jan Janssen
@@ -192,18 +161,23 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
 # Documentation
 * [Installation](https://pympipool.readthedocs.io/en/latest/installation.html)
-  * [Basic Installation](https://pympipool.readthedocs.io/en/latest/installation.html#basic-installation)
-  * [High Performance Computing](https://pympipool.readthedocs.io/en/latest/installation.html#high-performance-computing)
+  * [Compatible Job Schedulers](https://pympipool.readthedocs.io/en/latest/installation.html#compatible-job-schedulers)
+  * [pympipool with Flux Framework](https://pympipool.readthedocs.io/en/latest/installation.html#pympipool-with-flux-framework)
+  * [Test Flux Framework](https://pympipool.readthedocs.io/en/latest/installation.html#test-flux-framework)
+  * [Without Flux Framework](https://pympipool.readthedocs.io/en/latest/installation.html#without-flux-framework)
 * [Examples](https://pympipool.readthedocs.io/en/latest/examples.html)
   * [Compatibility](https://pympipool.readthedocs.io/en/latest/examples.html#compatibility)
+  * [Resource Assignment](https://pympipool.readthedocs.io/en/latest/examples.html#resource-assignment)
   * [Data Handling](https://pympipool.readthedocs.io/en/latest/examples.html#data-handling)
   * [Up-Scaling](https://pympipool.readthedocs.io/en/latest/examples.html#up-scaling)
+  * [SLURM Job Scheduler](https://pympipool.readthedocs.io/en/latest/examples.html#slurm-job-scheduler) 
+  * [Workstation Support](https://pympipool.readthedocs.io/en/latest/examples.html#workstation-support)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html)
   * [Contributions](https://pympipool.readthedocs.io/en/latest/development.html#contributions)
+  * [License](https://pympipool.readthedocs.io/en/latest/development.html#license)
   * [Integration](https://pympipool.readthedocs.io/en/latest/development.html#integration)
-  * [Alternative Projects](https://pympipool.readthedocs.io/en/latest/development.html#alternative-projects)
 * [Module Index](https://pympipool.readthedocs.io/en/latest/py-modindex.html)
```

### Comparing `pympipool-0.7.9/README.md` & `pympipool-0.8.0/pympipool.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,137 @@
+Metadata-Version: 2.1
+Name: pympipool
+Version: 0.8.0
+Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
+Author-email: Jan Janssen <janssen@lanl.gov>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2022, Jan Janssen
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/pyiron/pympipool
+Project-URL: Documentation, https://pympipool.readthedocs.io
+Project-URL: Repository, https://github.com/pyiron/pympipool
+Keywords: pyiron
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: <3.13,>=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
+Requires-Dist: mpi4py<=3.1.6,>=3.1.4
+Requires-Dist: pyzmq<=26.0.2,>=25.0.0
+Requires-Dist: tqdm<=4.66.2,>=4.44.0
+
 # pympipool - up-scale python functions for high performance computing
 [![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pympipool/HEAD?labpath=notebooks%2Fexamples.ipynb)
 
-Up-scaling python functions for high performance computing (HPC) can be challenging. While the python standard library
-provides interfaces for multiprocessing and asynchronous task execution, namely
-[multiprocessing](https://docs.python.org/3/library/multiprocessing.html) and
-[concurrent.futures](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures) both are
-limited to the execution on a single compute node. So a series of python libraries have been developed to address the
-up-scaling of python functions for HPC. Starting in the datascience and machine learning community with solutions
-like [dask](https://www.dask.org) over more HPC focused solutions like
-[fireworks](https://materialsproject.github.io/fireworks/) and [parsl](http://parsl-project.org) up to Python
-bindings for the message passing interface (MPI) named [mpi4py](https://mpi4py.readthedocs.io). Each of these
-solutions has their advantages and disadvantages, in particular scaling beyond serial python functions, including thread
-based parallelism, MPI parallel python application or assignment of GPUs to individual python function remains
-challenging.
-
-To address these challenges `pympipool` is developed with three goals in mind:
-
-* Extend the standard python library [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures) 
-  interface, to minimize the barrier of up-scaling an existing workflow to be used on HPC resources.
-* Integrate thread based parallelism, MPI parallel python functions based on [mpi4py](https://mpi4py.readthedocs.io) and 
-  GPU assignment. This allows the users to accelerate their workflows one function at a time.
-* Embrace [Jupyter](https://jupyter.org) notebooks for the interactive development of HPC workflows, as they allow the 
-  users to document their though process right next to the python code and their results all within one document.
-
-## HPC Context
-In contrast to frameworks like [dask](https://www.dask.org), [fireworks](https://materialsproject.github.io/fireworks/)
-and [parsl](http://parsl-project.org) which can be used to submit a number of worker processes directly the the HPC
-queuing system and then transfer tasks from either the login node or an interactive allocation to these worker processes
-to accelerate the execution, [mpi4py](https://mpi4py.readthedocs.io) and `pympipool` follow a different
-approach. Here the user creates their HPC allocation first and then [mpi4py](https://mpi4py.readthedocs.io) or
-`pympipool` can be used to distribute the tasks within this allocation. The advantage of this approach is that
-no central data storage is required as the workers and the scheduling task can communicate directly.
+## Challenges
+In high performance computing (HPC) the Python programming language is commonly used as high-level language to
+orchestrate the coupling of scientific applications. Still the efficient usage of highly parallel HPC clusters remains
+challenging, in primarily three aspects:
+
+* **Communication**: Distributing python function calls over hundreds of compute node and gathering the results on a
+  shared file system is technically possible, but highly inefficient. A socket-based communication approach is 
+  preferable.
+* **Resource Management**: Assigning Python functions to GPUs or executing Python functions on multiple CPUs using the 
+  message passing interface (MPI) requires major modifications to the python workflow.
+* **Integration**: Existing workflow libraries implement a secondary the job management on the Python level rather than
+  leveraging the existing infrastructure provided by the job scheduler of the HPC.
+
+### pympipool is ...
+In a given HPC allocation the `pympipool` library addresses these challenges by extending the Executor interface
+of the standard Python library to support the resource assignment in the HPC context. Computing resources can either be
+assigned on a per function call basis or as a block allocation on a per Executor basis. The `pympipool` library
+is built on top of the [flux-framework](https://flux-framework.org) to enable fine-grained resource assignment. In
+addition, [Simple Linux Utility for Resource Management (SLURM)](https://slurm.schedmd.com) is supported as alternative
+queuing system and for workstation installations `pympipool` can be installed without a job scheduler.
+
+### pympipool is not ...
+The pympipool library is not designed to request an allocation from the job scheduler of an HPC. Instead within a given
+allocation from the job scheduler the `pympipool` library can be employed to distribute a series of python
+function calls over the available computing resources to achieve maximum computing resource utilization.
 
-## Examples
+## Example
 The following examples illustrates how `pympipool` can be used to distribute a series of MPI parallel function calls 
 within a queuing system allocation. `example.py`:
-```
+```python
+import flux.job
 from pympipool import Executor
 
 def calc(i):
     from mpi4py import MPI
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
     return i, size, rank
 
-with Executor(max_workers=2, cores_per_worker=2) as exe:
-    fs_0 = exe.submit(calc, 0)
-    fs_1 = exe.submit(calc, 1)
-    print(fs_0.result(), fs_1.result())
+with flux.job.FluxExecutor() as flux_exe:
+    with Executor(max_cores=2, cores_per_worker=2, executor=flux_exe) as exe:
+        fs = exe.submit(calc, 3)
+        print(fs.result())
 ```
-This example can be executed using::
+This example can be executed using:
 ```
 python example.py
 ```
-Which returns::
+Which returns:
 ```
 >>> [(0, 2, 0), (0, 2, 1)], [(1, 2, 0), (1, 2, 1)]
 ```
 The important part in this example is that [mpi4py](https://mpi4py.readthedocs.io) is only used in the `calc()`
 function, not in the python script, consequently it is not necessary to call the script with `mpiexec` but instead
 a call with the regular python interpreter is sufficient. This highlights how `pympipool` allows the users to
 parallelize one function at a time and not having to convert their whole workflow to use [mpi4py](https://mpi4py.readthedocs.io).
 The same code can also be executed inside a jupyter notebook directly which enables an interactive development process.
 
-The standard [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
-interface is extended by adding the option `cores_per_worker=2` to assign multiple MPI ranks to each function call.
-To create two workers `max_workers=2` each with two cores each requires a total of four CPU cores to be available.
+The interface of the standard [concurrent.futures.Executor](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
+is extended by adding the option `cores_per_worker=2` to assign multiple MPI ranks to each function call. To create two 
+workers the maximum number of cores can be increased to `max_cores=4`. In this case each worker receives two cores
+resulting in a total of four CPU cores being utilized.
+
 After submitting the function `calc()` with the corresponding parameter to the executor `exe.submit(calc, 0)`
 a python [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) is
 returned. Consequently, the `pympipool.Executor` can be used as a drop-in replacement for the
 [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
 which allows the user to add parallelism to their workflow one function at a time.
 
-## Backends
-Depending on the availability of different resource schedulers in your HPC environment the `pympipool.Executor`
-uses a different backend, with the `pympipool.flux.PyFluxExecutor` being the preferred backend:
-
-* `pympipool.mpi.PyMpiExecutor`: The simplest executor of the three uses [mpi4py](https://mpi4py.readthedocs.io) as a 
-  backend. This simplifies the installation on all operating systems including Windows. Still at the same time it limits 
-  the up-scaling to a single compute node and serial or MPI parallel python functions. There is no support for thread 
-  based parallelism or GPU assignment. This interface is primarily used for testing and developing or as a fall-back 
-  solution. It is not recommended to use this interface in production.
-* `pympipool.slurm.PySlurmExecutor`: The [SLURM workload manager](https://www.schedmd.com) is commonly used on HPC 
-  systems to schedule and distribute tasks. `pympipool` provides a python interface for scheduling the execution of 
-  python functions as SLURM job steps which are typically created using the `srun` command. This executor supports 
-  serial python functions, thread based parallelism, MPI based parallelism and the assignment of GPUs to individual 
-  python functions. When the [SLURM workload manager](https://www.schedmd.com) is installed on your HPC cluster this 
-  interface can be a reasonable choice, still depending on the [SLURM workload manager](https://www.schedmd.com) 
-  configuration in can be limited in terms of the fine-grained scheduling or the responsiveness when working with 
-  hundreds of compute nodes in an individual allocation.
-* `pympipool.flux.PyFluxExecutor`: The [flux framework](https://flux-framework.org) is the preferred backend for 
-  `pympipool`. Just like the `pympipool.slurm.PySlurmExecutor` it supports serial python functions, thread based 
-  parallelism, MPI based parallelism and the assignment of GPUs to individual python functions. Still the advantages of 
-  using the [flux framework](https://flux-framework.org) as a backend are the easy installation, the faster allocation 
-  of resources as the resources are managed within the allocation and no central databases is used and the superior 
-  level of fine-grained resource assignment which is typically not available on HPC resource schedulers.
-
-Each of these backends consists of two parts a broker and a worker. When a new tasks is submitted from the user it is
-received by the broker and the broker identifies the first available worker. The worker then executes a task and returns
-it to the broker, who returns it to the user. While there is only one broker per `pympipool.Executor` the number
-of workers can be specified with the `max_workers` parameter.
-
 ## Disclaimer
 While we try to develop a stable and reliable software library, the development remains a opensource project under the
 BSD 3-Clause License without any warranties::
 ```
 BSD 3-Clause License
 
 Copyright (c) 2022, Jan Janssen
@@ -136,18 +161,23 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
 # Documentation
 * [Installation](https://pympipool.readthedocs.io/en/latest/installation.html)
-  * [Basic Installation](https://pympipool.readthedocs.io/en/latest/installation.html#basic-installation)
-  * [High Performance Computing](https://pympipool.readthedocs.io/en/latest/installation.html#high-performance-computing)
+  * [Compatible Job Schedulers](https://pympipool.readthedocs.io/en/latest/installation.html#compatible-job-schedulers)
+  * [pympipool with Flux Framework](https://pympipool.readthedocs.io/en/latest/installation.html#pympipool-with-flux-framework)
+  * [Test Flux Framework](https://pympipool.readthedocs.io/en/latest/installation.html#test-flux-framework)
+  * [Without Flux Framework](https://pympipool.readthedocs.io/en/latest/installation.html#without-flux-framework)
 * [Examples](https://pympipool.readthedocs.io/en/latest/examples.html)
   * [Compatibility](https://pympipool.readthedocs.io/en/latest/examples.html#compatibility)
+  * [Resource Assignment](https://pympipool.readthedocs.io/en/latest/examples.html#resource-assignment)
   * [Data Handling](https://pympipool.readthedocs.io/en/latest/examples.html#data-handling)
   * [Up-Scaling](https://pympipool.readthedocs.io/en/latest/examples.html#up-scaling)
+  * [SLURM Job Scheduler](https://pympipool.readthedocs.io/en/latest/examples.html#slurm-job-scheduler) 
+  * [Workstation Support](https://pympipool.readthedocs.io/en/latest/examples.html#workstation-support)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html)
   * [Contributions](https://pympipool.readthedocs.io/en/latest/development.html#contributions)
+  * [License](https://pympipool.readthedocs.io/en/latest/development.html#license)
   * [Integration](https://pympipool.readthedocs.io/en/latest/development.html#integration)
-  * [Alternative Projects](https://pympipool.readthedocs.io/en/latest/development.html#alternative-projects)
 * [Module Index](https://pympipool.readthedocs.io/en/latest/py-modindex.html)
```

### Comparing `pympipool-0.7.9/pympipool/backend/mpiexec.py` & `pympipool-0.8.0/pympipool/backend/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.9/pympipool/backend/serial.py` & `pympipool-0.8.0/pympipool/backend/serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from os.path import abspath
 import sys
+from typing import Optional
 
 from pympipool.shared.communication import (
     interface_connect,
     interface_send,
     interface_shutdown,
     interface_receive,
 )
 from pympipool.shared.backend import call_funct, parse_arguments
 
 
-def main(argument_lst=None):
+def main(argument_lst: Optional[list[str]] = None):
     if argument_lst is None:
         argument_lst = sys.argv
     argument_dict = parse_arguments(argument_lst=argument_lst)
     context, socket = interface_connect(
         host=argument_dict["host"], port=argument_dict["zmqport"]
     )
```

### Comparing `pympipool-0.7.9/pympipool/shared/backend.py` & `pympipool-0.8.0/pympipool/shared/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import Optional
 import inspect
 
 
-def call_funct(input_dict, funct=None, memory=None):
+def call_funct(
+    input_dict: dict, funct: Optional[callable] = None, memory: Optional[dict] = None
+) -> callable:
     """
     Call function from dictionary
 
     Args:
         input_dict (dict): dictionary containing the function 'fn', its arguments 'args' and keyword arguments 'kwargs'
         funct (None): function to be evaluated if it is not included in the input dictionary
         memory (dict/ None): variables stored in memory which can be used as keyword arguments
@@ -26,15 +29,15 @@
                 dict_output=input_dict["kwargs"],
                 keys_possible_lst=funct_args,
             )
         )
     return funct(input_dict["fn"], *input_dict["args"], **input_dict["kwargs"])
 
 
-def parse_arguments(argument_lst):
+def parse_arguments(argument_lst: list[str]) -> dict:
     """
     Simple function to parse command line arguments
 
     Args:
         argument_lst (list): list of arguments as strings
 
     Returns:
@@ -46,24 +49,28 @@
             "zmqport": "--zmqport",
             "host": "--host",
         },
         default_dict={"host": "localhost"},
     )
 
 
-def update_default_dict_from_arguments(argument_lst, argument_dict, default_dict):
+def update_default_dict_from_arguments(
+    argument_lst: list[str], argument_dict: dict, default_dict: dict
+) -> dict:
     default_dict.update(
         {
             k: argument_lst[argument_lst.index(v) + 1]
             for k, v in argument_dict.items()
             if v in argument_lst
         }
     )
     return default_dict
 
 
-def _update_dict_delta(dict_input, dict_output, keys_possible_lst):
+def _update_dict_delta(
+    dict_input: dict, dict_output: dict, keys_possible_lst: list
+) -> dict:
     return {
         k: v
         for k, v in dict_input.items()
         if k in keys_possible_lst and k not in dict_output.keys()
     }
```

### Comparing `pympipool-0.7.9/pympipool/shared/thread.py` & `pympipool-0.8.0/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.9/pympipool/shell/executor.py` & `pympipool-0.8.0/pympipool/shell/executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import queue
 from concurrent.futures import Future
 import subprocess
 
-from pympipool.shared.executorbase import executor_broker, ExecutorBase
+from pympipool.shared.executorbase import ExecutorBroker
 from pympipool.shared.thread import RaisingThread
 
 
-def execute_single_task(future_queue):
+def execute_single_task(future_queue: queue.Queue):
     """
     Process items received via the queue.
 
     Args:
         future_queue (queue.Queue):
     """
     while True:
@@ -33,73 +34,51 @@
                     raise thread_exception
                 else:
                     future_queue.task_done()
         else:
             raise KeyError(task_dict)
 
 
-class SubprocessSingleExecutor(ExecutorBase):
-    """
-    The pympipool.shell.SubprocessSingleExecutor is the internal worker for the pympipool.shell.SubprocessExecutor.
-    """
-
-    def __init__(self):
-        super().__init__()
-        self._process = RaisingThread(
-            target=execute_single_task,
-            kwargs={
-                "future_queue": self._future_queue,
-            },
-        )
-        self._process.start()
-
-    def submit(self, *args, **kwargs):
-        f = Future()
-        self._future_queue.put({"future": f, "args": args, "kwargs": kwargs})
-        return f
-
-
-class SubprocessExecutor(ExecutorBase):
+class SubprocessExecutor(ExecutorBroker):
     """
     The pympipool.shell.SubprocessExecutor enables the submission of command line calls via the subprocess.check_output()
     interface of the python standard library. It is based on the concurrent.futures.Executor class and returns a
     concurrent.futures.Future object for every submitted command line call. Still it does not provide any option to
     interact with the external executable during the execution.
 
     Args:
         max_workers (int): defines the number workers which can execute functions in parallel
-        sleep_interval (float): synchronization interval - default 0.1
 
     Examples:
 
         >>> from pympipool import SubprocessExecutor
         >>> with SubprocessExecutor(max_workers=2) as exe:
         >>>     future = exe.submit(["echo", "test"], universal_newlines=True)
         >>> print(future.done(), future.result(), future.done())
         (False, "test", True)
 
     """
 
     def __init__(
         self,
-        max_workers=1,
-        sleep_interval=0.1,
+        max_workers: int = 1,
     ):
         super().__init__()
-        self._process = RaisingThread(
-            target=executor_broker,
-            kwargs={
-                # Broker Arguments
-                "future_queue": self._future_queue,
-                "max_workers": max_workers,
-                "sleep_interval": sleep_interval,
-                "executor_class": SubprocessSingleExecutor,
-            },
+        self._set_process(
+            process=[
+                RaisingThread(
+                    target=execute_single_task,
+                    kwargs={
+                        # Executor Arguments
+                        "future_queue": self._future_queue,
+                    },
+                )
+                for _ in range(max_workers)
+            ],
         )
-        self._process.start()
 
     def submit(self, *args, **kwargs):
         """
         Submit a command line call to be executed. The given arguments are provided to subprocess.Popen() as additional
         inputs to control the execution.
 
         Returns:
```

### Comparing `pympipool-0.7.9/pympipool/shell/interactive.py` & `pympipool-0.8.0/pympipool/shell/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import queue
+import threading
+from typing import Optional
 from concurrent.futures import Future
 import subprocess
 from time import sleep
 
 from pympipool.shared.executorbase import cancel_items_in_queue, ExecutorBase
 from pympipool.shared.thread import RaisingThread
 
 
-def wait_for_process_to_stop(process, sleep_interval=10e-10):
+def wait_for_process_to_stop(process: threading.Thread, sleep_interval: float = 10e-10):
     """
     Wait for the subprocess.Popen() process to stop executing
 
     Args:
         process (subprocess.Popen): process object
         sleep_interval (float): interval to sleep during poll() calls
     """
     while process.poll() is None:
         sleep(sleep_interval)
 
 
-def execute_single_task(future_queue):
+def execute_single_task(future_queue: queue.Queue):
     """
     Process items received via the queue.
 
     Args:
         future_queue (queue.Queue):
     """
     process = None
@@ -103,24 +106,30 @@
         >>>     future_pattern = exe.submit(string_input="4", stop_read_pattern="done")
         >>>     print(future_pattern.done(), future_pattern.result(), future_pattern.done())
         (False, "0\n1\n2\n3\ndone\n", True)
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__()
-        self._process = RaisingThread(
-            target=execute_single_task,
-            kwargs={
-                "future_queue": self._future_queue,
-            },
+        self._set_process(
+            process=RaisingThread(
+                target=execute_single_task,
+                kwargs={
+                    "future_queue": self._future_queue,
+                },
+            ),
         )
-        self._process.start()
         self._future_queue.put({"init": True, "args": args, "kwargs": kwargs})
 
-    def submit(self, string_input, lines_to_read=None, stop_read_pattern=None):
+    def submit(
+        self,
+        string_input: str,
+        lines_to_read: Optional[int] = None,
+        stop_read_pattern: Optional[str] = None,
+    ):
         """
         Submit the input as a string to the executable. In addition to the input the ShellExecutor also needs a measure
         to identify the completion of the execution. This can either be provided based on the number of lines to read
         using the `lines_to_read` parameter or by providing a string pattern using the `stop_read_pattern` to stop
         reading new lines. One of these two stopping criteria has to be defined.
 
         Args:
@@ -144,15 +153,15 @@
                 "input": string_input,
                 "lines_to_read": lines_to_read,
                 "stop_read_pattern": stop_read_pattern,
             }
         )
         return f
 
-    def shutdown(self, wait=True, *, cancel_futures=False):
+    def shutdown(self, wait: bool = True, *, cancel_futures: bool = False):
         """Clean-up the resources associated with the Executor.
 
         It is safe to call this method several times. Otherwise, no other
         methods can be called after this one.
 
         Args:
             wait: If True then shutdown will not return until all running
```

### Comparing `pympipool-0.7.9/pympipool.egg-info/SOURCES.txt` & `pympipool-0.8.0/pympipool.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 pympipool/flux/executor.py
 pympipool/mpi/__init__.py
 pympipool/mpi/executor.py
 pympipool/shared/__init__.py
 pympipool/shared/backend.py
 pympipool/shared/communication.py
 pympipool/shared/executorbase.py
+pympipool/shared/inputcheck.py
 pympipool/shared/interface.py
 pympipool/shared/thread.py
 pympipool/shell/__init__.py
 pympipool/shell/executor.py
 pympipool/shell/interactive.py
 pympipool/slurm/__init__.py
 pympipool/slurm/executor.py
-tests/test_flux.py
-tests/test_future.py
-tests/test_interface.py
-tests/test_meta.py
-tests/test_parse.py
-tests/test_queue.py
-tests/test_serial.py
-tests/test_shell_interactive.py
-tests/test_subprocess_executor.py
-tests/test_task.py
-tests/test_thread.py
-tests/test_with_dynamic_objects.py
-tests/test_worker.py
-tests/test_worker_memory.py
-tests/test_zmq.py
+tests/test_backend_serial.py
+tests/test_executor_backend_flux.py
+tests/test_executor_backend_mpi.py
+tests/test_executor_backend_mpi_noblock.py
+tests/test_flux_executor.py
+tests/test_integration_pyiron_workflow.py
+tests/test_mpi_executor.py
+tests/test_mpi_executor_future.py
+tests/test_shared_backend.py
+tests/test_shared_communication.py
+tests/test_shared_executorbase.py
+tests/test_shared_thread.py
+tests/test_shell_executor.py
+tests/test_shell_interactive.py
```

### Comparing `pympipool-0.7.9/pyproject.toml` & `pympipool-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 description = "Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process."
 authors = [
     { name = "Jan Janssen", email = "janssen@lanl.gov" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["pyiron"]
-requires-python = ">=3.8"
+requires-python = ">=3.9, <3.13"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Physics",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "cloudpickle>=2.0.0,<=3.0.0",
-    "mpi4py>=3.1.4,<=3.1.5",
-    "pyzmq>=25.0.0,<=25.1.1",
-    "tqdm>=4.44.0,<=4.66.1",
+    "mpi4py>=3.1.4,<=3.1.6",
+    "pyzmq>=25.0.0,<=26.0.2",
+    "tqdm>=4.44.0,<=4.66.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pyiron/pympipool"
 Documentation = "https://pympipool.readthedocs.io"
 Repository = "https://github.com/pyiron/pympipool"
```

### Comparing `pympipool-0.7.9/tests/test_flux.py` & `pympipool-0.8.0/tests/test_flux_executor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from concurrent.futures import Future
 import os
 from queue import Queue
+import unittest
 
 import numpy as np
-import unittest
 
-from pympipool.shared.executorbase import cloudpickle_register, executor_broker, execute_parallel_tasks
+from pympipool.shared.executorbase import cloudpickle_register, execute_parallel_tasks
 
 
 try:
     import flux.job
     from pympipool.flux.executor import (
         PyFluxExecutor,
-        PyFluxSingleTaskExecutor,
         FluxPythonInterface,
     )
 
     skip_flux_test = "FLUX_URI" not in os.environ
 except ImportError:
     skip_flux_test = True
 
@@ -73,15 +72,17 @@
             max_workers=1, cores_per_worker=2, executor=self.executor
         ) as exe:
             fs_1 = exe.submit(mpi_funct, 1)
             self.assertEqual(fs_1.result(), [(1, 2, 0), (1, 2, 1)])
             self.assertTrue(fs_1.done())
 
     def test_single_task(self):
-        with PyFluxSingleTaskExecutor(cores=2, executor=self.executor) as p:
+        with PyFluxExecutor(
+            max_workers=1, cores_per_worker=2, executor=self.executor
+        ) as p:
             output = p.map(mpi_funct, [1, 2, 3])
         self.assertEqual(
             list(output),
             [[(1, 2, 0), (1, 2, 1)], [(2, 2, 0), (2, 2, 1)], [(3, 2, 0), (3, 2, 1)]],
         )
 
     def test_execute_task(self):
@@ -112,45 +113,17 @@
             executor=self.executor,
             interface_class=FluxPythonInterface,
         )
         self.assertEqual(f.result(), 2)
         q.join()
 
     def test_internal_memory(self):
-        with PyFluxSingleTaskExecutor(
-            cores=1, init_function=set_global, executor=self.executor
+        with PyFluxExecutor(
+            max_workers=1,
+            cores_per_worker=1,
+            init_function=set_global,
+            executor=self.executor,
         ) as p:
             f = p.submit(get_global)
             self.assertFalse(f.done())
             self.assertEqual(f.result(), np.array([5]))
             self.assertTrue(f.done())
-
-    def test_executor_broker(self):
-        q = Queue()
-        f = Future()
-        q.put({"fn": calc, "args": (1,), "kwargs": {}, "future": f})
-        q.put({"shutdown": True, "wait": True})
-        executor_broker(
-            future_queue=q,
-            max_workers=1,
-            executor=self.executor,
-            executor_class=PyFluxSingleTaskExecutor,
-        )
-        self.assertTrue(f.done())
-        self.assertEqual(f.result(), 1)
-        q.join()
-
-    def test_executor_broker_threads(self):
-        q = Queue()
-        f = Future()
-        q.put({"fn": calc, "args": (1,), "kwargs": {}, "future": f})
-        q.put({"shutdown": True, "wait": True})
-        executor_broker(
-            future_queue=q,
-            max_workers=1,
-            threads_per_core=2,
-            executor=self.executor,
-            executor_class=PyFluxSingleTaskExecutor,
-        )
-        self.assertTrue(f.done())
-        self.assertEqual(f.result(), 1)
-        q.join()
```

### Comparing `pympipool-0.7.9/tests/test_future.py` & `pympipool-0.8.0/tests/test_mpi_executor_future.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-import numpy as np
-import unittest
-from time import sleep
-from pympipool.mpi.executor import PyMPISingleTaskExecutor
 from concurrent.futures import Future
+from time import sleep
+import unittest
+
+import numpy as np
+
+from pympipool.mpi.executor import PyMPIExecutor
 
 
 def calc(i):
     return np.array(i**2)
 
 
 class TestFuture(unittest.TestCase):
     def test_pool_serial(self):
-        with PyMPISingleTaskExecutor(cores=1) as p:
+        with PyMPIExecutor(
+            max_workers=1, cores_per_worker=1, hostname_localhost=True
+        ) as p:
             output = p.submit(calc, i=2)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
         self.assertTrue(output.done())
         self.assertEqual(output.result(), np.array(4))
 
     def test_pool_serial_multi_core(self):
-        with PyMPISingleTaskExecutor(cores=2) as p:
+        with PyMPIExecutor(
+            max_workers=1, cores_per_worker=2, hostname_localhost=True
+        ) as p:
             output = p.submit(calc, i=2)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
         self.assertTrue(output.done())
         self.assertEqual(output.result(), [np.array(4), np.array(4)])
 
@@ -35,80 +41,85 @@
         """
 
         with self.subTest("From the main process"):
             mutable = []
 
             def slow_callable():
                 from time import sleep
+
                 sleep(1)
                 return True
 
             def callback(future):
                 mutable.append("Called back")
 
             def submit():
                 # Executor only exists in this scope and can get garbage collected after
                 # this function is exits
-                future = PyMPISingleTaskExecutor().submit(slow_callable)
+                future = PyMPIExecutor(hostname_localhost=True).submit(slow_callable)
                 future.add_done_callback(callback)
                 return future
 
             self.assertListEqual(
                 [],
                 mutable,
-                msg="Sanity check that test is starting in the expected condition"
+                msg="Sanity check that test is starting in the expected condition",
             )
             future = submit()
 
             self.assertFalse(
                 future.done(),
-                msg="The submit function is slow, it should be running still"
+                msg="The submit function is slow, it should be running still",
             )
             self.assertListEqual(
                 [],
                 mutable,
                 msg="While running, the mutable should not have been impacted by the "
-                    "callback"
+                "callback",
             )
             future.result()  # Wait for the calculation to finish
             self.assertListEqual(
                 ["Called back"],
                 mutable,
-                msg="After completion, the callback should modify the mutable data"
+                msg="After completion, the callback should modify the mutable data",
             )
 
         with self.subTest("From inside a class"):
+
             class Foo:
                 def __init__(self):
                     self.running = False
 
                 def run(self):
                     self.running = True
 
-                    future = PyMPISingleTaskExecutor().submit(self.return_42)
+                    future = PyMPIExecutor(hostname_localhost=True).submit(
+                        self.return_42
+                    )
                     future.add_done_callback(self.finished)
 
                     return future
 
                 def return_42(self):
                     from time import sleep
+
                     sleep(1)
                     return 42
 
                 def finished(self, future):
                     self.running = False
 
             foo = Foo()
             self.assertFalse(
                 foo.running,
-                msg="Sanity check that the test starts in the expected condition"
+                msg="Sanity check that the test starts in the expected condition",
             )
             fs = foo.run()
             self.assertTrue(
                 foo.running,
-                msg="We should be able to exit the run method before the task completes"
+                msg="We should be able to exit the run method before the task completes",
             )
             fs.result()  # Wait for completion
             self.assertFalse(
                 foo.running,
-                msg="After task completion, we expect the callback to modify the class"
-            )
+                msg="After task completion, we expect the callback to modify the class",
+            )
```

### Comparing `pympipool-0.7.9/tests/test_interface.py` & `pympipool-0.8.0/tests/test_shared_communication.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import os
 import sys
+import unittest
 
 import numpy as np
-import unittest
-from pympipool.shared.communication import SocketInterface
+import zmq
+
+from pympipool.shared.communication import (
+    interface_connect,
+    interface_shutdown,
+    interface_send,
+    interface_receive,
+    SocketInterface,
+)
 from pympipool.shared.executorbase import cloudpickle_register
 from pympipool.shared.interface import MpiExecInterface
 
 
 def calc(i):
     return np.array(i**2)
 
 
 class TestInterface(unittest.TestCase):
     def test_interface(self):
         cloudpickle_register(ind=1)
         task_dict = {"fn": calc, "args": (), "kwargs": {"i": 2}}
         interface = SocketInterface(
-            interface=MpiExecInterface(
-                cwd=None, cores=1, oversubscribe=False
-            )
+            interface=MpiExecInterface(cwd=None, cores=1, oversubscribe=False)
         )
         interface.bootup(
             command_lst=[
                 sys.executable,
                 os.path.abspath(
                     os.path.join(
                         __file__, "..", "..", "pympipool", "backend", "mpiexec.py"
@@ -33,7 +39,22 @@
                 str(interface.bind_to_random_port()),
             ]
         )
         self.assertEqual(
             interface.send_and_receive_dict(input_dict=task_dict), np.array(4)
         )
         interface.shutdown(wait=True)
+
+
+class TestZMQ(unittest.TestCase):
+    def test_initialize_zmq(self):
+        message = "test"
+        host = "localhost"
+
+        context_server = zmq.Context()
+        socket_server = context_server.socket(zmq.PAIR)
+        port = str(socket_server.bind_to_random_port("tcp://*"))
+        context_client, socket_client = interface_connect(host=host, port=port)
+        interface_send(socket=socket_server, result_dict={"message": message})
+        self.assertEqual(interface_receive(socket=socket_client), {"message": message})
+        interface_shutdown(socket=socket_client, context=context_client)
+        interface_shutdown(socket=socket_server, context=context_server)
```

### Comparing `pympipool-0.7.9/tests/test_parse.py` & `pympipool-0.8.0/tests/test_shared_backend.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 import unittest
+
 from pympipool.shared.backend import parse_arguments
 from pympipool.shared.interface import SrunInterface, MpiExecInterface
 
 
 class TestParser(unittest.TestCase):
     def test_command_local(self):
         result_dict = {
@@ -17,17 +18,15 @@
             "2",
             "--oversubscribe",
             sys.executable,
             "/",
             "--zmqport",
             result_dict["zmqport"],
         ]
-        interface = MpiExecInterface(
-            cwd=None, cores=2, oversubscribe=True
-        )
+        interface = MpiExecInterface(cwd=None, cores=2, oversubscribe=True)
         self.assertEqual(
             command_lst,
             interface.generate_command(
                 command_lst=[sys.executable, "/", "--zmqport", result_dict["zmqport"]]
             ),
         )
         self.assertEqual(result_dict, parse_arguments(command_lst))
@@ -57,14 +56,58 @@
         )
         self.assertEqual(
             command_lst,
             interface.generate_command(
                 command_lst=[
                     sys.executable,
                     "/",
+                    "--host",
+                    result_dict["host"],
+                    "--zmqport",
+                    result_dict["zmqport"],
+                ]
+            ),
+        )
+        self.assertEqual(result_dict, parse_arguments(command_lst))
+
+    def test_command_slurm_user_command(self):
+        result_dict = {
+            "host": "127.0.0.1",
+            "zmqport": "22",
+        }
+        command_lst = [
+            "srun",
+            "-n",
+            "2",
+            "-D",
+            os.path.abspath("."),
+            "--gpus-per-task=1",
+            "--oversubscribe",
+            "--account=test",
+            "--job-name=pympipool",
+            sys.executable,
+            "/",
+            "--host",
+            result_dict["host"],
+            "--zmqport",
+            result_dict["zmqport"],
+        ]
+        interface = SrunInterface(
+            cwd=os.path.abspath("."),
+            cores=2,
+            gpus_per_core=1,
+            oversubscribe=True,
+            command_line_argument_lst=["--account=test", "--job-name=pympipool"],
+        )
+        self.assertEqual(
+            command_lst,
+            interface.generate_command(
+                command_lst=[
+                    sys.executable,
+                    "/",
                     "--host",
                     result_dict["host"],
                     "--zmqport",
                     result_dict["zmqport"],
                 ]
             ),
         )
```

### Comparing `pympipool-0.7.9/tests/test_queue.py` & `pympipool-0.8.0/tests/test_shared_executorbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import unittest
 from concurrent.futures import Future, CancelledError
 from queue import Queue
+import unittest
+
 from pympipool.shared.executorbase import cancel_items_in_queue
 
 
 class TestQueue(unittest.TestCase):
     def test_cancel_items_in_queue(self):
         q = Queue()
         fs1 = Future()
```

### Comparing `pympipool-0.7.9/tests/test_serial.py` & `pympipool-0.8.0/tests/test_backend_serial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from threading import Thread
 import unittest
+
 import cloudpickle
 import zmq
+
 from pympipool.backend.serial import main
-from threading import Thread
 
 
 def calc(i, j):
     return i + j
 
 
 def set_global():
```

### Comparing `pympipool-0.7.9/tests/test_shell_interactive.py` & `pympipool-0.8.0/tests/test_shell_interactive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,70 @@
 from concurrent.futures import Future
 import os
 import queue
-
-from unittest import TestCase
+import unittest
 
 from pympipool.shell.interactive import ShellExecutor, execute_single_task
 
 
-class ShellInteractiveExecutorTest(TestCase):
+class ShellInteractiveExecutorTest(unittest.TestCase):
     def setUp(self):
-        self.executable_path = os.path.join(os.path.dirname(__file__), "executables", "count.py")
+        self.executable_path = os.path.join(
+            os.path.dirname(__file__), "executables", "count.py"
+        )
 
     def test_execute_single_task(self):
         test_queue = queue.Queue()
         future_lines = Future()
         future_pattern = Future()
-        test_queue.put({"init": True, "args": [["python", self.executable_path]], "kwargs": {"universal_newlines": True}})
-        test_queue.put({"future": future_lines, "input": "4\n", "lines_to_read": 5, "stop_read_pattern": None})
-        test_queue.put({"future": future_pattern, "input": "4\n", "lines_to_read": None, "stop_read_pattern": "done"})
+        test_queue.put(
+            {
+                "init": True,
+                "args": [["python", self.executable_path]],
+                "kwargs": {"universal_newlines": True},
+            }
+        )
+        test_queue.put(
+            {
+                "future": future_lines,
+                "input": "4\n",
+                "lines_to_read": 5,
+                "stop_read_pattern": None,
+            }
+        )
+        test_queue.put(
+            {
+                "future": future_pattern,
+                "input": "4\n",
+                "lines_to_read": None,
+                "stop_read_pattern": "done",
+            }
+        )
         test_queue.put({"shutdown": True})
         self.assertFalse(future_lines.done())
         self.assertFalse(future_pattern.done())
         execute_single_task(future_queue=test_queue)
         self.assertTrue(future_lines.done())
         self.assertTrue(future_pattern.done())
         self.assertEqual("0\n1\n2\n3\ndone\n", future_lines.result())
         self.assertEqual("0\n1\n2\n3\ndone\n", future_pattern.result())
 
     def test_shell_interactive_executor(self):
-        with ShellExecutor(["python", self.executable_path], universal_newlines=True) as exe:
-            future_lines = exe.submit(string_input="4", lines_to_read=5, stop_read_pattern=None)
-            future_pattern = exe.submit(string_input="4", lines_to_read=None, stop_read_pattern="done")
+        with ShellExecutor(
+            ["python", self.executable_path], universal_newlines=True
+        ) as exe:
+            future_lines = exe.submit(
+                string_input="4", lines_to_read=5, stop_read_pattern=None
+            )
+            future_pattern = exe.submit(
+                string_input="4", lines_to_read=None, stop_read_pattern="done"
+            )
             self.assertFalse(future_lines.done())
             self.assertFalse(future_pattern.done())
             self.assertEqual("0\n1\n2\n3\ndone\n", future_lines.result())
             self.assertEqual("0\n1\n2\n3\ndone\n", future_pattern.result())
             self.assertTrue(future_lines.done())
             self.assertTrue(future_pattern.done())
+
+    def test_meta(self):
+        with ShellExecutor(["sleep"]) as exe:
+            self.assertEqual(exe.info, {})
```

### Comparing `pympipool-0.7.9/tests/test_subprocess_executor.py` & `pympipool-0.8.0/tests/test_shell_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 from concurrent.futures import Future
 import queue
+import unittest
 
-from unittest import TestCase
+from pympipool.shell.executor import SubprocessExecutor, execute_single_task
 
-from pympipool.shell.executor import SubprocessSingleExecutor, SubprocessExecutor, execute_single_task
 
-
-class SubprocessExecutorTest(TestCase):
+class SubprocessExecutorTest(unittest.TestCase):
     def test_execute_single_task(self):
         test_queue = queue.Queue()
         f = Future()
-        test_queue.put({"future": f, "args": [["echo", "test"]], "kwargs": {"universal_newlines": True}})
+        test_queue.put(
+            {
+                "future": f,
+                "args": [["echo", "test"]],
+                "kwargs": {"universal_newlines": True},
+            }
+        )
         test_queue.put({"shutdown": True})
         self.assertFalse(f.done())
         execute_single_task(future_queue=test_queue)
         self.assertTrue(f.done())
         self.assertEqual("test\n", f.result())
 
+    def test_wrong_error(self):
+        test_queue = queue.Queue()
+        test_queue.put({"wrong_key": True})
+        with self.assertRaises(KeyError):
+            execute_single_task(future_queue=test_queue)
+
+    def test_broken_executable(self):
+        test_queue = queue.Queue()
+        f = Future()
+        test_queue.put(
+            {
+                "future": f,
+                "args": [["/executable/does/not/exist"]],
+                "kwargs": {"universal_newlines": True},
+            }
+        )
+        with self.assertRaises(FileNotFoundError):
+            execute_single_task(future_queue=test_queue)
+
     def test_shell_static_executor_args(self):
-        with SubprocessSingleExecutor() as exe:
+        with SubprocessExecutor(max_workers=1) as exe:
             future = exe.submit(["echo", "test"], universal_newlines=True, shell=False)
             self.assertFalse(future.done())
             self.assertEqual("test\n", future.result())
             self.assertTrue(future.done())
 
     def test_shell_static_executor_binary(self):
-        with SubprocessSingleExecutor() as exe:
+        with SubprocessExecutor(max_workers=1) as exe:
             future = exe.submit(["echo", "test"], universal_newlines=False, shell=False)
             self.assertFalse(future.done())
             self.assertEqual(b"test\n", future.result())
             self.assertTrue(future.done())
 
     def test_shell_static_executor_shell(self):
-        with SubprocessSingleExecutor() as exe:
+        with SubprocessExecutor(max_workers=1) as exe:
             future = exe.submit("echo test", universal_newlines=True, shell=True)
             self.assertFalse(future.done())
             self.assertEqual("test\n", future.result())
             self.assertTrue(future.done())
 
     def test_shell_executor(self):
         with SubprocessExecutor(max_workers=2) as exe:
```

### Comparing `pympipool-0.7.9/tests/test_with_dynamic_objects.py` & `pympipool-0.8.0/tests/test_integration_pyiron_workflow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 The purpose of these tests is the check executor behaviour when the python objects
 are dynamically generated.
 This is a special (and rather difficult) case for serializing objects which cannot
 be pickled using the standard pickle module, and thus poses a relatively thorough test
 for the general un-pickle-able case.
 """
+
 from concurrent.futures._base import TimeoutError as cfbTimeoutError
 from functools import partialmethod
 from time import sleep
 import unittest
 
 from pympipool import Executor
+from pympipool.shared.executorbase import cloudpickle_register
 
 
 class Foo:
     """
     A base class to be dynamically modified for putting an executor/serializer through
     its paces.
     """
+
     def __init__(self, fnc: callable):
         self.fnc = fnc
         self.result = None
         self.running = False
 
     @property
     def run(self):
@@ -36,24 +39,20 @@
 def dynamic_foo():
     """
     A decorator for dynamically modifying the Foo class to test
     CloudpickleProcessPoolExecutor.
 
     Overrides the `fnc` input of `Foo` with the decorated function.
     """
+
     def as_dynamic_foo(fnc: callable):
         return type(
             "DynamicFoo",
             (Foo,),  # Define parentage
-            {
-                "__init__": partialmethod(
-                    Foo.__init__,
-                    fnc
-                )
-            },
+            {"__init__": partialmethod(Foo.__init__, fnc)},
         )
 
     return as_dynamic_foo
 
 
 class TestDynamicallyDefinedObjects(unittest.TestCase):
     def test_args(self):
@@ -71,22 +70,23 @@
             Returns a complex, dynamically defined variable
             """
             sleep(0.1)
             dynamic_arg.attribute_on_dynamic = "attribute updated"
             return dynamic_arg
 
         dynamic_dynamic = slowly_returns_dynamic()
-        executor = Executor()
+        executor = Executor(hostname_localhost=True, block_allocation=True)
+        cloudpickle_register(ind=1)
         dynamic_object = does_nothing()
         fs = executor.submit(dynamic_dynamic.run, dynamic_object)
         self.assertEqual(
             fs.result().attribute_on_dynamic,
             "attribute updated",
             msg="The submit callable should have modified the mutable, dynamically "
-                "defined object with a new attribute."
+            "defined object with a new attribute.",
         )
 
     def test_callable(self):
         """
         We should be able to use a dynamic callable -- in this case, a method of
         a dynamically defined class.
         """
@@ -95,82 +95,80 @@
         @dynamic_foo()
         def slowly_returns_42():
             sleep(0.1)
             return fortytwo
 
         dynamic_42 = slowly_returns_42()  # Instantiate the dynamically defined class
         self.assertIsInstance(
-            dynamic_42,
-            Foo,
-            msg="Just a sanity check that the test is set up right"
+            dynamic_42, Foo, msg="Just a sanity check that the test is set up right"
         )
         self.assertIsNone(
-            dynamic_42.result,
-            msg="Just a sanity check that the test is set up right"
+            dynamic_42.result, msg="Just a sanity check that the test is set up right"
         )
-        executor = Executor()
+        executor = Executor(hostname_localhost=True, block_allocation=True)
+        cloudpickle_register(ind=1)
         fs = executor.submit(dynamic_42.run)
         fs.add_done_callback(dynamic_42.process_result)
         self.assertFalse(
             fs.done(),
             msg="The submit callable sleeps long enough that we expect to still be "
-                "running here -- did something fail to get submit to an executor??"
+            "running here -- did something fail to get submit to an executor??",
         )
         self.assertEqual(
-            fortytwo,
-            fs.result(),
-            msg="The future is expected to behave as usual"
+            fortytwo, fs.result(), msg="The future is expected to behave as usual"
         )
         self.assertEqual(
             fortytwo,
             dynamic_42.result,
             msg="The callback modifies its object and should run by the time the result"
-                "is available -- did it fail to get called?"
+            "is available -- did it fail to get called?",
         )
 
     def test_callback(self):
         """Make sure the callback methods can modify their owners"""
 
         @dynamic_foo()
         def returns_42():
             return 42
 
         dynamic_42 = returns_42()
         self.assertFalse(
             dynamic_42.running,
-            msg="Sanity check that the test starts in the expected condition"
+            msg="Sanity check that the test starts in the expected condition",
         )
-        executor = Executor()
+        executor = Executor(hostname_localhost=True, block_allocation=True)
+        cloudpickle_register(ind=1)
         fs = executor.submit(dynamic_42.run)
         fs.add_done_callback(dynamic_42.process_result)
         self.assertTrue(
             dynamic_42.running,
-            msg="Submit method need to be able to modify their owners"
+            msg="Submit method need to be able to modify their owners",
         )
         fs.result()  # Wait for the process to finish
         self.assertFalse(
             dynamic_42.running,
-            msg="Callback methods need to be able to modify their owners"
+            msg="Callback methods need to be able to modify their owners",
         )
 
     def test_exception(self):
         """
         Exceptions from dynamically defined callables should get cleanly raised.
         """
 
         @dynamic_foo()
         def raise_error():
             raise RuntimeError
 
         re = raise_error()
-        executor = Executor()
+        executor = Executor(hostname_localhost=True, block_allocation=True)
+        cloudpickle_register(ind=1)
         fs = executor.submit(re.run)
         with self.assertRaises(
             RuntimeError,
-            msg="The callable just raises an error -- this should get shown to the user"
+            msg="The callable just raises an error -- this should get shown to the user",
         ):
             fs.result()
 
     def test_return(self):
         """
         We should be able to use a dynamic return value -- in this case, a
         method of a dynamically defined class.
@@ -187,27 +185,28 @@
             """
             sleep(0.1)
             inside_variable = does_nothing()
             inside_variable.result = "it was an inside job!"
             return inside_variable
 
         dynamic_dynamic = slowly_returns_dynamic()
-        executor = Executor()
+        executor = Executor(hostname_localhost=True, block_allocation=True)
+        cloudpickle_register(ind=1)
         fs = executor.submit(dynamic_dynamic.run)
         self.assertIsInstance(
             fs.result(),
             Foo,
             msg="Just a sanity check that we're getting the right type of dynamically "
-                "defined type of object"
+            "defined type of object",
         )
         self.assertEqual(
             fs.result().result,
             "it was an inside job!",
             msg="The submit callable modifies the object that owns it, and this should"
-                "be reflected in the main process after deserialziation"
+            "be reflected in the main process after deserialziation",
         )
 
     def test_timeout(self):
         """
         Timeouts for dynamically defined callables should be handled ok.
         """
 
@@ -215,22 +214,23 @@
 
         @dynamic_foo()
         def slow():
             sleep(0.1)
             return fortytwo
 
         f = slow()
-        executor = Executor()
+        executor = Executor(hostname_localhost=True, block_allocation=True)
+        cloudpickle_register(ind=1)
         fs = executor.submit(f.run)
         self.assertEqual(
             fs.result(timeout=30),
             fortytwo,
-            msg="waiting long enough should get the result"
+            msg="waiting long enough should get the result",
         )
 
         with self.assertRaises(
             (TimeoutError, cfbTimeoutError),
             msg="With a timeout time smaller than our submit callable's sleep time, "
-                "we had better get an exception!"
+            "we had better get an exception!",
         ):
             fs = executor.submit(f.run)
             fs.result(timeout=0.0001)
```

