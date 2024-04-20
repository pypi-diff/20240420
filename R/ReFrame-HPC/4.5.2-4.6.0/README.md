# Comparing `tmp/ReFrame-HPC-4.5.2.tar.gz` & `tmp/reframe_hpc-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.5.2.tar", last modified: Tue Mar 26 20:44:54 2024, max compression
+gzip compressed data, was "reframe_hpc-4.6.0.tar", last modified: Sat Apr 20 17:40:59 2024, max compression
```

## Comparing `ReFrame-HPC-4.5.2.tar` & `reframe_hpc-4.6.0.tar`

### file list

```diff
@@ -1,135 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-03-26 20:44:54.000000 ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-26 20:44:54.000000 ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:44:54.000000 ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-26 20:44:54.000000 ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 20:44:54.000000 ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/bin/reframe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.268155 ReFrame-HPC-4.5.2/hpctestlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.264155 ReFrame-HPC-4.5.2/hpctestlib/data_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/data_analytics/spark/
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/data_analytics/spark/spark_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/data_analytics/spark/src/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/data_analytics/spark/src/spark_pi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.264155 ReFrame-HPC-4.5.2/hpctestlib/interactive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.264155 ReFrame-HPC-4.5.2/hpctestlib/interactive/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/interactive/jupyter/ipcmagic/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/interactive/jupyter/ipcmagic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.264155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/dgemm/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/gpu_burn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/kernel_latency/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/memory_bandwidth/
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/pointer_chase/
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/shmem/
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/shmem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/mpi/osu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.268155 ReFrame-HPC-4.5.2/hpctestlib/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/ml/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/ml/pytorch/horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/ml/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/ml/tensorflow/horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.268155 ReFrame-HPC-4.5.2/hpctestlib/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/python/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/python/numpy/numpy_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/python/numpy/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/python/numpy/src/np_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.268155 ReFrame-HPC-4.5.2/hpctestlib/sciapps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/sciapps/amber/
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/sciapps/amber/nve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/sciapps/gromacs/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/sciapps/gromacs/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.268155 ReFrame-HPC-4.5.2/hpctestlib/system/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/system/fs/
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/system/fs/mnt_opts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/hpctestlib/system/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/hpctestlib/system/ssh/host_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.272155 ReFrame-HPC-4.5.2/reframe/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.280155 ReFrame-HPC-4.5.2/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)    32121 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    24544 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    44510 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.280155 ReFrame-HPC-4.5.2/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/launchers/rsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    94981 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.280155 ReFrame-HPC-4.5.2/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25262 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/schedulers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    29700 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (127)    58136 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    26118 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:44:54.284155 ReFrame-HPC-4.5.2/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (127)    50110 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (127)    28585 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    32327 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-26 20:44:48.000000 ReFrame-HPC-4.5.2/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-26 20:44:54.288155 ReFrame-HPC-4.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/bin/reframe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/data_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/spark_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/src/spark_pi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/interactive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/ipcmagic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/ipcmagic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/dgemm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/gpu_burn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/kernel_latency/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/memory_bandwidth/
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/pointer_chase/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/shmem/
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/shmem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/mpi/osu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/ml/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/ml/pytorch/horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/ml/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/ml/tensorflow/horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/python/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/python/numpy/numpy_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/python/numpy/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/python/numpy/src/np_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/sciapps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/sciapps/amber/
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/sciapps/amber/nve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/sciapps/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/sciapps/gromacs/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/sciapps/qespresso/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/sciapps/qespresso/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/system/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/system/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/system/fs/mnt_opts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/system/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/system/ssh/host_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/reframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.175196 reframe_hpc-4.6.0/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32254 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24544 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44509 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.179196 reframe_hpc-4.6.0/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/rsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95804 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.179196 reframe_hpc-4.6.0/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26548 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23494 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32104 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58260 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    26802 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)    50528 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28585 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32327 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/setup.cfg
```

### Comparing `ReFrame-HPC-4.5.2/LICENSE` & `reframe_hpc-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/PKG-INFO` & `reframe_hpc-4.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.5.2
+Version: 4.6.0
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.5.2/README.md` & `reframe_hpc-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/README_minimal.md` & `reframe_hpc-4.6.0/README_minimal.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/PKG-INFO` & `reframe_hpc-4.6.0/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.5.2
+Version: 4.6.0
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.5.2/ReFrame_HPC.egg-info/SOURCES.txt` & `reframe_hpc-4.6.0/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 hpctestlib/microbenchmarks/mpi/osu.py
 hpctestlib/ml/pytorch/horovod.py
 hpctestlib/ml/tensorflow/horovod.py
 hpctestlib/python/numpy/numpy_ops.py
 hpctestlib/python/numpy/src/np_ops.py
 hpctestlib/sciapps/amber/nve.py
 hpctestlib/sciapps/gromacs/benchmarks.py
+hpctestlib/sciapps/qespresso/benchmarks.py
 hpctestlib/system/fs/mnt_opts.py
 hpctestlib/system/ssh/host_keys.py
 reframe/__init__.py
 reframe/core/backends.py
 reframe/core/buildsystems.py
 reframe/core/builtins.py
 reframe/core/config.py
```

### Comparing `ReFrame-HPC-4.5.2/bin/reframe` & `reframe_hpc-4.6.0/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/data_analytics/spark/spark_checks.py` & `reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/spark_checks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/interactive/jupyter/ipcmagic/__init__.py` & `reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/ipcmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/gpu_burn.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/gpu_burn.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/gpu/shmem/__init__.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/shmem/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/microbenchmarks/mpi/osu.py` & `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/mpi/osu.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/ml/pytorch/horovod.py` & `reframe_hpc-4.6.0/hpctestlib/ml/pytorch/horovod.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/ml/tensorflow/horovod.py` & `reframe_hpc-4.6.0/hpctestlib/ml/tensorflow/horovod.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/python/numpy/numpy_ops.py` & `reframe_hpc-4.6.0/hpctestlib/python/numpy/numpy_ops.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/python/numpy/src/np_ops.py` & `reframe_hpc-4.6.0/hpctestlib/python/numpy/src/np_ops.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/sciapps/amber/nve.py` & `reframe_hpc-4.6.0/hpctestlib/sciapps/amber/nve.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/sciapps/gromacs/benchmarks.py` & `reframe_hpc-4.6.0/hpctestlib/sciapps/gromacs/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/system/fs/mnt_opts.py` & `reframe_hpc-4.6.0/hpctestlib/system/fs/mnt_opts.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/hpctestlib/system/ssh/host_keys.py` & `reframe_hpc-4.6.0/hpctestlib/system/ssh/host_keys.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/__init__.py` & `reframe_hpc-4.6.0/reframe/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.5.2'
+VERSION = '4.6.0'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/backends.py` & `reframe_hpc-4.6.0/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/buildsystems.py` & `reframe_hpc-4.6.0/reframe/core/buildsystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,15 @@
 
     #: The CMake build directory, where all the generated files will be placed.
     #:
     #: :type: :class:`str`
     #: :default: :class:`None`
     builddir = variable(str, type(None), value=None)
 
-    #: Additional configuration options to be passed to the CMake invocation.
+    #: Additional configuration options to be passed to the configure step.
     #:
     #: :type: :class:`List[str]`
     #: :default: ``[]``
     config_opts = variable(typ.List[str], value=[])
 
     #: Options to be passed to the subsequent ``make`` invocation.
     #:
@@ -774,14 +774,18 @@
         self._eb_modules = [
             {'name': m, 'collection': False, 'path': modulesdir}
             for m in re.findall(r'building and installing (\S+)...', out)
         ]
 
     @property
     def generated_modules(self):
