# Comparing `tmp/jztools-0.1.3.tar.gz` & `tmp/jztools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jztools-0.1.3.tar", last modified: Fri Apr 19 05:53:48 2024, max compression
+gzip compressed data, was "jztools-0.1.5.tar", last modified: Sat Apr 20 16:28:38 2024, max compression
```

## Comparing `jztools-0.1.3.tar` & `jztools-0.1.5.tar`

### file list

```diff
@@ -1,71 +1,166 @@
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.067010 jztools-0.1.3/
--rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-18 02:46:37.000000 jztools-0.1.3/LICENSE
--rw-r--r--   0 jazs       (501) staff       (20)      550 2024-04-19 05:53:48.066825 jztools-0.1.3/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)      221 2024-04-18 18:21:34.000000 jztools-0.1.3/README.md
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.057075 jztools-0.1.3/jztools/
--rw-r--r--   0 jazs       (501) staff       (20)       39 2024-04-17 23:46:09.000000 jztools-0.1.3/jztools/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     8144 2024-04-18 22:33:24.000000 jztools-0.1.3/jztools/logging.py
--rw-r--r--   0 jazs       (501) staff       (20)     7125 2024-04-18 22:28:25.000000 jztools-0.1.3/jztools/numpy.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.059492 jztools-0.1.3/jztools/parallelization/
--rw-r--r--   0 jazs       (501) staff       (20)      622 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     3975 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/_base.py
--rw-r--r--   0 jazs       (501) staff       (20)     4929 2024-04-18 22:28:25.000000 jztools-0.1.3/jztools/parallelization/_outsourced_iterable_base.py
--rw-r--r--   0 jazs       (501) staff       (20)     1563 2024-04-18 22:28:25.000000 jztools-0.1.3/jztools/parallelization/mock.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.060291 jztools-0.1.3/jztools/parallelization/multiprocessing/
--rw-r--r--   0 jazs       (501) staff       (20)      294 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/multiprocessing/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      380 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/multiprocessing/handlers.py
--rw-r--r--   0 jazs       (501) staff       (20)     1236 2024-04-18 22:28:25.000000 jztools-0.1.3/jztools/parallelization/multiprocessing/outsourced_iterable.py
--rw-r--r--   0 jazs       (501) staff       (20)     1067 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/multiprocessing/process_with_info.py
--rw-r--r--   0 jazs       (501) staff       (20)     1224 2024-04-18 22:29:44.000000 jztools-0.1.3/jztools/parallelization/outsourced_callable_base.py
--rw-r--r--   0 jazs       (501) staff       (20)     4461 2024-04-18 22:28:24.000000 jztools-0.1.3/jztools/parallelization/selector.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.061380 jztools-0.1.3/jztools/parallelization/threading/
--rw-r--r--   0 jazs       (501) staff       (20)      441 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/threading/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     1935 2024-04-19 05:02:52.000000 jztools-0.1.3/jztools/parallelization/threading/general.py
--rw-r--r--   0 jazs       (501) staff       (20)     2417 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/threading/lock.py
--rw-r--r--   0 jazs       (501) staff       (20)      145 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/threading/outsourced_callable.py
--rw-r--r--   0 jazs       (501) staff       (20)      250 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/threading/outsourced_iterable.py
--rw-r--r--   0 jazs       (501) staff       (20)     2460 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/threading/queue.py
--rw-r--r--   0 jazs       (501) staff       (20)     1349 2024-04-18 22:28:24.000000 jztools-0.1.3/jztools/parallelization/threading/util.py
--rw-r--r--   0 jazs       (501) staff       (20)     6522 2024-04-14 20:09:15.000000 jztools-0.1.3/jztools/parallelization/utils.py
--rw-r--r--   0 jazs       (501) staff       (20)    13782 2024-04-19 04:59:51.000000 jztools-0.1.3/jztools/py.py
--rw-r--r--   0 jazs       (501) staff       (20)     4452 2024-04-17 23:46:09.000000 jztools-0.1.3/jztools/reference_sequence.py
--rw-r--r--   0 jazs       (501) staff       (20)     3688 2024-04-17 23:46:09.000000 jztools-0.1.3/jztools/rentemp.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.062353 jztools-0.1.3/jztools/serializer/
--rw-r--r--   0 jazs       (501) staff       (20)      649 2024-04-18 22:28:24.000000 jztools-0.1.3/jztools/serializer/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      905 2024-03-31 00:34:30.000000 jztools-0.1.3/jztools/serializer/abstract_type_serializer.py
--rw-r--r--   0 jazs       (501) staff       (20)     1326 2024-04-18 22:28:24.000000 jztools-0.1.3/jztools/serializer/extensions.py
--rw-r--r--   0 jazs       (501) staff       (20)     6779 2024-04-18 22:28:24.000000 jztools-0.1.3/jztools/serializer/serializer.py
--rw-r--r--   0 jazs       (501) staff       (20)     7078 2024-04-17 23:46:09.000000 jztools-0.1.3/jztools/validation.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.066614 jztools-0.1.3/jztools.egg-info/
--rw-r--r--   0 jazs       (501) staff       (20)      550 2024-04-19 05:53:48.000000 jztools-0.1.3/jztools.egg-info/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)     2135 2024-04-19 05:53:48.000000 jztools-0.1.3/jztools.egg-info/SOURCES.txt
--rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-19 05:53:48.000000 jztools-0.1.3/jztools.egg-info/dependency_links.txt
--rw-r--r--   0 jazs       (501) staff       (20)       39 2024-04-19 05:53:48.000000 jztools-0.1.3/jztools.egg-info/requires.txt
--rw-r--r--   0 jazs       (501) staff       (20)       14 2024-04-19 05:53:48.000000 jztools-0.1.3/jztools.egg-info/top_level.txt
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.062645 jztools-0.1.3/scripts/
--rw-r--r--   0 jazs       (501) staff       (20)     1259 2024-04-18 19:16:42.000000 jztools-0.1.3/scripts/test_install
--rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-19 05:53:48.067058 jztools-0.1.3/setup.cfg
--rw-r--r--   0 jazs       (501) staff       (20)      555 2024-04-18 22:32:45.000000 jztools-0.1.3/setup.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.054420 jztools-0.1.3/tests/
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.064080 jztools-0.1.3/tests/jztools/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 23:46:09.000000 jztools-0.1.3/tests/jztools/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     3211 2024-04-19 04:30:13.000000 jztools-0.1.3/tests/jztools/logging.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.065086 jztools-0.1.3/tests/jztools/parallelization/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-03-31 00:34:30.000000 jztools-0.1.3/tests/jztools/parallelization/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     1028 2024-04-18 22:28:24.000000 jztools-0.1.3/tests/jztools/parallelization/_outsourced_iterable_base.py
--rw-r--r--   0 jazs       (501) staff       (20)     1727 2024-04-19 04:39:04.000000 jztools-0.1.3/tests/jztools/parallelization/_parallelizer.py
--rw-r--r--   0 jazs       (501) staff       (20)      218 2024-04-18 22:28:24.000000 jztools-0.1.3/tests/jztools/parallelization/mock.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.065640 jztools-0.1.3/tests/jztools/parallelization/multiprocessing/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-14 20:09:15.000000 jztools-0.1.3/tests/jztools/parallelization/multiprocessing/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      312 2024-04-18 22:28:23.000000 jztools-0.1.3/tests/jztools/parallelization/multiprocessing/outsourced_iterable.py
--rw-r--r--   0 jazs       (501) staff       (20)      538 2024-04-18 22:28:23.000000 jztools-0.1.3/tests/jztools/parallelization/multiprocessing/process_with_info.py
--rw-r--r--   0 jazs       (501) staff       (20)     4140 2024-04-19 04:46:05.000000 jztools-0.1.3/tests/jztools/parallelization/selector.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-19 05:53:48.066352 jztools-0.1.3/tests/jztools/parallelization/threading/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-14 20:09:15.000000 jztools-0.1.3/tests/jztools/parallelization/threading/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     5255 2024-04-18 22:28:23.000000 jztools-0.1.3/tests/jztools/parallelization/threading/general.py
--rw-r--r--   0 jazs       (501) staff       (20)      715 2024-04-18 22:28:23.000000 jztools-0.1.3/tests/jztools/parallelization/threading/outsourced_callable.py
--rw-r--r--   0 jazs       (501) staff       (20)      307 2024-04-18 22:20:22.000000 jztools-0.1.3/tests/jztools/parallelization/threading/outsourced_iterable.py
--rw-r--r--   0 jazs       (501) staff       (20)     5892 2024-04-17 23:46:09.000000 jztools-0.1.3/tests/jztools/py.py
--rw-r--r--   0 jazs       (501) staff       (20)      135 2024-04-18 05:42:40.000000 jztools-0.1.3/tests/jztools/py_support.py
--rw-r--r--   0 jazs       (501) staff       (20)     3433 2024-04-17 23:46:09.000000 jztools-0.1.3/tests/jztools/reference_sequence.py
--rw-r--r--   0 jazs       (501) staff       (20)     3051 2024-04-17 23:46:09.000000 jztools-0.1.3/tests/jztools/validation.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.863589 jztools-0.1.5/
+-rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-18 02:46:37.000000 jztools-0.1.5/LICENSE
+-rw-r--r--   0 jazs       (501) staff       (20)      670 2024-04-20 16:28:38.863392 jztools-0.1.5/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)      221 2024-04-18 18:21:34.000000 jztools-0.1.5/README.md
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.848518 jztools-0.1.5/jztools/
+-rw-r--r--   0 jazs       (501) staff       (20)       39 2024-04-19 21:56:35.000000 jztools-0.1.5/jztools/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1184 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/algos.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8417 2024-04-19 22:01:44.000000 jztools-0.1.5/jztools/autonamed_pattern.py
+-rw-r--r--   0 jazs       (501) staff       (20)      418 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/colorama.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2943 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/contextlib.py
+-rw-r--r--   0 jazs       (501) staff       (20)      932 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/datetime.py
+-rw-r--r--   0 jazs       (501) staff       (20)     9342 2024-04-19 22:01:44.000000 jztools-0.1.5/jztools/datetime64.py
+-rw-r--r--   0 jazs       (501) staff       (20)     9908 2024-04-19 22:01:44.000000 jztools-0.1.5/jztools/filelock.py
+-rw-r--r--   0 jazs       (501) staff       (20)      653 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/files.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1394 2024-04-19 22:01:44.000000 jztools-0.1.5/jztools/freezegun.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1072 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/general.py
+-rw-r--r--   0 jazs       (501) staff       (20)      717 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/gunicorn.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2418 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/humanize.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1110 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/json.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8144 2024-04-18 22:33:24.000000 jztools-0.1.5/jztools/logging.py
+-rw-r--r--   0 jazs       (501) staff       (20)      105 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/mplib.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.849317 jztools-0.1.5/jztools/nnets/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/nnets/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1006 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/nnets/numtor.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7125 2024-04-18 22:28:25.000000 jztools-0.1.5/jztools/numpy.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.850875 jztools-0.1.5/jztools/object_recorder/
+-rw-r--r--   0 jazs       (501) staff       (20)     5643 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/object_recorder/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      493 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/object_recorder/_testing_utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3520 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/object_recorder/call_unordered.py
+-rw-r--r--   0 jazs       (501) staff       (20)      290 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/object_recorder/example.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.851206 jztools-0.1.5/jztools/object_recorder/freeze_call_times/
+-rw-r--r--   0 jazs       (501) staff       (20)       82 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/object_recorder/freeze_call_times/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8067 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/object_recorder/freeze_call_times/freeze_call_times.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2084 2024-04-19 22:01:43.000000 jztools-0.1.5/jztools/object_recorder/freeze_call_times/stack.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1325 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/global_time.py
+-rw-r--r--   0 jazs       (501) staff       (20)    11590 2024-04-19 22:29:13.000000 jztools-0.1.5/jztools/object_recorder/object_recorder.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4559 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/rec_obj_factory.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2430 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/rec_obj_factory__call_unordered.py
+-rw-r--r--   0 jazs       (501) staff       (20)      235 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/rec_obj_factory__defs.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3300 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/record_instances.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7100 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/recorded_attributes.py
+-rw-r--r--   0 jazs       (501) staff       (20)    22097 2024-04-19 22:29:25.000000 jztools-0.1.5/jztools/object_recorder/recording_switch_utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1886 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/object_recorder/replicate.py
+-rw-r--r--   0 jazs       (501) staff       (20)      659 2024-04-19 22:29:01.000000 jztools-0.1.5/jztools/object_recorder/utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)      222 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/os.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.851401 jztools-0.1.5/jztools/pacers/
+-rw-r--r--   0 jazs       (501) staff       (20)       93 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/pacers/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2442 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/pacers/pacers.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.852830 jztools-0.1.5/jztools/parallelization/
+-rw-r--r--   0 jazs       (501) staff       (20)      622 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3975 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/_base.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4929 2024-04-18 22:28:25.000000 jztools-0.1.5/jztools/parallelization/_outsourced_iterable_base.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1563 2024-04-18 22:28:25.000000 jztools-0.1.5/jztools/parallelization/mock.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.853511 jztools-0.1.5/jztools/parallelization/multiprocessing/
+-rw-r--r--   0 jazs       (501) staff       (20)      294 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/multiprocessing/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      380 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/multiprocessing/handlers.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1236 2024-04-18 22:28:25.000000 jztools-0.1.5/jztools/parallelization/multiprocessing/outsourced_iterable.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1067 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/multiprocessing/process_with_info.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1224 2024-04-18 22:29:44.000000 jztools-0.1.5/jztools/parallelization/outsourced_callable_base.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4461 2024-04-18 22:28:24.000000 jztools-0.1.5/jztools/parallelization/selector.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.854423 jztools-0.1.5/jztools/parallelization/threading/
+-rw-r--r--   0 jazs       (501) staff       (20)      441 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/threading/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1935 2024-04-19 05:02:52.000000 jztools-0.1.5/jztools/parallelization/threading/general.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2417 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/threading/lock.py
+-rw-r--r--   0 jazs       (501) staff       (20)      145 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/threading/outsourced_callable.py
+-rw-r--r--   0 jazs       (501) staff       (20)      250 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/threading/outsourced_iterable.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2460 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/threading/queue.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1349 2024-04-18 22:28:24.000000 jztools-0.1.5/jztools/parallelization/threading/util.py
+-rw-r--r--   0 jazs       (501) staff       (20)     6522 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/parallelization/utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1102 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/profile.py
+-rw-r--r--   0 jazs       (501) staff       (20)    10505 2024-04-19 18:54:25.000000 jztools-0.1.5/jztools/profiling.py
+-rw-r--r--   0 jazs       (501) staff       (20)    13785 2024-04-19 21:52:19.000000 jztools-0.1.5/jztools/py.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4452 2024-04-19 21:59:01.000000 jztools-0.1.5/jztools/reference_sequence.py
+-rw-r--r--   0 jazs       (501) staff       (20)      146 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/reference_sequence2.py
+-rw-r--r--   0 jazs       (501) staff       (20)    11213 2024-04-19 22:01:42.000000 jztools-0.1.5/jztools/reference_sequence_v0.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3688 2024-04-19 21:52:50.000000 jztools-0.1.5/jztools/rentemp.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.855305 jztools-0.1.5/jztools/serializer/
+-rw-r--r--   0 jazs       (501) staff       (20)      649 2024-04-18 22:28:24.000000 jztools-0.1.5/jztools/serializer/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      905 2024-03-31 00:34:30.000000 jztools-0.1.5/jztools/serializer/abstract_type_serializer.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1326 2024-04-18 22:28:24.000000 jztools-0.1.5/jztools/serializer/extensions.py
+-rw-r--r--   0 jazs       (501) staff       (20)     6779 2024-04-18 22:28:24.000000 jztools-0.1.5/jztools/serializer/serializer.py
+-rw-r--r--   0 jazs       (501) staff       (20)    12214 2024-04-19 22:01:41.000000 jztools-0.1.5/jztools/shared_memory.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3629 2024-04-19 21:37:25.000000 jztools-0.1.5/jztools/slice_sequence.py
+-rw-r--r--   0 jazs       (501) staff       (20)      672 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/socket.py
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:50:17.000000 jztools-0.1.5/jztools/sphinx.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.856007 jztools-0.1.5/jztools/sqlalchemy/
+-rw-r--r--   0 jazs       (501) staff       (20)       97 2024-03-31 00:34:30.000000 jztools-0.1.5/jztools/sqlalchemy/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1198 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/sqlalchemy/deprecated.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8814 2024-04-19 21:35:20.000000 jztools-0.1.5/jztools/sqlalchemy/threaded_insert_cache.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4003 2024-04-19 23:07:07.000000 jztools-0.1.5/jztools/sqlalchemy/types.py
+-rw-r--r--   0 jazs       (501) staff       (20)      466 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/sqlalchemy/utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2378 2024-04-19 22:01:41.000000 jztools-0.1.5/jztools/timer.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.856413 jztools-0.1.5/jztools/unittest/
+-rw-r--r--   0 jazs       (501) staff       (20)       61 2024-03-31 00:34:30.000000 jztools-0.1.5/jztools/unittest/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      345 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/unittest/decorators.py
+-rw-r--r--   0 jazs       (501) staff       (20)      815 2024-04-19 18:54:25.000000 jztools-0.1.5/jztools/unittest/speed.py
+-rw-r--r--   0 jazs       (501) staff       (20)      725 2024-04-14 20:09:15.000000 jztools-0.1.5/jztools/unittest/utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7078 2024-04-19 21:52:54.000000 jztools-0.1.5/jztools/validation.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.863159 jztools-0.1.5/jztools.egg-info/
+-rw-r--r--   0 jazs       (501) staff       (20)      670 2024-04-20 16:28:38.000000 jztools-0.1.5/jztools.egg-info/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)     4862 2024-04-20 16:28:38.000000 jztools-0.1.5/jztools.egg-info/SOURCES.txt
+-rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-20 16:28:38.000000 jztools-0.1.5/jztools.egg-info/dependency_links.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       84 2024-04-20 16:28:38.000000 jztools-0.1.5/jztools.egg-info/requires.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       14 2024-04-20 16:28:38.000000 jztools-0.1.5/jztools.egg-info/top_level.txt
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.856732 jztools-0.1.5/scripts/
+-rw-r--r--   0 jazs       (501) staff       (20)     1348 2024-04-20 15:58:40.000000 jztools-0.1.5/scripts/isorun
+-rw-r--r--   0 jazs       (501) staff       (20)     1289 2024-04-20 15:41:33.000000 jztools-0.1.5/scripts/isotest
+-rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-20 16:28:38.863629 jztools-0.1.5/setup.cfg
+-rw-r--r--   0 jazs       (501) staff       (20)      715 2024-04-20 16:03:55.000000 jztools-0.1.5/setup.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.842448 jztools-0.1.5/tests/
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.859298 jztools-0.1.5/tests/jztools/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:51:24.000000 jztools-0.1.5/tests/jztools/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1166 2024-04-19 22:01:41.000000 jztools-0.1.5/tests/jztools/algos.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5389 2024-04-19 22:01:41.000000 jztools-0.1.5/tests/jztools/autonamed_pattern.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5094 2024-04-19 22:01:41.000000 jztools-0.1.5/tests/jztools/datetime64.py
+-rw-r--r--   0 jazs       (501) staff       (20)    12593 2024-04-19 22:01:41.000000 jztools-0.1.5/tests/jztools/filelock.py
+-rw-r--r--   0 jazs       (501) staff       (20)      558 2024-04-19 22:01:41.000000 jztools-0.1.5/tests/jztools/freezegun.py
+-rw-r--r--   0 jazs       (501) staff       (20)      224 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/general.py
+-rw-r--r--   0 jazs       (501) staff       (20)      399 2024-04-19 21:46:05.000000 jztools-0.1.5/tests/jztools/humanize.py
+-rw-r--r--   0 jazs       (501) staff       (20)      540 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/json.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3211 2024-04-19 04:30:13.000000 jztools-0.1.5/tests/jztools/logging.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.859506 jztools-0.1.5/tests/jztools/nnets/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:51:24.000000 jztools-0.1.5/tests/jztools/nnets/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3137 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/numpy.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.860092 jztools-0.1.5/tests/jztools/object_recorder/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:51:24.000000 jztools-0.1.5/tests/jztools/object_recorder/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1012 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/object_recorder/call_unordered.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.860311 jztools-0.1.5/tests/jztools/object_recorder/freeze_call_times/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:51:24.000000 jztools-0.1.5/tests/jztools/object_recorder/freeze_call_times/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2306 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/object_recorder/freeze_call_times/freeze_call_times.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3916 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/object_recorder/init_doc.py
+-rw-r--r--   0 jazs       (501) staff       (20)     6595 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/object_recorder/object_recorder.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3295 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/object_recorder/record_instances.py
+-rw-r--r--   0 jazs       (501) staff       (20)    12208 2024-04-19 22:01:40.000000 jztools-0.1.5/tests/jztools/object_recorder/recording_switch_utils.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.860491 jztools-0.1.5/tests/jztools/pacers/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-14 20:09:15.000000 jztools-0.1.5/tests/jztools/pacers/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4548 2024-04-19 18:50:02.000000 jztools-0.1.5/tests/jztools/pacers/pacers.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.861313 jztools-0.1.5/tests/jztools/parallelization/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-03-31 00:34:30.000000 jztools-0.1.5/tests/jztools/parallelization/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1028 2024-04-18 22:28:24.000000 jztools-0.1.5/tests/jztools/parallelization/_outsourced_iterable_base.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1727 2024-04-19 04:39:04.000000 jztools-0.1.5/tests/jztools/parallelization/_parallelizer.py
+-rw-r--r--   0 jazs       (501) staff       (20)      218 2024-04-18 22:28:24.000000 jztools-0.1.5/tests/jztools/parallelization/mock.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.861883 jztools-0.1.5/tests/jztools/parallelization/multiprocessing/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-14 20:09:15.000000 jztools-0.1.5/tests/jztools/parallelization/multiprocessing/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      312 2024-04-18 22:28:23.000000 jztools-0.1.5/tests/jztools/parallelization/multiprocessing/outsourced_iterable.py
+-rw-r--r--   0 jazs       (501) staff       (20)      538 2024-04-18 22:28:23.000000 jztools-0.1.5/tests/jztools/parallelization/multiprocessing/process_with_info.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4140 2024-04-19 04:46:05.000000 jztools-0.1.5/tests/jztools/parallelization/selector.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.862574 jztools-0.1.5/tests/jztools/parallelization/threading/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-14 20:09:15.000000 jztools-0.1.5/tests/jztools/parallelization/threading/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5255 2024-04-18 22:28:23.000000 jztools-0.1.5/tests/jztools/parallelization/threading/general.py
+-rw-r--r--   0 jazs       (501) staff       (20)      715 2024-04-18 22:28:23.000000 jztools-0.1.5/tests/jztools/parallelization/threading/outsourced_callable.py
+-rw-r--r--   0 jazs       (501) staff       (20)      307 2024-04-18 22:20:22.000000 jztools-0.1.5/tests/jztools/parallelization/threading/outsourced_iterable.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3432 2024-04-19 22:01:39.000000 jztools-0.1.5/tests/jztools/profiling.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5892 2024-04-17 23:46:09.000000 jztools-0.1.5/tests/jztools/py.py
+-rw-r--r--   0 jazs       (501) staff       (20)      135 2024-04-18 05:42:40.000000 jztools-0.1.5/tests/jztools/py_support.py
+-rw-r--r--   0 jazs       (501) staff       (20)      423 2024-04-19 22:01:39.000000 jztools-0.1.5/tests/jztools/recording_switch_utils__helper.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3433 2024-04-19 21:59:01.000000 jztools-0.1.5/tests/jztools/reference_sequence.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3720 2024-04-19 22:01:39.000000 jztools-0.1.5/tests/jztools/reference_sequence_v0.py
+-rw-r--r--   0 jazs       (501) staff       (20)    16184 2024-04-19 22:01:39.000000 jztools-0.1.5/tests/jztools/shared_memory.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3265 2024-04-19 21:37:25.000000 jztools-0.1.5/tests/jztools/slice_sequence.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 16:28:38.863005 jztools-0.1.5/tests/jztools/sqlalchemy/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-03-31 00:34:30.000000 jztools-0.1.5/tests/jztools/sqlalchemy/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      766 2024-04-14 20:09:15.000000 jztools-0.1.5/tests/jztools/sqlalchemy/_helper.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2170 2024-04-19 21:35:20.000000 jztools-0.1.5/tests/jztools/sqlalchemy/threaded_insert_cache.py
+-rw-r--r--   0 jazs       (501) staff       (20)      859 2024-04-19 22:01:39.000000 jztools-0.1.5/tests/jztools/timer.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3051 2024-04-17 23:46:09.000000 jztools-0.1.5/tests/jztools/validation.py
```

### Comparing `jztools-0.1.3/LICENSE` & `jztools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/logging.py` & `jztools-0.1.5/jztools/logging.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/numpy.py` & `jztools-0.1.5/jztools/numpy.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/__init__.py` & `jztools-0.1.5/jztools/parallelization/__init__.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/_base.py` & `jztools-0.1.5/jztools/parallelization/_base.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/_outsourced_iterable_base.py` & `jztools-0.1.5/jztools/parallelization/_outsourced_iterable_base.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/mock.py` & `jztools-0.1.5/jztools/parallelization/mock.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/multiprocessing/outsourced_iterable.py` & `jztools-0.1.5/jztools/parallelization/multiprocessing/outsourced_iterable.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/multiprocessing/process_with_info.py` & `jztools-0.1.5/jztools/parallelization/multiprocessing/process_with_info.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/outsourced_callable_base.py` & `jztools-0.1.5/jztools/parallelization/outsourced_callable_base.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/selector.py` & `jztools-0.1.5/jztools/parallelization/selector.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/threading/general.py` & `jztools-0.1.5/jztools/parallelization/threading/general.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/threading/lock.py` & `jztools-0.1.5/jztools/parallelization/threading/lock.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/threading/queue.py` & `jztools-0.1.5/jztools/parallelization/threading/queue.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/threading/util.py` & `jztools-0.1.5/jztools/parallelization/threading/util.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/parallelization/utils.py` & `jztools-0.1.5/jztools/parallelization/utils.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/py.py` & `jztools-0.1.5/jztools/py.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from io import IOBase
 from inspect import isclass, ismodule
 from typing import Dict, List, Any, Union, Callable
 import traceback
 import inspect
 import tempfile
 from importlib import import_module as _import_module