+        '''List of the EasyBuild generated modules.
+
+        This list will be populated *after* the build succeeds.
+        '''
         return self._eb_modules
 
 
 class Spack(BuildSystem):
     '''A build system for building test code using `Spack
     <https://spack.io/>`__.
 
@@ -887,15 +891,14 @@
     #: is created, but before it is installed.
     #:
     #: :type: :class:`List[str]`
     #: :default: ``[]``
     #:
     preinstall_cmds = variable(typ.List[str], value=[])
 
-
     def __init__(self):
         # Set to True if the environment was auto-generated
         self._auto_env = False
 
     def emit_build_commands(self, environ):
         ret = self._create_env_cmds()
 
@@ -977,8 +980,8 @@
     def __set__(self, obj, value):
         if isinstance(value, str):
             try:
                 value = globals()[value]()
             except KeyError:
                 raise ValueError(f'unknown build system: {value}') from None
 
-        super().__set__(obj, value)
+        return super().__set__(obj, value)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/builtins.py` & `reframe_hpc-4.6.0/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/config.py` & `reframe_hpc-4.6.0/reframe/core/config.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/containers.py` & `reframe_hpc-4.6.0/reframe/core/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,8 +283,8 @@
     def __init__(self, *other_types):
         super().__init__(ContainerPlatform, *other_types)
 
     def __set__(self, obj, value):
         if isinstance(value, str):
             value = ContainerPlatform.create(value)
 
-        super().__set__(obj, value)
+        return super().__set__(obj, value)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/decorators.py` & `reframe_hpc-4.6.0/reframe/core/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         # Instantiate fixtures
 
         # Do a level-order traversal of the fixture registries of all leaf
         # tests, instantiate all fixtures and generate the final set of
         # candidate tests; the leaf tests are consumed at the end of the
         # traversal and all instantiated tests (including fixtures) are stored
         # in `final_tests`.
-        unset_vars = {}
         final_tests = []
         fixture_registry = FixtureRegistry()
         while leaf_tests:
             tmp_registry = FixtureRegistry()
             while leaf_tests:
                 c = leaf_tests.pop()
                 reg = getattr(c, '_rfm_fixture_registry', None)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/deferrable.py` & `reframe_hpc-4.6.0/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/environments.py` & `reframe_hpc-4.6.0/reframe/core/environments.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,14 +215,15 @@
     .. warning::
        Users may not create :class:`ProgEnvironment` objects directly.
     '''
 
     _cc = fields.TypedField(str)
     _cxx = fields.TypedField(str)
     _ftn = fields.TypedField(str)
+    _nvcc = fields.TypedField(str)
     _cppflags = fields.TypedField(typ.List[str])
     _cflags = fields.TypedField(typ.List[str])
     _cxxflags = fields.TypedField(typ.List[str])
     _fflags = fields.TypedField(typ.List[str])
     _ldflags = fields.TypedField(typ.List[str])
 
     def __init__(self,
@@ -237,26 +238,28 @@
                  ftn='ftn',
                  nvcc='nvcc',
                  cppflags=None,
                  cflags=None,
                  cxxflags=None,
                  fflags=None,
                  ldflags=None,
+                 resources=None,
                  **kwargs):
         super().__init__(name, modules, env_vars, extras, features,
                          prepare_cmds)
         self._cc = cc
         self._cxx = cxx
         self._ftn = ftn
         self._nvcc = nvcc
         self._cppflags = cppflags or []
         self._cflags   = cflags   or []
         self._cxxflags = cxxflags or []
         self._fflags   = fflags   or []
         self._ldflags  = ldflags  or []
+        self._resources = resources or {}
 
     @property
     def cc(self):
         '''The C compiler of this programming environment.
 
         :type: :class:`str`
         '''
@@ -316,8 +319,22 @@
 
         :type: :class:`List[str]`
         '''
         return self._ldflags
 
     @property
     def nvcc(self):
+        '''The NVIDIA CUDA compiler of this programming environment.
+
+        :type: :class:`str`
+        '''
         return self._nvcc
+
+    @property
+    def resources(self):
+        '''The scheduler resources associated with this environment.
+
+        .. versionadded:: 4.6.0
+
+        :type: :class:`Dict[str, object]`
+        '''
+        return self._resources
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/exceptions.py` & `reframe_hpc-4.6.0/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/fields.py` & `reframe_hpc-4.6.0/reframe/core/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,24 @@
         except KeyError:
             # We raise an AttributeError to emulate the standard attribute
             # access.
             raise AttributeError("%s object has no attribute '%s'" %
                                  (objtype.__name__, self._name)) from None
 
     def __set__(self, obj, value):
-        obj.__dict__[self._name] = remove_convertible(value)
+        # NOTE: We extend the Python data model by returning the value that
+        # would be otherwise written to the field, if ``obj`` is :obj:`None`.
+        # Subclasses must make sure to return to the caller the value returned
+        # from ``super().__set__(...)``.
+
+        value = remove_convertible(value)
+        if obj is None:
+            return value
+
+        obj.__dict__[self._name] = value
 
 
 class TypedField(Field):
     '''Stores a field of predefined type'''
 
     def __init__(self, main_type, *other_types,
                  attr_name=None, allow_implicit=False):
@@ -75,15 +84,15 @@
     def valid_types(self):
         return self._types
 
     def _check_type(self, value):
         if not any(isinstance(value, t) for t in self._types):
             typedescr = '|'.join(t.__name__ for t in self._types)
             raise TypeError(
-                "failed to set field '%s': '%s' is not of type '%s'" %
+                "failed to set variable '%s': '%s' is not of type '%s'" %
                 (self._name, value, typedescr))
 
     def __set__(self, obj, value):
         try:
             self._check_type(value)
         except TypeError:
             raw_value = remove_convertible(value)
@@ -96,26 +105,25 @@
             value = raw_value
             for t in self._types:
                 try:
                     value = t(value)
                 except TypeError:
                     continue
                 else:
-                    super().__set__(obj, value)
-                    return
+                    return super().__set__(obj, value)
 
             # Conversion failed
             typenames = [t.__name__ for t in self._types]
             raise TypeError(
-                f'failed to set field {self._name!r}: '
+                f'failed to set variable {self._name!r}: '
                 f'could not convert to any of the supported types: '
                 f'{typenames}'
             )
         else:
-            super().__set__(obj, value)
+            return super().__set__(obj, value)
 
 
 class ConstantField(Field):
     '''Holds a constant.
 
     Attempt to set it will raise an exception. This field may be accessed also
     from the class and will return the same constant value.
@@ -148,15 +156,15 @@
 
     def __set__(self, obj, value):
         value = remove_convertible(value)
         self._check_type(value)
         if not isinstance(value, ScopedDict):
             value = ScopedDict(value) if value is not None else value
 
-        Field.__set__(self, obj, value)
+        return Field.__set__(self, obj, value)
 
 
 class DeprecatedField(Field):
     '''Field wrapper for deprecating fields.'''
 
     OP_GET = 1
     OP_SET = 2
@@ -183,14 +191,14 @@
         self._op = op
         self._from_version = from_version
 
     def __set__(self, obj, value):
         if self._op & DeprecatedField.OP_SET:
             user_deprecation_warning(self._message, self._from_version)
 
-        self._target_field.__set__(obj, value)
+        return self._target_field.__set__(obj, value)
 
     def __get__(self, obj, objtype):
         if self._op & DeprecatedField.OP_GET:
             user_deprecation_warning(self._message, self._from_version)
 
         return self._target_field.__get__(obj, objtype)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/fixtures.py` & `reframe_hpc-4.6.0/reframe/core/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,18 +403,19 @@
         fixture class to derive from
         :class:`~reframe.core.pipeline.RunOnlyRegressionTest`.
 
       - **environment**: The extent of this scope covers a single combination
         of system partition and programming environment. Since the fixture is
         guaranteed to have the same partition and programming environment as
         the parent test, the fixture class can be any derived class from
-        :class:`~reframe.core.pipeline.RegressionTest`. * **test**: This scope
-        covers a single instance of the parent test, where the resources
-        provided by the fixture are exclusive to each parent test instance.
-        The fixture class can be any derived class from
+        :class:`~reframe.core.pipeline.RegressionTest`.
+
+      - **test**: This scope covers a single instance of the parent test,
+        where the resources provided by the fixture are exclusive to each
+        parent test instance. The fixture class can be any derived class from
         :class:`~reframe.core.pipeline.RegressionTest`.
 
     Rather than specifying the scope at the fixture class definition, ReFrame
     fixtures set the scope level from the consumer side (i.e. when used by
     another test or fixture). A test may declare multiple fixtures using the
     same class, where fixtures with different scopes are guaranteed to point
     to different instances of the fixture class. On the other hand, when two
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/hooks.py` & `reframe_hpc-4.6.0/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/launchers/local.py` & `reframe_hpc-4.6.0/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/launchers/mpi.py` & `reframe_hpc-4.6.0/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/launchers/rsh.py` & `reframe_hpc-4.6.0/reframe/core/launchers/rsh.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,9 +25,15 @@
 class SSHLauncher(JobLauncher):
     def command(self, job):
         hostname = job.sched_access[-1]
         ssh_opts = list(job.sched_access[:-1]) + self.options
         return ['ssh', '-o BatchMode=yes'] + ssh_opts + [hostname]
 
     def run_command(self, job):
+        cmd_tokens = []
+        if self.modifier:
+            cmd_tokens.append(self.modifier)
+            cmd_tokens += self.modifier_options
+
         # self.options is processed specially above
-        return ' '.join(self.command(job))
+        cmd_tokens += self.command(job)
+        return ' '.join(cmd_tokens)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/logging.py` & `reframe_hpc-4.6.0/reframe/core/logging.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/meta.py` & `reframe_hpc-4.6.0/reframe/core/meta.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/modules.py` & `reframe_hpc-4.6.0/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/namespaces.py` & `reframe_hpc-4.6.0/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/parameters.py` & `reframe_hpc-4.6.0/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/pipeline.py` & `reframe_hpc-4.6.0/reframe/core/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,18 @@
 
         :arg hook_name: The function name of the hook to be disabled.
 
         :meta private:
         '''
         self._disabled_hooks.add(hook_name)
 
+    @property
+    def disabled_hooks(self):
+        return self._disabled_hooks
+
     @classmethod
     def pipeline_hooks(cls):
         ret = {}
         last = {}
         for hook in cls._rfm_hook_registry:
             for stage, always_last in hook.stages:
                 if always_last:
@@ -725,58 +729,61 @@
     #:
     #: :type: boolean
     #: :default: :const:`False`
     #:
     #: .. versionadded:: 4.0.0
     require_reference = variable(typ.Bool, value=False, loggable=False)
 
-    #:
-    #: Refer to the :doc:`ReFrame Tutorials </tutorials>` for concrete usage
-    #: examples.
+    #: Patterns for checking the sanity of this test.
     #:
     #: If not set, a sanity error may be raised during sanity checking if no
     #: other sanity checking functions already exist.
     #:
     #: :type: A deferrable expression (i.e., the result of a :doc:`sanity
     #:     function </deferrable_functions_reference>`)
     #: :default: :class:`required`
     #:
     #: .. note::
     #:    .. versionchanged:: 2.9
     #:       The default behaviour has changed and it is now considered a
     #:       sanity failure if this attribute is set to :class:`required`.
     #:
-    #:       If a test doesn't care about its output, this must be stated
+    #:       If a test does not care about its output, this must be stated
     #:       explicitly as follows:
     #:
     #:       ::
     #:
     #:           self.sanity_patterns = sn.assert_true(1)
     #:
     #:    .. versionchanged:: 3.6
     #:       The default value has changed from ``None`` to ``required``.
+    #:
+    #: .. note::
+    #:
+    #:    You are advised to follow the new syntax for defining the sanity
+    #:    check of the test using the builtin :func:`@sanity_function
+    #:    <reframe.core.builtins.sanity_function>` decorator.
     sanity_patterns = variable(_DeferredExpression, loggable=False)
 
     #: Patterns for verifying the performance of this test.
     #:
     #: If set to :class:`None`, no performance checking will be performed.
     #:
     #: :type: A dictionary with keys of type :class:`str` and deferrable
     #:     expressions (i.e., the result of a :doc:`sanity function
     #:     </deferrable_functions_reference>`) as values.
     #:     :class:`None` is also allowed.
     #: :default: :class:`None`
     #:
-    #: .. warning::
+    #: .. note::
     #:
     #:    You are advised to follow the new syntax for defining performance
     #:    variables in your tests using either the :func:`@performance_function
     #:    <reframe.core.builtins.performance_function>` builtin or the
-    #:    :attr:`perf_variables`, as :attr:`perf_patterns` will likely be
-    #:    deprecated in the future.
+    #:    :attr:`perf_variables`.
     perf_patterns = variable(typ.Dict[str, _DeferredExpression], type(None),
                              loggable=False)
 
     #: The performance variables associated with the test.
     #:
     #: In this context, a performance variable is a key-value pair, where the
     #: key is the desired variable name and the value is the deferred
@@ -793,17 +800,14 @@
     #:
     #: This mapping may be extended or replaced by other performance variables
     #: that may be defined in any pipeline hook executing before the
     #: performance stage. To this end, deferred performance functions can be
     #: created inline using the utility
     #: :func:`~reframe.utility.sanity.make_performance_function`.
     #:
-    #: Refer to the :doc:`ReFrame Tutorials </tutorials>` for concrete usage
-    #: examples.
-    #:
     #: :type: A dictionary with keys of type :class:`str` and deferred
     #:     performance expressions as values (see
     #:     :ref:`deferrable-performance-functions`).
     #: :default: Collection of performance variables associated to each of
     #:     the member functions decorated with the :func:`@performance_function
     #:     <reframe.core.builtins.performance_function>`
     #:     decorator.
@@ -2028,15 +2032,21 @@
 
         # Update num_tasks if test is flexible
         if self.job.sched_flex_alloc_nodes:
             self.num_tasks = self.job.num_tasks
 
     def _map_resources_to_jobopts(self):
         resources_opts = []
-        for r, v in self.extra_resources.items():
+        # Combine all resources into one dictionary, where extra_resources
+        # can overwrite _current_environ.resources
+        combined_resources = {
+            **self._current_environ.resources,
+            **self.extra_resources
+        }
+        for r, v in combined_resources.items():
             resources_opts += self._current_partition.get_resource(r, **v)
 
         return resources_opts
 
     @final
     def compile_complete(self):
         '''Check if the build phase has completed.
@@ -2441,18 +2451,14 @@
             raise TypeError("'how' argument must be callable")
 
         self._userdeps.append((target, how))
 
     def getdep(self, target, environ=None, part=None):
         '''Retrieve the test case of a target dependency.
 
-        This is a low-level method. The :func:`@require_deps
-        <reframe.core.decorators.require_deps>` decorators should be
-        preferred.
-
         :arg target: The name of the target dependency to be retrieved.
         :arg environ: The name of the programming environment that will be
             used to retrieve the test case of the target test. If ``None``,
             :attr:`RegressionTest.current_environ` will be used.
 
         .. versionadded:: 2.21
 
@@ -2597,16 +2603,26 @@
 
     These tests are by default local and will skip the run phase of the
     regression test pipeline.
 
     The standard output and standard error of the test will be set to those of
     the compilation stage.
 
+    Compile-only tests do not need to define a sanity checking function, since
+    the compile stage will always fail if the compilation fails.
+    However, if a sanity function is defined, it will be used to validate the
+    test.
+
     This class is also directly available under the top-level :mod:`reframe`
     module.
+
+    .. versionchanged:: 4.6
+
+       Compile-only tests do not require an explicit sanity checking function.
+
     '''
 
     _rfm_regression_class_kind = _RFM_TEST_KIND_COMPILE
 
     def setup(self, partition, environ, **job_opts):
         '''The setup stage of the regression test pipeline.
 
@@ -2638,7 +2654,15 @@
         '''
 
     def run_wait(self):
         '''Wait for this test to finish.
 
         Implemented as no-op
         '''