-from py.path import local  # TODO - pytest session still returns this type of paths
+
+# from py.path import local  # TODO - pytest session still returns this type of paths
 
 
 def _raise(ex):
     raise ex
 
 
 def not_implemented_property(name):
```

### Comparing `jztools-0.1.3/jztools/reference_sequence.py` & `jztools-0.1.5/jztools/reference_sequence.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/rentemp.py` & `jztools-0.1.5/jztools/rentemp.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/serializer/__init__.py` & `jztools-0.1.5/jztools/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/serializer/abstract_type_serializer.py` & `jztools-0.1.5/jztools/serializer/abstract_type_serializer.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/serializer/extensions.py` & `jztools-0.1.5/jztools/serializer/extensions.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/serializer/serializer.py` & `jztools-0.1.5/jztools/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/jztools/validation.py` & `jztools-0.1.5/jztools/validation.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/scripts/test_install` & `jztools-0.1.5/scripts/isotest`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from uuid import uuid1
 
 
 @clx.command()
 @clx.argument(
     "--package",
     default="local:.",
-    help="Package to install. Use local:<path> to install from local source or pip:<name> to install from pip repository",
-)
+    help="[local:.] Package to install. Use local:<path> to install from local source or pip:<name> to install from pip repository",
+)  #
 @clx.argument("--tests", default="./tests", help="Path to tests")
 def main(package, tests):
     """
     Creates a new conda environment, installs the specified package, and runs the tests in the specified directory.
 
     Run from a python project root to test the module under development in isolation.
     """
@@ -26,14 +26,14 @@
 
     # Build the env and run tests
     conda_env = str(uuid1())
     try:
         subp.check_call(["conda", "create", "-y", "-n", conda_env, "pip", "pytest"])
         cmds = [install_cmd, ["pytest", tests]]
         for cmd in cmds:
-            subp.check_call(["conda", "run", *cmd])
+            subp.check_call(["conda", "run", "-n", conda_env, *cmd])
     finally:
         subp.check_call(["conda", "env", "remove", "-y", "-n", conda_env])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jztools-0.1.3/tests/jztools/logging.py` & `jztools-0.1.5/tests/jztools/logging.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/parallelization/_outsourced_iterable_base.py` & `jztools-0.1.5/tests/jztools/parallelization/_outsourced_iterable_base.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/parallelization/_parallelizer.py` & `jztools-0.1.5/tests/jztools/parallelization/_parallelizer.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/parallelization/multiprocessing/process_with_info.py` & `jztools-0.1.5/tests/jztools/parallelization/multiprocessing/process_with_info.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/parallelization/selector.py` & `jztools-0.1.5/tests/jztools/parallelization/selector.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/parallelization/threading/general.py` & `jztools-0.1.5/tests/jztools/parallelization/threading/general.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/parallelization/threading/outsourced_callable.py` & `jztools-0.1.5/tests/jztools/parallelization/threading/outsourced_callable.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/py.py` & `jztools-0.1.5/tests/jztools/py.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/reference_sequence.py` & `jztools-0.1.5/tests/jztools/reference_sequence.py`

 * *Files identical despite different names*

### Comparing `jztools-0.1.3/tests/jztools/validation.py` & `jztools-0.1.5/tests/jztools/validation.py`

 * *Files identical despite different names*