+
+    def check_sanity(self):
+        # If no sanity function is defined, then use an identity expression
+        if (not hasattr(self, '_rfm_sanity') and
+            not hasattr(self, 'sanity_patterns')):
+            self.sanity_patterns = sn.assert_true(1)
+
+        super().check_sanity()
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/runtime.py` & `reframe_hpc-4.6.0/reframe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/__init__.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -149,14 +149,45 @@
         backends.
 
         :meta private:
         '''
         getlogger().log(level, f'[S] {self.registered_name}: {message}')
 
 
+def filter_nodes_by_state(nodelist, state):
+    '''Filter nodes by their state
+
+    :arg nodelist: List of :class:`Node` instances to filter.
+    :arg state: The state of the nodes.
+        If ``all``, the initial list is returned untouched.
+        If ``avail``, only the available nodes will be returned.
+        All other values are interpretes as a state string.
+        State match is exclusive unless the ``*`` is added at the end of the
+        state string.
+    :returns: the filtered node list
+    '''
+    if state == 'avail':
+        nodelist = {n for n in nodelist if n.is_avail()}
+    elif state != 'all':
+        if state.endswith('*'):
+            # non-exclusive stat match
+            state = state[:-1]
+            nodelist = {
+                n for n in nodelist if n.in_state(state)
+            }
+        else:
+            nodelist = {
+                n for n in nodelist if n.in_statex(state)
+            }
+
+    return nodelist
+    nodes[part.fullname] = [n.name for n in nodelist]
+
+
+
 class Job(jsonext.JSONSerializable, metaclass=JobMeta):
     '''A job descriptor.
 
     A job descriptor is created by the framework after the "setup" phase and
     is associated with the test.
 
     .. warning::
@@ -477,30 +508,31 @@
         '''
         return self._state
 
     @property
     def nodelist(self):
         '''The list of node names assigned to this job.
 
+        This attribute is supported by the ``local``, ``pbs``, ``slurm``,
+        ``squeue``, ``ssh``, and ``torque`` scheduler backends.
+
         This attribute is :class:`None` if no nodes are assigned to the job
         yet.
-        This attribute is set reliably only for the ``slurm`` backend, i.e.,
-        Slurm *with* accounting enabled.
+
         The ``squeue`` scheduler backend, i.e., Slurm *without* accounting,
         might not set this attribute for jobs that finish very quickly.
-        For the ``local`` scheduler backend, this returns an one-element list
+
+        For the ``local`` scheduler backend, this returns a one-element list
         containing the hostname of the current host.
 
         This attribute might be useful in a flexible regression test for
         determining the actual nodes that were assigned to the test.
         For more information on flexible node allocation, see the
         :option:`--flex-alloc-nodes` command-line option.
 
-        This attribute is *not* supported by the ``pbs`` scheduler backend.
-
         .. versionadded:: 2.17
 
         :type: :class:`List[str]` or :class:`None`
         '''
         return self._nodelist
 
     @property
@@ -564,24 +596,18 @@
 
         available_nodes = self.scheduler.allnodes()
         getlogger().debug(
             f'[F] Total available nodes: {len(available_nodes)}'
         )
 
         # Try to guess the number of tasks now
+        available_nodes = filter_nodes_by_state(
+            available_nodes, self.sched_flex_alloc_nodes.lower()
+        )
         available_nodes = self.scheduler.filternodes(self, available_nodes)
-        if self.sched_flex_alloc_nodes.casefold() != 'all':
-            available_nodes = {n for n in available_nodes
-                               if n.in_state(self.sched_flex_alloc_nodes)}
-            getlogger().debug(
-                f'[F] Selecting nodes in state '
-                f'{self.sched_flex_alloc_nodes!r}: '
-                f'available nodes now: {len(available_nodes)}'
-            )
-
         return len(available_nodes) * num_tasks_per_node
 
     def submit(self):
         return self.scheduler.submit(self)
 
     def wait(self):
         if self.jobid is None:
@@ -616,26 +642,53 @@
 class Node(abc.ABC):
     '''Abstract base class for representing system nodes.
 
     :meta private:
     '''
 
     @abc.abstractmethod
+    def in_statex(self, state):
+        '''Returns whether the node is in the give state exclusively.
+
+            :arg state: The node state.
+            :returns: :class:`True` if the nodes is exclusively
+                in the requested state.
+        '''
+
+    @abc.abstractmethod
     def in_state(self, state):
         '''Returns whether the node is in the given state.
 
            :arg state: The node state.
            :returns: :class:`True` if the nodes's state matches the given one,
                      :class:`False` otherwise.
         '''
 
+    @abc.abstractmethod
+    def is_avail(self):
+        '''Check whether the node is available for scheduling jobs.'''
+
+    def is_down(self):
+        '''Check whether node is down.
+
+        This is the inverse of :func:`is_avail`.
+        '''
+        return not self.is_avail()
+
 
 class AlwaysIdleNode(Node):
     def __init__(self, name):
         self._name = name
+        self._state = 'idle'
 
     @property
     def name(self):
         return self._name
 
+    def is_avail(self):
+        return True
+
+    def in_statex(self, state):
+        return state.lower() == self._state
+
     def in_state(self, state):
-        return state.casefold() == 'idle'
+        return self.in_statex(state)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/flux.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/local.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,18 +77,18 @@
         job._submit_time = time.time()
         job._state = 'RUNNING'
 
     def emit_preamble(self, job):
         return []
 
     def allnodes(self):
-        return [_LocalNode(socket.gethostname())]
+        return [sched.AlwaysIdleNode(socket.gethostname())]
 
     def filternodes(self, job, nodes):
-        return [_LocalNode(socket.gethostname())]
+        return [sched.AlwaysIdleNode(socket.gethostname())]
 
     def _kill_all(self, job):
         '''Send SIGKILL to all the processes of the spawned job.'''
         try:
             os.killpg(job.jobid, signal.SIGKILL)
             job._signal = signal.SIGKILL
         except (ProcessLookupError, PermissionError):
@@ -198,19 +198,7 @@
         # Retrieve the status of the job and return
         if os.WIFEXITED(status):
             job._exitcode = os.WEXITSTATUS(status)
             job._state = 'FAILURE' if job.exitcode != 0 else 'SUCCESS'
         elif os.WIFSIGNALED(status):
             job._state = 'FAILURE'
             job._signal = os.WTERMSIG(status)
-
-
-class _LocalNode(sched.Node):
-    def __init__(self, name):
-        self._name = name
-
-    @property
-    def name(self):
-        return self._name
-
-    def in_state(self, state):
-        return state.casefold() == 'idle'
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/lsf.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/oar.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/pbs.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/registry.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/sge.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/slurm.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/slurm.py`

 * *Files 9% similar despite different names*

```diff
@@ -209,34 +209,43 @@
                 )
             )
 
         for opt in job.sched_access:
             if not opt.strip().startswith(('-C', '--constraint')):
                 preamble.append('%s %s' % (self._prefix, opt))
 
+        # To avoid overriding a constraint that's passed into `sched_access`,
+        # we AND it with the `--constraint` option passed either in `options`
+        # or in `cli_options`
         constraints = []
         constraint_parser = ArgumentParser()
         constraint_parser.add_argument('-C', '--constraint')
         parsed_options, _ = constraint_parser.parse_known_args(
-            job.sched_access)
+            job.sched_access
+        )
         if parsed_options.constraint:
             constraints.append(parsed_options.constraint.strip())
 
         # NOTE: Here last of the passed --constraint job options is taken
         # into account in order to respect the behavior of slurm.
         parsed_options, _ = constraint_parser.parse_known_args(
             job.options + job.cli_options
         )
         if parsed_options.constraint:
             constraints.append(parsed_options.constraint.strip())
 
         if constraints:
-            preamble.append(
-                self._format_option('&'.join(constraints), '--constraint={0}')
-            )
+            if len(constraints) == 1:
+                constr = constraints[0]
+            else:
+                # Parenthesize the constraints prior to joining them with `&`
+                # to make sure that precedence is respected.
+                constr = '&'.join(f'({c})' for c in constraints)
+
+            preamble.append(self._format_option(constr, '--constraint={0}'))
 
         preamble.append(self._format_option(hint, '--hint={0}'))
         prefix_patt = re.compile(r'(#\w+)')
         for opt in job.options + job.cli_options:
             if opt.strip().startswith(('-C', '--constraint')):
                 # Constraints are already processed
                 continue
@@ -346,16 +355,15 @@
                 f'[F] No partition specified; using {default_partition!r}'
             )
 
         nodes = {n for n in nodes if n.partitions >= partitions}
         self.log(f'[F] Filtering nodes by partition(s) {partitions}: '
                  f'available nodes now: {len(nodes)}')
         if constraints:
-            constraints = set(constraints.strip().split('&'))
-            nodes = {n for n in nodes if n.active_features >= constraints}
+            nodes = {n for n in nodes if n.satisfies(constraints)}
             self.log(f'[F] Filtering nodes by constraint(s) {constraints}: '
                      f'available nodes now: {len(nodes)}')
 
         if nodelist:
             nodelist = nodelist.strip()
             nodes &= self._get_nodes_by_name(nodelist)
             self.log(f'[F] Filtering nodes by nodelist: {nodelist}: '
@@ -655,16 +663,40 @@
     def __hash__(self):
         return hash(self.name)
 
     def in_state(self, state):
         return all([self._states >= set(state.upper().split('+')),
                     self._partitions, self._active_features, self._states])
 
+    def in_statex(self, state):
+        return self._states == set(state.upper().split('+'))
+
+    def is_avail(self):
+        return any(self.in_statex(s)
+                   for s in ('ALLOCATED', 'COMPLETING', 'IDLE'))
+
     def is_down(self):
-        return bool({'DOWN', 'DRAIN', 'MAINT', 'NO_RESPOND'} & self._states)
+        return not self.is_avail()
+
+    def satisfies(self, slurm_constraint):
+        # Convert the Slurm constraint to a Python expression and evaluate it,
+        # but restrict our syntax to accept only AND or OR constraints and
+        # their combinations
+        if not re.match(r'^[\w\d\(\)\|\&]*$', slurm_constraint):
+            return False
+
+        names = {grp[0]
+                 for grp in re.finditer(r'(\w(\w|\d)*)', slurm_constraint)}
+        expr = slurm_constraint.replace('|', ' or ').replace('&', ' and ')
+        vars = {n: True for n in self.active_features}
+        vars.update({n: False for n in names - self.active_features})
+        try:
+            return eval(expr, {}, vars)
+        except BaseException:
+            return False
 
     @property
     def active_features(self):
         return self._active_features
 
     @property
     def name(self):
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/schedulers/ssh.py` & `reframe_hpc-4.6.0/reframe/core/schedulers/ssh.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/settings.py` & `reframe_hpc-4.6.0/reframe/core/settings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/shell.py` & `reframe_hpc-4.6.0/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/core/systems.py` & `reframe_hpc-4.6.0/reframe/core/systems.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     .. warning::
        Users may not create :class:`ProcessorInfo` objects directly.
 
     '''
 
     __slots__ = ()
     _known_attrs = (
-        'arch', 'num_cpus', 'num_cpus_per_core',
+        'arch', 'model', 'platform', 'num_cpus', 'num_cpus_per_core',
         'num_cpus_per_socket', 'num_sockets', 'topology'
     )
 
     @property
     def info(self):
         '''All the available information from the configuration.
 
@@ -124,15 +124,15 @@
 
     .. warning::
        Users may not create :class:`DeviceInfo` objects directly.
 
     '''
 
     __slots__ = ()
-    _known_attrs = ('type', 'arch')
+    _known_attrs = ('type', 'arch', 'model')
 
     @property
     def info(self):
         '''All the available information from the configuration.
 
         :type: :class:`dict`
         '''
@@ -185,14 +185,20 @@
         self._resources = {r['name']: r['options'] for r in resources}
         self._processor = ProcessorInfo(processor)
         self._devices = [DeviceInfo(d) for d in devices]
         self._extras = extras
         self._features = features
         self._time_limit = time_limit
 
+        # Add implicit extras from scheduler and launcher
+        sched_name = self._sched_type.registered_name
+        launcher_name = self._launcher_type.registered_name
+        self._extras.setdefault('scheduler', sched_name)
+        self._extras.setdefault('launcher', launcher_name)
+
     @property
     def access(self):
         '''The scheduler options for accessing this system partition.
 
         :type: :class:`List[str]`
         '''
         return util.SequenceView(self._access)
@@ -534,19 +540,21 @@
                     features=site_config.get(f'environments/@{e}/features'),
                     prepare_cmds=site_config.get(
                         f'environments/@{e}/prepare_cmds'
                     ),
                     cc=site_config.get(f'environments/@{e}/cc'),
                     cxx=site_config.get(f'environments/@{e}/cxx'),
                     ftn=site_config.get(f'environments/@{e}/ftn'),
+                    nvcc=site_config.get(f'environments/@{e}/nvcc'),
                     cppflags=site_config.get(f'environments/@{e}/cppflags'),
                     cflags=site_config.get(f'environments/@{e}/cflags'),
                     cxxflags=site_config.get(f'environments/@{e}/cxxflags'),
                     fflags=site_config.get(f'environments/@{e}/fflags'),
-                    ldflags=site_config.get(f'environments/@{e}/ldflags')
+                    ldflags=site_config.get(f'environments/@{e}/ldflags'),
+                    resources=site_config.get(f'environments/@{e}/resources')
                 ) for e in site_config.get(f'{partid}/environs')
                 if any(re.match(pattern, e) for pattern in env_patt)
             ]
             partitions.append(
                 SystemPartition(
                     parent=site_config.get('systems/0/name'),
                     name=part_name,
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/variables.py` & `reframe_hpc-4.6.0/reframe/core/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,21 +34,24 @@
 
 class TestVar:
     '''Insert a new  test variable.
 
     Declaring a test variable through the :func:`variable` built-in allows for
     a more robust test implementation than if the variables were just defined
     as regular test attributes (e.g. ``self.a = 10``). Using variables
-    declared through the :func:`variable` built-in guarantees that these
-    regression test variables will not be redeclared by any child class, while
-    also ensuring that any values that may be assigned to such variables
-    comply with its original declaration. In essence, declaring test variables
-    with the :func:`variable` built-in removes any potential test errors that
-    might be caused by accidentally overriding a class attribute. See the
-    example below.
+    declared through the :func:`variable` built-in has a number of advantages:
+
+    1. Variables are type checked, so attempts to assign a value of a wrong
+       type will cause the test to fail.
+    2. You can set the values of variables from the command line using the
+       :option:`-S` option.
+    3. You can avoid variable redefinitions.
+    4. You can control whether a variable can be inherited multiple times.
+
+    The following is an example of type checking performed by variables:
 
     .. code:: python
 
        class Foo(rfm.RegressionTest):
            my_var = variable(int, value=8)
            not_a_var = my_var - 4
 
@@ -62,16 +65,16 @@
     Here, the argument ``value`` in the :func:`variable` built-in sets the
     default value for the variable. This value may be accessed directly from
     the class body, as long as it was assigned before either in the same class
     body or in the class body of a parent class. This behavior extends the
     standard Python data model, where a regular class attribute from a parent
     class is never available in the class body of a child class. Hence, using
     the :func:`variable` built-in enables us to directly use or modify any
-    variables that may have been declared upstream the class inheritance
-    chain, without altering their original value at the parent class level.
+    variables that may have been declared upstream the class hierarchy, without
+    altering their original value at the parent class level.
 
     .. code:: python
 
        class Bar(Foo):
            print(my_var) # prints 8
            # print(not_a_var) # This is standard Python and raises a NameError
 
@@ -147,66 +150,83 @@
     not been set. Conversely, a variable with a default value already assigned
     to it can be made required by assigning it the ``required`` keyword.
     However, this ``required`` keyword is only available in the class body.
 
     .. code:: python
 
        class MyRequiredTest(HelloTest):
-         what = required
+           what = required
 
 
     Running the above test will cause the :func:`set_exec_and_sanity` hook
     from :class:`EchoBaseTest` to throw an error indicating that the variable
     ``what`` has not been set.
 
     Finally, variables may alias each other. If a variable is an alias of
     another one it behaves in the exact same way as its target. If a change is
     made to the target variable, this is reflected to the alias and vice
     versa. However, alias variables are independently loggable: an alias may
     be logged but not its target and vice versa. Aliased variables are useful
     when you want to rename a variable and you want to keep the old one for
     compatibility reasons.
 
-    :param `types`: the supported types for the variable.
+    :param types: the supported types for the variable.
     :param value: the default value assigned to the variable. If no value is
         provided, the variable is set as ``required``.
     :param field: the field validator to be used for this variable. If no
         field argument is provided, it defaults to
         :attr:`reframe.core.fields.TypedField`. The provided field validator
         by this argument must derive from :attr:`reframe.core.fields.Field`.
     :param alias: the target variable if this variable is an alias. This must
         refer to an already declared variable and neither default value nor a
         field can be specified for an alias variable.
     :param loggable: Mark this variable as loggable. If :obj:`True`, this
         variable will become a log record attribute under the name
         ``check_NAME``, where ``NAME`` is the name of the variable (default
         :obj:`True`).
-    :param `kwargs`: keyword arguments to be forwarded to the constructor of
+    :param merge_func: Enable multiple inheritance for this variable by
+        defining a merge strategy of their default values.
+        (default: :obj:`None`).
+
+        This is a function that accepts two arguments of the type of the
+        variable and returns a new value of the same type. The new default
+        value of the variable will be determined as follows:
+
+        .. code-block:: python
+
+           current_value = merge_func(parent_value, current_value)
+
+        If ``current_value`` is undefined and ``parent_value`` is not, then
+        ``current_value = parent_value``. If ``parent_value`` is undefined or
+        both values are undefined, the variable remains intact.
+    :param kwargs: keyword arguments to be forwarded to the constructor of
         the field validator.
     :returns: A new test variable.
 
     .. versionadded:: 3.10.2
        The ``loggable`` argument is added.
 
     .. versionadded:: 4.0.0
        Alias variable are introduced.
 
     .. versionchanged:: 4.5
        Variables are now loggable by default.
 
+    .. versionchanged:: 4.6
+       The ``merge_func`` parameter is added.
     '''
 
     # NOTE: We can't use truly private fields in `__slots__`, because
     # `__setattr__()` will be called with their mangled name and we cannot
     # match them in the `__slots__` without making implementation-defined
     # assumptions about the mangled name. So we just add the `_p_` prefix for
     # to denote the "private" fields.
 
     __slots__ = ('_p_default_value', '_p_field',
-                 '_loggable', '_name', '_target', '_refs')
+                 '_loggable', '_name', '_target', '_refs', '_merge_fn')
 
     __mutable_props = ('_default_value',)
 
     def __init__(self, *args, **kwargs):
         alias = kwargs.pop('alias', None)
         if alias is not None and 'field' in kwargs:
             raise ValueError(f"'field' cannot be set for an alias variable")
@@ -220,14 +240,18 @@
 
         field_type = kwargs.pop('field', fields.TypedField)
         if alias is not None:
             self._p_default_value = alias._default_value
         else:
             self._p_default_value = kwargs.pop('value', Undefined)
 
+        self._merge_fn = kwargs.pop('merge_func', None)
+        if self._merge_fn is not None and not callable(self._merge_fn):
+            raise TypeError("'merge_func' is not callable")
+
         self._loggable = kwargs.pop('loggable', True)
         if not issubclass(field_type, fields.Field):
             raise TypeError(
                 f'field {field_type!r} is not derived from '
                 f'{fields.Field.__qualname__}'
             )
 
@@ -244,14 +268,15 @@
     def create_deprecated(cls, var, message,
                           kind=DEPRECATE_RDWR, from_version='0.0.0'):
         ret = TestVar.__new__(TestVar)
         ret._p_field = fields.DeprecatedField(var.field, message,
                                               kind, from_version)
         ret._p_default_value = var._default_value
         ret._loggable = var._loggable
+        ret._merge_fn = var._merge_fn
         ret._target = var._target
         ret._refs = var._refs
         if var.is_alias():
             # If we are deprecating an alias, we need to update the back
             # reference in the target variable with the deprecated one
             ret._target.replace_ref(var, ret)
 
@@ -277,40 +302,55 @@
 
     def is_deprecated(self):
         return isinstance(self._p_field, fields.DeprecatedField)
 
     def is_loggable(self):
         return self._loggable
 
+    def is_mergeable(self):
+        return self._merge_fn is not None
+
     def is_defined(self):
         return self._default_value is not Undefined
 
     def is_alias(self):
         return self._target is not None
 
     def undefine(self):
         self._default_value = Undefined
 
     def define(self, value):
         self._warn_deprecation(DEPRECATE_WR)
         self._default_value = value
 
+    def update_from(self, other):
+        if self.is_defined() and other.is_defined():
+            self._default_value = self._merge_fn(self._default_value,
+                                                 other._default_value)
+        elif not self.is_defined() and other.is_defined():
+            self._default_value = other._default_value
+        else:
+            '''If other is undefined or both are undefined,
+            we keep our value'''
+
     @property
     def _default_value(self):
         if self.is_alias():
             return self._target._default_value
         else:
             return self._p_default_value
 
     @_default_value.setter
     def _default_value(self, value):
         if self.is_alias():
             self._target._default_value = value
-        else:
+        elif value is Undefined:
             self._p_default_value = value
+        else:
+            self._p_default_value = self._p_field.__set__(None, value)
 
     @property
     def default_value(self):
         # Variables must be returned by-value to prevent an instance from
         # modifying the class variable space.
         self._check_is_defined()
         self._warn_deprecation(DEPRECATE_RD)
@@ -344,14 +384,26 @@
         else:
             self._p_field._target_field = new_target._field
 
         self._target = new_target
 
     def __set_name__(self, owner, name):
         self._name = name
+        self._p_field.__set_name__(owner, name)
+
+        # Type check and convert the variable's value if defined
+        if self.is_defined():
+            if isinstance(self._p_default_value, TestVar):
+                # Treat shadow variables
+                value = self._p_default_value._p_default_value
+            else:
+                value = self._p_default_value
+
+            with suppress_deprecations():
+                self._p_default_value = self._p_field.__set__(None, value)
 
     def __setattr__(self, name, value):
         '''Set any additional variable attribute into the default value.'''
         if name in self.__slots__ or name in self.__mutable_props:
             super().__setattr__(name, value)
         else:
             setattr(self._default_value, name, value)
@@ -774,23 +826,25 @@
     def join(self, other, cls):
         '''Join an existing VarSpace into the current one.
 
         :param other: instance of the VarSpace class.
         :param cls: the target class.
         '''
         for key, var in other.items():
-            # Make doubly declared vars illegal. Note that this will be
-            # triggered when inheriting from multiple RegressionTest classes.
             if key in self.vars:
-                raise ReframeSyntaxError(
-                    f'variable {key!r} is declared in more than one of the '
-                    f'parent classes of class {cls.__qualname__!r}'
-                )
-
-            self.vars[key] = copy.deepcopy(var)
+                this_var = self.vars[key]
+                if this_var.is_mergeable():
+                    this_var.update_from(var)
+                else:
+                    raise ReframeSyntaxError(
+                        f'multiple inheritance is disabled for variable '
+                        f'{key!r}; consider declaring it with a `merge_func`'
+                    )
+            else:
+                self.vars[key] = copy.deepcopy(var)
 
         # Inherited variables are copied in the current namespace, so we need
         # to update any aliases to point to the current namespace copies
         for var in self.vars.values():
             if var.is_alias():
                 var.reset_target(self.vars[var.target.name])
 
@@ -874,20 +928,24 @@
         # value; deprecations have been checked already during the class
         # construction, so we don't want to trigger them also here.
         with suppress_deprecations():
             self._inject(obj, cls)
 
     def _inject(self, obj, cls):
         for name, var in self.items():
+            # Replace the variable with its descriptor
             setattr(cls, name, var.field)
             getattr(cls, name).__set_name__(obj, name)
 
             # If the var is defined, set its value
             if var.is_defined():
-                setattr(obj, name, var.default_value)
+                # Variable's value is already validated and converted,
+                # so we bypass completely the descriptor logic by not calling
+                # `setattr()`
+                obj.__dict__[name] = var.default_value
 
             # Track the variables that have been injected.
             self._injected_vars.add(name)
 
     @property
     def vars(self):
         return self._namespace
```

### Comparing `ReFrame-HPC-4.5.2/reframe/core/warnings.py` & `reframe_hpc-4.6.0/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/argparse.py` & `reframe_hpc-4.6.0/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/autodetect.py` & `reframe_hpc-4.6.0/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/ci.py` & `reframe_hpc-4.6.0/reframe/frontend/ci.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/cli.py` & `reframe_hpc-4.6.0/reframe/frontend/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,16 +152,17 @@
             rec['display_name'] = tc.check.display_name
             rec['pipeline_hooks'] = {}
             rec['perf_variables'] = list(rec['perf_variables'].keys())
             rec['prefix'] = tc.check.prefix
             rec['variant_num'] = tc.check.variant_num
             for stage, hooks in tc.check.pipeline_hooks().items():
                 for hk in hooks:
-                    rec['pipeline_hooks'].setdefault(stage, [])
-                    rec['pipeline_hooks'][stage].append(hk.__name__)
+                    if hk.__name__ not in tc.check.disabled_hooks:
+                        rec['pipeline_hooks'].setdefault(stage, [])
+                        rec['pipeline_hooks'][stage].append(hk.__name__)
 
             for attr in list(rec.keys()):
                 if attr == '__rfm_class__':
                     rec['@class'] = rec[attr]
                     del rec[attr]
                 elif attr == '__rfm_file__':
                     rec['@file'] = rec[attr]
@@ -509,15 +510,15 @@
         dest='unload_modules', default=[],
         help='Unload module MOD before running any regression check',
         envvar='RFM_UNLOAD_MODULES ,', configvar='general/unload_modules'
     )
 
     # Test generation options
     testgen_options.add_argument(
-        '--distribute', action='store', metavar='{all|STATE}',
+        '--distribute', action='store', metavar='{all|avail|STATE}',
         nargs='?', const='idle',
         help=('Distribute the selected single-node jobs on every node that'
               'is in STATE (default: "idle"')
     )
     testgen_options.add_argument(
         '-P', '--parameterize', action='append', metavar='VAR:VAL0,VAL1,...',
         default=[], help='Parameterize a test on a set of variables'
@@ -1146,15 +1147,16 @@
                     "a non-negative integer"
                 ) from None
 
             testcases_all = repeat_tests(testcases, num_repeats)
             testcases = testcases_all
 
         if options.distribute:
-            node_map = getallnodes(options.distribute, parsed_job_options)
+            node_map = getallnodes(options.distribute.lower(),
+                                   parsed_job_options)
 
             # Remove the job options that begin with '--nodelist' and '-w', so
             # that they do not override those set from the distribute feature.
             #
             # NOTE: This is Slurm-specific. When support of distributing tests
             # is added to other scheduler backends, this needs to be updated,
             # too.
```

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/dependencies.py` & `reframe_hpc-4.6.0/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/executors/__init__.py` & `reframe_hpc-4.6.0/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/executors/policies.py` & `reframe_hpc-4.6.0/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/filters.py` & `reframe_hpc-4.6.0/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/loader.py` & `reframe_hpc-4.6.0/reframe/frontend/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,23 @@
         if not self._validate_source(filename):
             return []
 
         try:
             dirname = os.path.dirname(filename)
             with osext.change_dir(dirname):
                 with util.temp_sys_path(dirname):
+                    if os.path.exists(os.path.join(dirname, '__init__.py')):
+                        # If the containing directory is a package,
+                        # import it, too.
+                        parent = util.import_module_from_file(dirname).__name__
+                    else:
+                        parent = None
+
                     return self.load_from_module(
-                        util.import_module_from_file(filename, force)
+                        util.import_module_from_file(filename, force, parent)
                     )
         except Exception:
             exc_info = sys.exc_info()
             if not is_severe(*exc_info):
                 # Simply skip the file in this case
                 getlogger().warning(
                     f"skipping test file {filename!r}: {what(*exc_info)} "
```

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/printer.py` & `reframe_hpc-4.6.0/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/runreport.py` & `reframe_hpc-4.6.0/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/statistics.py` & `reframe_hpc-4.6.0/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/frontend/testgenerators.py` & `reframe_hpc-4.6.0/reframe/frontend/testgenerators.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import reframe.core.runtime as runtime
 import reframe.utility as util
 
 from reframe.core.decorators import TestRegistry
 from reframe.core.fields import make_convertible
 from reframe.core.logging import getlogger, time_function
 from reframe.core.meta import make_test
-from reframe.core.schedulers import Job
+from reframe.core.schedulers import Job, filter_nodes_by_state
 from reframe.frontend.executors import generate_testcases
 
 
 @time_function
-def getallnodes(state='all', jobs_cli_options=None):
+def getallnodes(state, jobs_cli_options=None):
     rt = runtime.runtime()
     nodes = {}
     for part in rt.system.partitions:
         # This job will not be submitted, it's used only to filter
         # the nodes based on the partition configuration
         dummy_job = Job.create(part.scheduler,
                                part.launcher_type(),
@@ -32,22 +32,15 @@
         available_nodes = part.scheduler.allnodes()
         available_nodes = part.scheduler.filternodes(dummy_job,
                                                      available_nodes)
         getlogger().debug(
             f'Total available nodes for {part.name}: {len(available_nodes)}'
         )
 
-        if state.casefold() != 'all':
-            available_nodes = {n for n in available_nodes
-                               if n.in_state(state)}
-            getlogger().debug(
-                f'[F] Selecting nodes in state {state!r}: '
-                f'available nodes now: {len(available_nodes)}'
-            )
-
+        available_nodes = filter_nodes_by_state(available_nodes, state)
         nodes[part.fullname] = [n.name for n in available_nodes]
 
     return nodes
 
 
 def _generate_tests(testcases, gen_fn):
     tmp_registry = TestRegistry()
```

### Comparing `ReFrame-HPC-4.5.2/reframe/schemas/config.json` & `reframe_hpc-4.6.0/reframe/schemas/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992675523636172%*

 * *Differences: {"'defaults'": "{'environments/nvcc': 'nvcc'}",*

 * * "'defs'": "{'processor_info': {'properties': {'vendor': OrderedDict([('type', 'string')]), "*

 * *           "'model': OrderedDict([('type', 'string')]), 'platform': OrderedDict([('type', "*

 * *           "'string')])}}, 'device_info': {'properties': {'model': OrderedDict([('type', "*

 * *           "'string')])}}}",*

 * * "'properties'": "{'environments': {'items': {'properties': {'nvcc': OrderedDict([('type', "*

 * *                 "'string')]), 'resources': OrderedDict([('type', […]*

```diff
@@ -14,14 +14,15 @@
         "environments/env_vars": [],
         "environments/extras": {},
         "environments/features": [],
         "environments/fflags": [],
         "environments/ftn": "ftn",
         "environments/ldflags": [],
         "environments/modules": [],
+        "environments/nvcc": "nvcc",
         "environments/target_systems": [
             "*"
         ],
         "environments/variables": [],
         "general/check_search_path": [
             "${RFM_INSTALL_PREFIX}/checks/"
         ],
@@ -129,14 +130,17 @@
             "type": "string"
         },
         "device_info": {
             "properties": {
                 "arch": {
                     "type": "string"
                 },
+                "model": {
+                    "type": "string"
+                },
                 "num_devices": {
                     "type": "number"
                 },
                 "type": {
                     "type": "string"
                 }
             },
@@ -346,28 +350,37 @@
         },
         "processor_info": {
             "additionalProperties": false,
             "properties": {
                 "arch": {
                     "type": "string"
                 },
+                "model": {
+                    "type": "string"
+                },
                 "num_cpus": {
                     "type": "number"
                 },
                 "num_cpus_per_core": {
                     "type": "number"
                 },
                 "num_cpus_per_socket": {
                     "type": "number"
                 },
                 "num_sockets": {
                     "type": "number"
                 },
+                "platform": {
+                    "type": "string"
+                },
                 "topology": {
                     "$ref": "#/defs/topology_info"
+                },
+                "vendor": {
+                    "type": "string"
                 }
             },
             "type": "object"
         },
         "sched_options": {
             "properties": {
                 "hosts": {
@@ -587,20 +600,33 @@
                     },
                     "modules": {
                         "$ref": "#/defs/modules_list"
                     },
                     "name": {
                         "$ref": "#/defs/alphanum_ext_string"
                     },
+                    "nvcc": {
+                        "type": "string"
+                    },
                     "prepare_cmds": {
                         "items": {
                             "type": "string"
                         },
                         "type": "array"
                     },
+                    "resources": {
+                        "additionalProperties": {
+                            "additionalProperties": true,
+                            "type": "object"
+                        },
+                        "propertyNames": {
+                            "pattern": "^[a-zA-Z_][a-zA-Z0-9_]*$"
+                        },
+                        "type": "object"
+                    },
                     "target_systems": {
                         "$ref": "#/defs/system_ref"
                     },
                     "variables": {
                         "$ref": "#/defs/envvar_list"
                     }
                 },
```

### Comparing `ReFrame-HPC-4.5.2/reframe/schemas/junit.xsd` & `reframe_hpc-4.6.0/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/schemas/runreport.json` & `reframe_hpc-4.6.0/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/__init__.py` & `reframe_hpc-4.6.0/reframe/utility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,30 +66,37 @@
 
     module = importlib.util.module_from_spec(spec)
     sys.modules[module_name] = module
     spec.loader.exec_module(module)
     return module
 
 
-def import_module_from_file(filename, force=False):
+def import_module_from_file(filename, force=False, parent=None):
     '''Import module from file.
 
     If the file location refers to a directory, the contained ``__init__.py``
     will be loaded. If the filename resolves to a location that is within the
     current working directory, a module name will be derived from the supplied
     file name and Python's :func:`importlib.import_module` will be invoked to
     actually load the module. If the file location refers to a path outside
     the current working directory, then the module will be loaded directly
     from the file, but it will be assigned a mangled name in
     :obj:`sys.modules`, to avoid clashes with other modules loaded using the
     standard import mechanism.
 
     :arg filename: The path to the filename of a Python module.
     :arg force: Force reload of module in case it is already loaded.
+    :arg parent: The name of the parent module of the one that will be loaded.
+        This will essentially prefix the module of the newly loaded module with
+        ``parent`` so that Python would be able to resolve relative imports in
+        the module file.
     :returns: The loaded Python module.
+
+    .. versionchanged:: 4.6
+       The ``parent`` argument is added.
     '''
 
     # Expand and sanitize filename
     filename = os.path.abspath(os.path.expandvars(filename))
     if os.path.isdir(filename):
         filename = os.path.join(filename, '__init__.py')
 
@@ -99,14 +106,17 @@
     if rel_filename.startswith('..'):
         # We cannot use the standard Python import mechanism here, because the
         # module to import is outside the top-level package. We also mangle
         # the name that we assign to the module, in order to avoid clashes
         # with other modules loaded with a standard `import` or with multiple
         # test files with the same name that reside in different directories.
         module_hash = sha256(filename.encode('utf-8')).hexdigest()[:8]
+        if parent:
+            module_name = f'{parent}.{module_name}'
+
         module_name = f'{module_name}@{module_hash}'
         return _do_import_module_from_file(filename, module_name)
 
     # Extract module name if `filename` is under `site-packages/` or the
     # Debian specific `dist-packages/`
     site_packages = re.compile(r'.*(site|dist)-packages/(?P<rel_filename>.+)')
     match = site_packages.search(filename)
```

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/color.py` & `reframe_hpc-4.6.0/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/cpuinfo.py` & `reframe_hpc-4.6.0/reframe/utility/cpuinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import archspec.cpu
 import contextlib
 import glob
 import os
+import platform
 import re
 
 import reframe.utility.osext as osext
 from reframe.core.exceptions import SpawnedProcessError
 
 
 def _bits_from_str(mask_s):
@@ -277,15 +278,19 @@
         cpuinfo['topology']['caches'].append(t)
 
     return cpuinfo
 
 
 def cpuinfo():
     ret = {
-        'arch': archspec.cpu.host().name
+        'arch': archspec.cpu.host().name,
+        'vendor': archspec.cpu.host().vendor,
+        'model': archspec.cpu.detect.raw_info_dictionary().get('model name',
+                                                               'N/A'),
+        'platform': platform.machine()
     }
 
     # Try first to get information from the filesystem
     if os.path.isdir('/sys'):
         topology = _sysfs_topo()
     else:
         # Try with the `sysctl` command
```

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/jsonext.py` & `reframe_hpc-4.6.0/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/osext.py` & `reframe_hpc-4.6.0/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/profile.py` & `reframe_hpc-4.6.0/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/sanity.py` & `reframe_hpc-4.6.0/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/typecheck.py` & `reframe_hpc-4.6.0/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/udeps.py` & `reframe_hpc-4.6.0/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/reframe/utility/versioning.py` & `reframe_hpc-4.6.0/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.5.2/setup.cfg` & `reframe_hpc-4.6.0/setup.cfg`

 * *Files identical despite different names*

