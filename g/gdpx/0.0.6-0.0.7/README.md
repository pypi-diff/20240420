# Comparing `tmp/gdpx-0.0.6.tar.gz` & `tmp/gdpx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdpx-0.0.6.tar", last modified: Sun Apr  7 20:51:53 2024, max compression
+gzip compressed data, was "gdpx-0.0.7.tar", last modified: Sat Apr 20 02:07:30 2024, max compression
```

## Comparing `gdpx-0.0.6.tar` & `gdpx-0.0.7.tar`

### file list

```diff
@@ -1,299 +1,321 @@
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.978648 gdpx-0.0.6/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    35149 2023-04-10 18:29:40.000000 gdpx-0.0.6/LICENSE
--rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-04-07 20:51:53.977647 gdpx-0.0.6/PKG-INFO
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6294 2023-12-12 17:08:13.000000 gdpx-0.0.6/README.md
--rw-r--r--   0 jx1279   (353055) chem     (30004)      899 2024-04-07 20:50:42.000000 gdpx-0.0.6/pyproject.toml
--rw-r--r--   0 jx1279   (353055) chem     (30004)       38 2024-04-07 20:51:53.978648 gdpx-0.0.6/setup.cfg
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.498654 gdpx-0.0.6/src/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.507654 gdpx-0.0.6/src/gdpx/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.527653 gdpx-0.0.6/src/gdpx/bias/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      543 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/bias/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3140 2024-02-14 21:26:12.000000 gdpx-0.0.6/src/gdpx/bias/afir.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1679 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/bias/bias.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3071 2024-04-07 20:47:54.000000 gdpx-0.0.6/src/gdpx/bias/gaussian.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2866 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/bias/harmonic.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1209 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/bias/nuclei.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.537653 gdpx-0.0.6/src/gdpx/builder/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2881 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3100 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/builder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      800 2023-12-03 04:28:22.000000 gdpx-0.0.6/src/gdpx/builder/cleave_group.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2659 2023-12-03 04:22:10.000000 gdpx-0.0.6/src/gdpx/builder/cleave_surface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5743 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/constraints.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      384 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/crossover.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1469 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/dimer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7451 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/direct.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.540653 gdpx-0.0.6/src/gdpx/builder/graph/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      287 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/graph/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5942 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/exchange.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5089 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/insert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5355 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/modifier.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5664 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/remove.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5373 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/group.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6914 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/builder/hypercube.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2745 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/insert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8537 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.540653 gdpx-0.0.6/src/gdpx/builder/mutation/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      892 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/mutation/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5565 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/packer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2972 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/perturbator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    15179 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/randomBuilder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    19280 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/region.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      745 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/repeat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3614 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/species.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6065 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1391 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/zoom.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.550653 gdpx-0.0.6/src/gdpx/colvar/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      463 2024-04-07 20:47:54.000000 gdpx-0.0.6/src/gdpx/colvar/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2622 2023-09-06 03:11:48.000000 gdpx-0.0.6/src/gdpx/colvar/compute_reweight.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1554 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/colvar/coordination.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      636 2024-04-07 20:47:54.000000 gdpx-0.0.6/src/gdpx/colvar/distance.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3567 2024-02-19 02:43:10.000000 gdpx-0.0.6/src/gdpx/colvar/fingerprint.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5096 2023-08-21 19:26:15.000000 gdpx-0.0.6/src/gdpx/colvar/plot_meta.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5603 2023-11-09 19:54:15.000000 gdpx-0.0.6/src/gdpx/colvar/plot_string.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4637 2023-08-31 04:35:40.000000 gdpx-0.0.6/src/gdpx/colvar/plotstring.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      178 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/colvar/position.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2749 2023-09-05 04:11:13.000000 gdpx-0.0.6/src/gdpx/colvar/reweight.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-02-21 03:43:26.000000 gdpx-0.0.6/src/gdpx/colvar/rmsd.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.614652 gdpx-0.0.6/src/gdpx/comparator/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      954 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/comparator/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2739 2023-12-06 01:21:35.000000 gdpx-0.0.6/src/gdpx/comparator/cartesian.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      827 2024-01-23 21:20:47.000000 gdpx-0.0.6/src/gdpx/comparator/comparator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5645 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/comparator/coordination.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4595 2023-12-06 01:21:35.000000 gdpx-0.0.6/src/gdpx/comparator/graph.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1193 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/comparator/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3067 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/comparator/reaction.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5123 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/comparator/singlepoint.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.636652 gdpx-0.0.6/src/gdpx/computation/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      657 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/computation/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    27174 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/asedriver.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    21647 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18003 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/driver.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8651 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/computation/espresso.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    19842 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31347 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/lammps.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    22229 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/lasp.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.637652 gdpx-0.0.6/src/gdpx/computation/md/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1082 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/computation/md/md_utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5296 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/computation/md/nosehoover.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/computation/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2372 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    20268 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1463 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/config.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.640652 gdpx-0.0.6/src/gdpx/core/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      108 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/core/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2415 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/core/node.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2492 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/operation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      861 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/core/placeholder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7032 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/register.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.644652 gdpx-0.0.6/src/gdpx/core/session/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      148 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/core/session/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12927 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/active.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2007 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/basic.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7692 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2583 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/session.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1998 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/core/session/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/core/variable.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.673651 gdpx-0.0.6/src/gdpx/data/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6210 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/ClusterAndCUR.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      249 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    57236 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/data/analyser.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    14976 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/array.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7981 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/cleave_deviation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1901 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/convert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3103 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/correction.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9171 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/database.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11961 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/dataset.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1552 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/extatoms.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3389 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/extract_evolution.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    14345 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10543 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/operators.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1950 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/system.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1210 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/utils.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.676651 gdpx-0.0.6/src/gdpx/describer/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      441 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/describer/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2325 2024-02-09 18:38:45.000000 gdpx-0.0.6/src/gdpx/describer/describer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2066 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/describer/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2365 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/describer/soap.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2438 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/describer/spc.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.678651 gdpx-0.0.6/src/gdpx/expedition/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1360 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.679651 gdpx-0.0.6/src/gdpx/expedition/af/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10315 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/af/afir.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1793 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/expedition.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.680651 gdpx-0.0.6/src/gdpx/expedition/ga/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    25925 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/ga/engine.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17387 2024-02-27 18:01:28.000000 gdpx-0.0.6/src/gdpx/expedition/ga/population.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5346 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.682651 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      149 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      802 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/basin_hopping.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18345 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/monte_carlo.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.686651 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2356 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9188 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/exchange.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5008 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/move.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8411 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/operator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11096 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/react.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4394 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/swap.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.686651 gdpx-0.0.6/src/gdpx/expedition/simulated_annealing/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5956 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/simulated_annealing/simulated_annealing.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.738651 gdpx-0.0.6/src/gdpx/graph/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      147 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    13870 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/graph/comparison.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12839 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/creator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12200 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/graph/graph_main.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5142 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/molecule.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31066 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/sites.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/surface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1849 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/graph/utils.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     8927 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/main.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2242 2023-07-23 06:17:20.000000 gdpx-0.0.6/src/gdpx/nanoparticle.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.757650 gdpx-0.0.6/src/gdpx/potential/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      273 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.758650 gdpx-0.0.6/src/gdpx/potential/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      654 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/calculators/dummy.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4675 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/calculators/mixer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1256 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5629 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/manager.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.779650 gdpx-0.0.6/src/gdpx/potential/managers/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2977 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1534 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/bias.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2947 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/cp2k.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.782650 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      225 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7170 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/calculator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4058 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/convert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    23429 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/deepmd.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1141 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/dftd3.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2231 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/eam.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1117 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/emt.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2363 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/espresso.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.786650 gdpx-0.0.6/src/gdpx/potential/managers/gp/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2348 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/bench.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/fgp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3746 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/gptools.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3474 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/representation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    46869 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/sgp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2715 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/potential/managers/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1986 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/lasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    13122 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/mace.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1840 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/mixer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7976 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/nequip.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.786650 gdpx-0.0.6/src/gdpx/potential/managers/plumed/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.788650 gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2728 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9361 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed2.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2394 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/plumed/plumed.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.789650 gdpx-0.0.6/src/gdpx/potential/managers/reann/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7421 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/reann/beann.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.790650 gdpx-0.0.6/src/gdpx/potential/managers/reann/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3361 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/reann/calculators/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17687 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/reann/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1396 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/reax.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8903 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/schnet.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3654 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1207 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/xtb.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5499 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/trainer.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.804650 gdpx-0.0.6/src/gdpx/reactor/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      860 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.811650 gdpx-0.0.6/src/gdpx/reactor/future/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    23672 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/AccCons.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    16224 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/AccHop.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2601 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/AccNEB.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2921 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/cmp_mep.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3833 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/constrain.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7051 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/crs.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2226 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/diffusion3.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    11410 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/find_adsorption.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3188 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/find_inter.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3002 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/muller-brown.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     1154 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/test_mh.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7056 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1482 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/reactor.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.818650 gdpx-0.0.6/src/gdpx/reactor/string/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      232 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/string/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17830 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/reactor/string/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5117 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/reactor/string/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9587 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/string/pathway.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11394 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/string/string.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8168 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/string/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2320 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/utils.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.822650 gdpx-0.0.6/src/gdpx/scheduler/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      699 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      624 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/scheduler/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      631 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/local.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3553 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/lsf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1147 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/pbs.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4439 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/scheduler.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3226 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/slurm.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.862649 gdpx-0.0.6/src/gdpx/selector/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1078 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3664 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/basin.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6276 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/compare.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/composition.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8362 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/cur.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7161 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/descriptor.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5631 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/graph.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6398 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/interval.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      622 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/invariant.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3284 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/locate.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11955 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/property.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1987 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/random.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      955 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/scf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10041 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/selector.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.874649 gdpx-0.0.6/src/gdpx/trainer/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1050 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/trainer/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6277 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/trainer/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.901648 gdpx-0.0.6/src/gdpx/utils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7894 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/atomUtils.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2908 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/cleave_cluster.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1247 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/utils/cmdrun.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6500 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/cmp_refdat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6476 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/utils/command.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    12328 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/comparision.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.902649 gdpx-0.0.6/src/gdpx/utils/dputils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9418 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/dputils/DeepPot.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    14661 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/dputils/acquire_dmat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1095 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/geometry.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2147 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/plot_dimer.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7761 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/reduce_dataset.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6200 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/second_reduce.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5412 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/utils/split-dataset.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2444 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/utils/strucopy.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.957648 gdpx-0.0.6/src/gdpx/validator/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1945 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5610 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/diffusion_coefficient.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4095 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/validator/dimer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2640 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/eos.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4779 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/validator/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5879 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/mdf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7477 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/melting_point.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5744 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/minima.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      583 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/rank.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9391 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/rdf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3436 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/validator/rxn.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8794 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/validator/spc.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3690 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/surface_energy.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2029 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      980 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/validator.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.976647 gdpx-0.0.6/src/gdpx/worker/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       84 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31878 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/worker/drive.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6935 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/explore.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7188 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11343 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18256 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/react.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12738 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/worker/single.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11940 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/train.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1958 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6077 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/worker.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.977647 gdpx-0.0.6/src/gdpx.egg-info/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/PKG-INFO
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8166 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/SOURCES.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)        1 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/dependency_links.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)       39 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/entry_points.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)      111 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/requires.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)        5 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/top_level.txt
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:30.729788 gdpx-0.0.7/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    35149 2023-04-10 18:29:40.000000 gdpx-0.0.7/LICENSE
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-04-20 02:07:30.729788 gdpx-0.0.7/PKG-INFO
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6294 2023-12-12 17:08:13.000000 gdpx-0.0.7/README.md
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      899 2024-04-20 02:07:12.000000 gdpx-0.0.7/pyproject.toml
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       38 2024-04-20 02:07:30.730788 gdpx-0.0.7/setup.cfg
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.658738 gdpx-0.0.7/src/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.730739 gdpx-0.0.7/src/gdpx/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.817740 gdpx-0.0.7/src/gdpx/bias/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1216 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.818740 gdpx-0.0.7/src/gdpx/bias/afir/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      119 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/afir/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4571 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/afir/afir.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1679 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/bias/bias.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7641 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/bondboost.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.820740 gdpx-0.0.7/src/gdpx/bias/gaussian/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      309 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/gaussian/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9777 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/gaussian/bond.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5649 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/gaussian/com.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3047 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/gaussian/gaussian.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5429 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/gaussian/rmsd.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.822740 gdpx-0.0.7/src/gdpx/bias/harmonic/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      248 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/harmonic/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2417 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/harmonic/distance.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2740 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/harmonic/harmonic.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2192 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/harmonic/plane.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1209 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/bias/nuclei.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1404 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/timeio.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:26.823740 gdpx-0.0.7/src/gdpx/bias/utils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      224 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/utils/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2696 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/bias/utils/bondpair.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.132744 gdpx-0.0.7/src/gdpx/builder/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2881 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3100 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/builder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      800 2023-12-03 04:28:22.000000 gdpx-0.0.7/src/gdpx/builder/cleave_group.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2659 2023-12-03 04:22:10.000000 gdpx-0.0.7/src/gdpx/builder/cleave_surface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5743 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/constraints.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      384 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/crossover.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1469 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/dimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7451 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/direct.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.248745 gdpx-0.0.7/src/gdpx/builder/graph/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      287 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/graph/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5942 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/graph/exchange.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5089 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/graph/insert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5355 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/graph/modifier.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5664 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/graph/remove.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5373 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/group.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6914 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/builder/hypercube.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8530 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/builder/insert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8537 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.273745 gdpx-0.0.7/src/gdpx/builder/mutation/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      892 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/mutation/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5565 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/packer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3406 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/builder/perturbator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    15179 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/randomBuilder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    19280 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/builder/region.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      745 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/repeat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3614 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/species.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7762 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/builder/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1391 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/builder/zoom.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.303746 gdpx-0.0.7/src/gdpx/cli/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2044 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/cli/compute.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.442747 gdpx-0.0.7/src/gdpx/colvar/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      463 2024-04-20 02:06:38.000000 gdpx-0.0.7/src/gdpx/colvar/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2622 2023-09-06 03:11:48.000000 gdpx-0.0.7/src/gdpx/colvar/compute_reweight.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1554 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/colvar/coordination.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      636 2024-04-20 02:06:38.000000 gdpx-0.0.7/src/gdpx/colvar/distance.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3567 2024-02-19 02:43:10.000000 gdpx-0.0.7/src/gdpx/colvar/fingerprint.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5096 2023-08-21 19:26:15.000000 gdpx-0.0.7/src/gdpx/colvar/plot_meta.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5603 2023-11-09 19:54:15.000000 gdpx-0.0.7/src/gdpx/colvar/plot_string.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4637 2023-08-31 04:35:40.000000 gdpx-0.0.7/src/gdpx/colvar/plotstring.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      178 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/colvar/position.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2749 2023-09-05 04:11:13.000000 gdpx-0.0.7/src/gdpx/colvar/reweight.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-02-21 03:43:26.000000 gdpx-0.0.7/src/gdpx/colvar/rmsd.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.585749 gdpx-0.0.7/src/gdpx/comparator/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      954 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/comparator/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2739 2023-12-06 01:21:35.000000 gdpx-0.0.7/src/gdpx/comparator/cartesian.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      827 2024-01-23 21:20:47.000000 gdpx-0.0.7/src/gdpx/comparator/comparator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5645 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/comparator/coordination.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4595 2023-12-06 01:21:35.000000 gdpx-0.0.7/src/gdpx/comparator/graph.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1193 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/comparator/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3067 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/comparator/reaction.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5123 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/comparator/singlepoint.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.719751 gdpx-0.0.7/src/gdpx/computation/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      657 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/computation/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    27675 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/computation/asedriver.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    21647 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/computation/cp2k.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18003 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/computation/driver.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8651 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/computation/espresso.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    19844 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/computation/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31347 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/computation/lammps.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    22229 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/computation/lasp.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.758751 gdpx-0.0.7/src/gdpx/computation/mc/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4259 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/computation/mc/tfmc.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.771751 gdpx-0.0.7/src/gdpx/computation/md/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1082 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/computation/md/md_utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5296 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/computation/md/nosehoover.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/computation/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2372 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/computation/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    20268 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/computation/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1463 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/config.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.834752 gdpx-0.0.7/src/gdpx/core/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      108 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/core/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2415 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/core/node.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2492 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/core/operation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      861 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/core/placeholder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7122 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/core/register.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:27.893753 gdpx-0.0.7/src/gdpx/core/session/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      148 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/core/session/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12927 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/core/session/active.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2007 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/core/session/basic.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7922 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/core/session/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2686 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/core/session/session.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1998 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/core/session/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/core/variable.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.100756 gdpx-0.0.7/src/gdpx/data/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6210 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/ClusterAndCUR.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      249 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    57236 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/data/analyser.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14976 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/data/array.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7981 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/cleave_deviation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1901 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/convert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3103 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/correction.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9171 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/database.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11961 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/data/dataset.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1552 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/data/extatoms.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3389 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/extract_evolution.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14345 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/data/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10543 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/data/operators.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1950 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/data/system.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1210 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/data/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.219757 gdpx-0.0.7/src/gdpx/describer/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      441 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/describer/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2325 2024-02-09 18:38:45.000000 gdpx-0.0.7/src/gdpx/describer/describer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2066 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/describer/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2365 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/describer/soap.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2438 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/describer/spc.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.266758 gdpx-0.0.7/src/gdpx/expedition/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1360 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.308758 gdpx-0.0.7/src/gdpx/expedition/accelerated_dynamics/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    16224 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/expedition/accelerated_dynamics/prev_example.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.309758 gdpx-0.0.7/src/gdpx/expedition/af/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10315 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/af/afir.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1793 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/expedition.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.319758 gdpx-0.0.7/src/gdpx/expedition/ga/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    25876 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/expedition/ga/engine.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18347 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/expedition/ga/population.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5346 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.337758 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      149 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      802 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/basin_hopping.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    20410 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/monte_carlo.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.396759 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2356 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9188 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/exchange.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5008 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/move.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8411 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/operator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11096 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/react.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4394 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/swap.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.405759 gdpx-0.0.7/src/gdpx/expedition/simulated_annealing/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5956 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/expedition/simulated_annealing/simulated_annealing.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.529761 gdpx-0.0.7/src/gdpx/graph/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      147 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/graph/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    13870 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/graph/comparison.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12839 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/graph/creator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12200 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/graph/graph_main.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5142 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/graph/molecule.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31066 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/graph/sites.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/graph/surface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1849 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/graph/utils.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     8774 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/main.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2242 2023-07-23 06:17:20.000000 gdpx-0.0.7/src/gdpx/nanoparticle.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.554761 gdpx-0.0.7/src/gdpx/potential/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      274 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/potential/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.579761 gdpx-0.0.7/src/gdpx/potential/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      654 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/calculators/dummy.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4675 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/potential/calculators/mixer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1256 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/potential/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5629 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/manager.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.874765 gdpx-0.0.7/src/gdpx/potential/managers/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3069 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/potential/managers/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1430 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/potential/managers/asepot.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1511 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/potential/managers/bias.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2947 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/cp2k.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:28.942766 gdpx-0.0.7/src/gdpx/potential/managers/deepmd/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      225 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/deepmd/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7170 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/deepmd/calculator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4058 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/deepmd/convert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    23429 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/deepmd/deepmd.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1141 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/dftd3.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2231 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/eam.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1117 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/emt.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2363 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/espresso.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.062767 gdpx-0.0.7/src/gdpx/potential/managers/gp/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/gp/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2348 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/gp/bench.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/gp/fgp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3746 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/gp/gptools.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3474 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/gp/representation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    46869 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/gp/sgp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2715 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/potential/managers/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1986 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/lasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17097 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/potential/managers/mace.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1840 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/potential/managers/mixer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7976 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/potential/managers/nequip.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.070767 gdpx-0.0.7/src/gdpx/potential/managers/plumed/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.099768 gdpx-0.0.7/src/gdpx/potential/managers/plumed/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2728 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/plumed/calculators/plumed.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9361 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/plumed/calculators/plumed2.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2394 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/plumed/plumed.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.146768 gdpx-0.0.7/src/gdpx/potential/managers/reann/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7421 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/potential/managers/reann/beann.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.171769 gdpx-0.0.7/src/gdpx/potential/managers/reann/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3361 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/potential/managers/reann/calculators/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17687 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/managers/reann/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1396 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/reax.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8903 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/schnet.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3654 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1207 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/potential/managers/xtb.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5499 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/potential/trainer.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.196769 gdpx-0.0.7/src/gdpx/reactor/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      860 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/reactor/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.355771 gdpx-0.0.7/src/gdpx/reactor/future/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    23672 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/AccCons.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2601 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/AccNEB.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2921 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/cmp_mep.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3833 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/constrain.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7051 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/crs.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2226 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/diffusion3.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    11410 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/find_adsorption.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3188 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/find_inter.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3002 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/muller-brown.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     1154 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/future/test_mh.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3971 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/reactor/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1482 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/reactor.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.453772 gdpx-0.0.7/src/gdpx/reactor/string/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      232 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/reactor/string/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17830 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/reactor/string/cp2k.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5117 2024-03-17 21:29:29.000000 gdpx-0.0.7/src/gdpx/reactor/string/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9587 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/reactor/string/pathway.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11906 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/reactor/string/string.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9158 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/reactor/string/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2320 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/reactor/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.532773 gdpx-0.0.7/src/gdpx/scheduler/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      699 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/scheduler/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      624 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/scheduler/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      631 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/scheduler/local.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3553 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/scheduler/lsf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1147 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/scheduler/pbs.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4439 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/scheduler/scheduler.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3226 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/scheduler/slurm.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.691775 gdpx-0.0.7/src/gdpx/selector/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1078 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/selector/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3664 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/basin.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6276 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/compare.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/composition.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8362 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/cur.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7241 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/selector/descriptor.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5631 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/graph.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6398 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/selector/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/interval.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      622 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/invariant.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3284 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/locate.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14855 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/selector/property.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1987 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/selector/random.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      955 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/selector/scf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10041 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/selector/selector.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:29.711775 gdpx-0.0.7/src/gdpx/trainer/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1050 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/trainer/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6277 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/trainer/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:30.057780 gdpx-0.0.7/src/gdpx/utils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7894 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/atomUtils.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2908 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/cleave_cluster.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1247 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/utils/cmdrun.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6500 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/cmp_refdat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6476 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/utils/command.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    12328 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/comparision.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:30.087780 gdpx-0.0.7/src/gdpx/utils/dputils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9418 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/dputils/DeepPot.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    14661 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/dputils/acquire_dmat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1095 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/geometry.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2147 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/plot_dimer.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7761 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/reduce_dataset.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6200 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/utils/second_reduce.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5412 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/utils/split-dataset.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2444 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/utils/strucopy.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:30.486785 gdpx-0.0.7/src/gdpx/validator/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1945 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/validator/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5610 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/validator/diffusion_coefficient.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4095 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/validator/dimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2640 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/validator/eos.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4779 2024-03-02 03:59:21.000000 gdpx-0.0.7/src/gdpx/validator/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5879 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/validator/mdf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7477 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/validator/melting_point.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5744 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/validator/minima.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      583 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/validator/rank.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9391 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/validator/rdf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3436 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/validator/rxn.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8794 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/validator/spc.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3690 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/validator/surface_energy.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2029 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/validator/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      980 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/validator/validator.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:30.716788 gdpx-0.0.7/src/gdpx/worker/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       84 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/worker/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31878 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/worker/drive.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6935 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/worker/explore.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7188 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/worker/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11514 2024-04-20 02:06:51.000000 gdpx-0.0.7/src/gdpx/worker/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18256 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/worker/react.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12738 2024-04-07 20:49:18.000000 gdpx-0.0.7/src/gdpx/worker/single.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11940 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/worker/train.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1958 2023-12-01 19:22:44.000000 gdpx-0.0.7/src/gdpx/worker/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6077 2024-03-17 21:29:30.000000 gdpx-0.0.7/src/gdpx/worker/worker.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-20 02:07:30.728788 gdpx-0.0.7/src/gdpx.egg-info/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-04-20 02:07:26.000000 gdpx-0.0.7/src/gdpx.egg-info/PKG-INFO
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8681 2024-04-20 02:07:26.000000 gdpx-0.0.7/src/gdpx.egg-info/SOURCES.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        1 2024-04-20 02:07:26.000000 gdpx-0.0.7/src/gdpx.egg-info/dependency_links.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       39 2024-04-20 02:07:26.000000 gdpx-0.0.7/src/gdpx.egg-info/entry_points.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      111 2024-04-20 02:07:26.000000 gdpx-0.0.7/src/gdpx.egg-info/requires.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        5 2024-04-20 02:07:26.000000 gdpx-0.0.7/src/gdpx.egg-info/top_level.txt
```

### Comparing `gdpx-0.0.6/LICENSE` & `gdpx-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/PKG-INFO` & `gdpx-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automate computational chemistry/materials sciance and machine learning interatomic potential training workflow.
 Author-email: Jiayan Xu <ahcigar@foxmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdpx-0.0.6/README.md` & `gdpx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/pyproject.toml` & `gdpx-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdpx"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
   "ase>=3.22",
   "h5py>=3.7.0",
   "joblib>=1.1.0",
   "networkx>=2.6.3",
   "omegaconf>=2.3.0",
   "pydantic>=2.1.1",
```

### Comparing `gdpx-0.0.6/src/gdpx/bias/bias.py` & `gdpx-0.0.7/src/gdpx/bias/bias.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/bias/gaussian.py` & `gdpx-0.0.7/src/gdpx/bias/gaussian/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import numpy as np
 
 import jax
 import jax.numpy as jnp
 
 from ase.calculators.calculator import Calculator
 
-from . import registers
-
 
 @jax.jit
 def gaussian_bias(x, x_t, sigma, omega):
     """Compute bias potential.
 
     Args:
         x: (1, num_dim)
@@ -114,8 +112,8 @@
         self.results["energy"] = np.asarray(e)
         self.results["forces"] = np.array(f)
 
         return
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.6/src/gdpx/bias/harmonic.py` & `gdpx-0.0.7/src/gdpx/bias/harmonic/harmonic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from typing import List, Callable
 
-import pydantic
+import dataclasses
+from typing import List, Callable
 
 import numpy as np
 
 import jax
 import jax.numpy as jnp
-from jax import jit, grad, value_and_grad
 
 from ase.calculators.calculator import Calculator, all_changes
 
 
-@jit
+@jax.jit
 def harmonic(positions, cvfunc: Callable, k: float, s: float):
     """Harmonic bias potential."""
     colvars = cvfunc(positions) # NOTE: Must be 1D CV.
     bias = k*jnp.square(colvars - s)
 
     return jnp.sum(bias)
 
-@jit
+@jax.jit
 def upper_harmonic(positions, cvfunc: Callable, k: float, s: float):
     """Harmonic bias potential."""
     colvars = cvfunc(positions) # NOTE: Must be 1D CV.
     colvars = jnp.where(colvars > s, colvars, s)
 
     bias = k*jnp.square(colvars - s)
 
     return jnp.sum(bias)
 
-@jit
+@jax.jit
 def lower_harmonic(positions, cvfunc: Callable, k: float, s: float):
     """Harmonic bias potential."""
     colvars = cvfunc(positions) # NOTE: Must be 1D CV.
     colvars = jnp.where(colvars < s, colvars, s)
 
     bias = k*jnp.square(colvars - s)
 
     return jnp.sum(bias)
 
 
 
-class HarmonicSetting(pydantic.BaseModel):
+@dataclasses.dataclass
+class HarmonicSetting:
 
     #: Spring constant, unit of eV.
     k: float = 100.
 
     #: Function origin, unit of colvar.
     s: float = 0.
 
@@ -72,27 +72,23 @@
     """
 
     def __init__(self, colvar: dict=None, restart=None, label=None, atoms=None, directory=".", **kwargs):
         """"""
         super().__init__(restart=restart, label=label, atoms=atoms, directory=directory, **kwargs)
 
         # - check bias params
-        try:
-            self._setting = HarmonicSetting(**self.parameters)
-        except pydantic.ValidationError as e:
-            raise RuntimeError(e.errors())
-
+        self._setting = HarmonicSetting(**self.parameters)
         assert not (self._setting.upper and self._setting.lower)
 
         bias_func = harmonic
         if self._setting.upper:
             bias_func = upper_harmonic
         if self._setting.lower:
             bias_func = lower_harmonic
-        self.compute_harmonic = value_and_grad(bias_func, argnums=0)
+        self.compute_harmonic = jax.value_and_grad(bias_func, argnums=0)
 
         # - check colvar
         self.colvar = initiate_colvar(colvar)
 
         return
     
     def calculate(self, atoms=None, properties=["energy"], system_changes=["positions"]):
@@ -107,8 +103,8 @@
         self.results["energy"] = np.asarray(ret[0])
         self.results["forces"] = -np.array(ret[1]) # copy forces
 
         return
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.6/src/gdpx/bias/nuclei.py` & `gdpx-0.0.7/src/gdpx/bias/nuclei.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/__init__.py` & `gdpx-0.0.7/src/gdpx/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/builder.py` & `gdpx-0.0.7/src/gdpx/builder/builder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/cleave_group.py` & `gdpx-0.0.7/src/gdpx/builder/cleave_group.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/cleave_surface.py` & `gdpx-0.0.7/src/gdpx/builder/cleave_surface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/constraints.py` & `gdpx-0.0.7/src/gdpx/builder/constraints.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/dimer.py` & `gdpx-0.0.7/src/gdpx/builder/dimer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/direct.py` & `gdpx-0.0.7/src/gdpx/builder/direct.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/graph/exchange.py` & `gdpx-0.0.7/src/gdpx/builder/graph/exchange.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/graph/insert.py` & `gdpx-0.0.7/src/gdpx/builder/graph/insert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/graph/modifier.py` & `gdpx-0.0.7/src/gdpx/builder/graph/modifier.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/graph/remove.py` & `gdpx-0.0.7/src/gdpx/builder/graph/remove.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/group.py` & `gdpx-0.0.7/src/gdpx/builder/group.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/hypercube.py` & `gdpx-0.0.7/src/gdpx/builder/hypercube.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/insert.py` & `gdpx-0.0.7/src/gdpx/validator/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,78 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-
-import copy
-import itertools
-
 from typing import List
 
+import numpy as np
+from scipy.interpolate import make_interp_spline, BSpline
+
 from ase import Atoms
-from ase.io import read, write
+from ase.geometry import find_mic
 
+def get_properties(frames: List[Atoms], other_props = []):
+    """Get properties of frames for comparison.
 
-from . import registers
-from .builder import StructureModifier
-from .utils import check_overlap_neighbour, convert_composition_to_list
+    Currently, only total energy and forces are considered.
 
+    Returns:
+        tot_symbols: shape (nframes,)
+        tot_energies: shape (nframes,)
+        tot_forces: shape (nframes,3)
 
-class InsertModifier(StructureModifier):
+    """
+    tot_symbols, tot_energies, tot_forces = [], [], []
 
-    name = "insert"
+    for atoms in frames: # free energy per atom
+        # -- basic info
+        symbols = atoms.get_chemical_symbols()
+        tot_symbols.extend(symbols)
 
-    def __init__(
-        self, region, composition: dict, covalent_ratio=[0.8, 2.0], 
-        max_times_size: int=5, *args, **kwargs
-    ):
-        """"""
-        super().__init__(*args, **kwargs)
+        # -- energy
+        energy = atoms.get_potential_energy() 
+        tot_energies.append(energy)
 
-        # - system definition
-        self.region = copy.deepcopy(region) # TODO: str, dict, or a Region obeject?
-        shape = region.pop("method", None)
-        self._region = registers.create("region", shape, convert_name=True, **region)
+        # -- force
+        forces = atoms.get_forces(apply_constraint=False)
+        tot_forces.extend(forces.tolist())
 
-        self.composition = composition
-        self._composition_list = convert_composition_to_list(composition, region)
+    return tot_symbols, tot_energies, tot_forces
 
-        # - bond distance check
-        self.covalent_ratio = covalent_ratio
-        self.MAX_TIMES_SIZE = max_times_size
+def wrap_traj(frames):
+    """Align positions according to the first frame.
 
-        return
-    
-    def run(self, substrates: List[Atoms]=None, size:int=1, *args, **kwargs) -> List[Atoms]:
-        """"""
-        super().run(substrates=substrates, *args, **kwargs)
-
-        # TODO: if substrates is None?
-
-        frames = []
-        for substrate in self.substrates:
-            curr_frames = self._irun(substrate, size)
-            frames.extend(curr_frames)
+    This is necessary for computing physical quantities base on atomic positions 
+    with periodic boundary conditions.
 
-        return frames
+    NOTE:
+        This only works for fixed cell systems.
     
-    def _irun(self, substrate: Atoms, size: int):
-        """"""
-        frames = []
-        for i in range(size*self.MAX_TIMES_SIZE):
-            nframes = len(frames)
-            if nframes < size:
-                atoms = copy.deepcopy(substrate)
-                atoms = self._insert_species(atoms)
-                if check_overlap_neighbour(atoms, self.covalent_ratio):
-                    frames.append(atoms)
-            else:
-                break
-        else:
-            raise RuntimeError(
-                f"Failed to create {size} structures, only {nframes} are created."
-            )
+    TODO:
+        Variable cell systems?
 
-        return frames
-    
-    def _insert_species(self, atoms: Atoms):
-        """"""
-        species_list = itertools.chain(
-            *[[k for i in range(v)] for k, v in self._composition_list]
-        )
-        species_list = sorted(species_list, key=lambda a: a.get_chemical_formula())
-        nspecies = len(species_list)
-
-        random_positions = self._region.get_random_positions(
-            size=nspecies, rng=self.rng
-        )
-        for a, p in zip(species_list, random_positions):
-            # TODO: molecule?
-            a.positions = p
-            atoms += a
-        #write("xxx.xyz", atoms)
-        #exit()
+    """
+    cell = frames[0].get_cell(complete=True)
+    nframes = len(frames)
+    for i in range(1,nframes):
+        prev_positions = frames[i-1].get_positions()
+        curr_positions = frames[i].get_positions()
+        shift = curr_positions - prev_positions
+        curr_vectors, curr_distances = find_mic(shift, cell, pbc=True)
+        frames[i].positions = prev_positions + curr_vectors
+
+    return frames
+
+def smooth_curve(bins, points):
+    """"""
+    spl = make_interp_spline(bins, points, k=3)
+    bins = np.linspace(bins.min(), bins.max(), 300)
+    points= spl(bins)
+
+    for i, d in enumerate(points):
+        if d < 1e-6:
+            points[i] = 0.0
 
-        return atoms
+    return bins, points
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.6/src/gdpx/builder/interface.py` & `gdpx-0.0.7/src/gdpx/builder/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/mutation/__init__.py` & `gdpx-0.0.7/src/gdpx/builder/mutation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/packer.py` & `gdpx-0.0.7/src/gdpx/builder/packer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/perturbator.py` & `gdpx-0.0.7/src/gdpx/builder/perturbator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import copy
-from typing import List
+from typing import Optional, List
 
 import numpy as np
 
 from ase import Atoms
-from ase.io import read, write
 
 from .builder import StructureModifier 
-from .utils import check_overlap_neighbour
+from .utils import str2list_int, check_overlap_neighbour
 
 
 class PerturbatorBuilder(StructureModifier):
 
     name = "perturbater"
 
     #: Number of attempts to create a random candidate.
@@ -23,22 +22,22 @@
     #: Number of attempts to create a number of candidates.
     #       if 10 structures are to create, run will try 5*10=50 times.
     MAX_TIMES_SIZE: int = 5
 
     """Perturb positions of input structures.
 
     TODO:
-        1. Perturb cell.
-        2. Perturb distances, angles...
-        3. Check if perturbed structures are valid (too close distance).
+        1. Perturb distances, angles...
 
     """
 
     def __init__(
-            self, eps: float=None, ceps: float=None, covalent_ratio=[0.8, 2.0],
+            self, eps: Optional[float]=None, ceps: Optional[float]=None, 
+            group: Optional[str]=None,
+            covalent_ratio=[0.8, 2.0],
             max_times_size: int = 5, *args, **kwargs
         ):
         """Initialise a perturbator.
 
         Args:
             eps: Drift on atomic positions. Unit Ang.
             ceps: Drift on lattice constants. Unit Ang.
@@ -55,21 +54,26 @@
             ...
         else:
             ...
 
         self.eps = eps
         self.ceps = ceps
 
+        # - apply perturbation on a group of atoms, default is all
+        self.group = group
+        if self.group is not None:
+            self.group = str2list_int(self.group, convention="lmp")
+
         # - distance check
         self.covalent_ratio = covalent_ratio
         self.MAX_TIMES_SIZE = max_times_size
 
         return
     
-    def run(self, substrates: List[Atoms]=None, size:int=1, *args, **kwargs) -> List[Atoms]:
+    def run(self, substrates: Optional[List[Atoms]]=None, size:int=1, *args, **kwargs) -> List[Atoms]:
         """"""
         super().run(substrates=substrates, *args, **kwargs)
 
         frames = []
         for substrate in self.substrates:
             curr_frames = self._irun(substrate, size)
             frames.extend(curr_frames)
@@ -82,25 +86,30 @@
         for i in range(size*self.MAX_TIMES_SIZE):
             nframes = len(frames)
             if nframes < size:
                 atoms = copy.deepcopy(substrate)
                 if self.eps is not None:
                     natoms = len(atoms)
                     pos_drift = self.rng.random((natoms, 3))
+                    if self.group is not None:
+                        pos_drift_ = np.zeros((natoms, 3))
+                        pos_drift_[self.group] = pos_drift[self.group]
+                        pos_drift = pos_drift_
                     atoms.positions += pos_drift*self.eps
                 if all(atoms.pbc) and self.ceps is not None:
                     lat_drift = self.rng.random((3, 3))
                     atoms.cell += lat_drift*self.ceps
                 if check_overlap_neighbour(atoms, self.covalent_ratio):
                     frames.append(atoms)
             else:
                 break
         else:
+            nframes = len(frames)
             raise RuntimeError(
                 f"Failed to create {size} structures, only {nframes} are created."
             )
 
         return frames
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.6/src/gdpx/builder/randomBuilder.py` & `gdpx-0.0.7/src/gdpx/builder/randomBuilder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/region.py` & `gdpx-0.0.7/src/gdpx/builder/region.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/repeat.py` & `gdpx-0.0.7/src/gdpx/builder/repeat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/species.py` & `gdpx-0.0.7/src/gdpx/builder/species.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/builder/utils.py` & `gdpx-0.0.7/src/gdpx/builder/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
-from typing import List, Tuple, Mapping
+import copy
+from typing import Union, List, Tuple, Mapping
 
 import numpy as np
 
 import ase
 from ase import Atoms, units
 from ase.build import molecule
 from ase.collections import g2
@@ -16,25 +17,80 @@
 
 from ..core.operation import Operation
 from ..data.array import AtomsNDArray
 
 """Some extra operations.
 """
 
+
+def str2list_int(inp: str, convention: str = "lmp") -> List[int]:
+    """Convert a string to a List of int.
+
+    Args:
+        inp: A string contains numbers and colons.
+        convention: The input convention either `lmp` or `ase`.
+                    lmp index starts from 1 and includes the last.
+
+    Examples:
+        >>> str2list_int("1:2 4:6", "lmp")
+        >>> [0, 1, 3, 4, 5]
+        >>> str2list_int("1:2 4:6", "ase")
+        >>> [1, 4, 5]
+
+    Returns:
+        A List of integers.
+
+    """
+    ret = []
+    for x in inp.strip().split():
+        curr_range = list(map(int, x.split(":")))
+        if len(curr_range) == 1:
+            start, end = curr_range[0], curr_range[0]
+        else:
+            start, end = curr_range
+        if convention == "lmp":
+            ret.extend([i - 1 for i in list(range(start, end + 1))])
+        elif convention == "ase":
+            ret.extend(list(range(start, end)))
+        else:
+            ...
+
+    # remove duplicates
+    ret = sorted(list(set(ret)))
+
+    return ret
+
+
+def rotate_a_molecule(atoms, use_com: bool, rng):
+    """"""
+    atoms = copy.deepcopy(atoms)
+    num_atoms = len(atoms)
+    if not use_com:
+        center = np.mean(atoms.positions, axis=0)
+    else:
+        center = atoms.get_center_of_mass()
+
+    if num_atoms > 1:
+        phi, theta, psi = 360 * rng.uniform(0, 1, 3)
+        atoms.euler_rotate(phi=phi, theta=0.5 * theta, psi=psi, center=center)
+
+    return atoms
+
+
 def convert_string_to_atoms(species: str):
     """Convert a string to an Atoms object.
 
     Args:
         species: Species' name can be a chemical symbol or a chemical formula.
 
     """
     # - build adsorbate
     atoms = None
     if species in ase.data.chemical_symbols:
-        atoms = Atoms(species, positions=[[0.,0.,0.]])
+        atoms = Atoms(species, positions=[[0.0, 0.0, 0.0]])
     elif species in g2.names:
         atoms = molecule(species)
     else:
         raise ValueError(f"Fail to create species {species}")
 
     return atoms
 
@@ -42,134 +98,142 @@
 def compute_molecule_number_from_density(molecular_mass, volume, density) -> int:
     """Compute the number of molecules in the region with a given density.
 
     Args:
         moleculer_mass: unit in g/mol.
         volume: unit in Ang^3.
         density: unit in g/cm^3.
-    
+
     Returns:
         Number of molecules in the region.
 
     """
-    number = (density/molecular_mass) * volume * units._Nav * 1e-24
+    number = (density / molecular_mass) * volume * units._Nav * 1e-24
 
     return int(number)
 
 
 def check_overlap_neighbour(
-    atoms: Atoms, covalent_ratio
+    atoms: Atoms, covalent_ratio, custom_dmin_dict={}, excluded_pairs=[]
 ):
-    """ use neighbour list to check newly added atom is neither too close or too
-        far from other atoms
+    """use neighbour list to check newly added atom is neither too close or too
+    far from other atoms
     """
     atomic_numbers = atoms.get_atomic_numbers()
     cell = atoms.get_cell(complete=True)
     natoms = len(atoms)
 
     cov_min, cov_max = covalent_ratio
     dmin_dict = closest_distances_generator(set(atomic_numbers), cov_min)
+    # print(f"{dmin_dict =}")
+    # print(f"{custom_dmin_dict}")
+    for k, v in custom_dmin_dict.items():
+        dmin_dict[k] = v
+    # print(f"{dmin_dict =}")
     nl = NeighborList(
-        cov_max*np.array(natural_cutoffs(atoms)), 
-        skin=0.0, self_interaction=False, bothways=True
+        cov_max * np.array(natural_cutoffs(atoms)),
+        skin=0.0,
+        self_interaction=False,
+        bothways=True,
     )
     nl.update(atoms)
 
     is_valid = True
     for i in range(natoms):
         nei_indices, nei_offsets = nl.get_neighbors(i)
         if len(nei_indices) > 0:
             for j, offset in zip(nei_indices, nei_offsets):
                 distance = np.linalg.norm(
                     atoms.positions[i] - (atoms.positions[j] + np.dot(offset, cell))
                 )
-                atomic_pair = (atomic_numbers[i], atomic_numbers[j])
-                if distance < dmin_dict[atomic_pair]:
-                    is_valid = False
-                    break
+                if (i, j) not in excluded_pairs:
+                    atomic_pair = (atomic_numbers[i], atomic_numbers[j])
+                    if distance < dmin_dict[atomic_pair]:
+                        is_valid = False
+                        break
         else:
             # Find isolated atom which is not allowed...
             is_valid = False
             break
 
     return is_valid
 
+
 def convert_composition_to_list(composition: dict, region) -> List[Tuple[Atoms, int]]:
     """"""
     # - define the composition of the atoms to optimise
     blocks = []
     for k, v in composition.items():
         k = convert_string_to_atoms(k)
-        if isinstance(v, int): # number
+        if isinstance(v, int):  # number
             v = v
-        else: # string command
+        else:  # string command
             data = v.split()
             if data[0] == "density":
                 v = compute_molecule_number_from_density(
-                    np.sum(k.get_masses()), region.get_volume(), 
-                    density = float(data[1])
+                    np.sum(k.get_masses()), region.get_volume(), density=float(data[1])
                 )
             else:
                 raise RuntimeError(f"Unrecognised composition {k:v}.")
         blocks.append((k, v))
 
     # - check if there is any molecule
     for k, v in blocks:
         if len(k) > 1:
             use_tags = True
             break
     else:
         use_tags = False
 
-    #atom_numbers = [] # atomic number of inserted atoms
-    #for species, num in composition_blocks:
+    # atom_numbers = [] # atomic number of inserted atoms
+    # for species, num in composition_blocks:
     #    numbers = []
     #    for s, n in ase.formula.Formula(species.get_chemical_formula()).count().items():
     #        numbers.extend([ase.data.atomic_numbers[s]]*n)
     #    atom_numbers.extend(numbers*num)
-    
+
     return blocks
 
 
 class remove_vacuum(Operation):
 
     cache: str = "cache_frames.xyz"
 
-    def __init__(self, structures, thickness: float=20., directory="./") -> None:
+    def __init__(self, structures, thickness: float = 20.0, directory="./") -> None:
         """"""
         input_nodes = [structures]
         super().__init__(input_nodes, directory)
 
         self.thickness = thickness
 
         return
-    
+
     def forward(self, structures) -> List[Atoms]:
         """Remove some vaccum of structures.
 
         Args:
             structures: List[Atoms] or AtomsNDArray.
 
         """
         super().forward()
 
         if isinstance(structures, AtomsNDArray):
             frames = structures.get_marked_structures()
         else:
             frames = structures
-        
+
         # TODO: convert to atoms_array?
-        cache_fpath = self.directory/self.cache
+        cache_fpath = self.directory / self.cache
         if cache_fpath.exists():
             frames = read(cache_fpath, ":")
         else:
             for a in frames:
                 a.cell[2, 2] -= self.thickness
             write(cache_fpath, frames)
-        
+
         self.status = "finished"
 
         return frames
 
 
 class reset_cell(Operation):
 
@@ -179,41 +243,41 @@
         """"""
         input_nodes = [structures]
         super().__init__(input_nodes, directory)
 
         self.cell = np.array(cell)
 
         return
-    
+
     def forward(self, structures) -> List[Atoms]:
         """Remove some vaccum of structures.
 
         Args:
             structures: List[Atoms] or AtomsNDArray.
 
         """
         super().forward()
 
         if isinstance(structures, AtomsNDArray):
             frames = structures.get_marked_structures()
         else:
             frames = structures
-        
+
         # TODO: convert to atoms_array?
-        cache_fpath = self.directory/self.cache
+        cache_fpath = self.directory / self.cache
         if cache_fpath.exists():
             frames = read(cache_fpath, ":")
         else:
-            center_of_cell = np.sum(self.cell, axis=0)/2.
+            center_of_cell = np.sum(self.cell, axis=0) / 2.0
             for a in frames:
                 com = a.get_center_of_mass()
                 a.set_cell(self.cell)
                 a.positions -= com - center_of_cell
             write(cache_fpath, frames)
-        
+
         self.status = "finished"
 
         return frames
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.6/src/gdpx/builder/zoom.py` & `gdpx-0.0.7/src/gdpx/builder/zoom.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/compute_reweight.py` & `gdpx-0.0.7/src/gdpx/colvar/compute_reweight.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/coordination.py` & `gdpx-0.0.7/src/gdpx/colvar/coordination.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/distance.py` & `gdpx-0.0.7/src/gdpx/colvar/distance.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/fingerprint.py` & `gdpx-0.0.7/src/gdpx/colvar/fingerprint.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/plot_meta.py` & `gdpx-0.0.7/src/gdpx/colvar/plot_meta.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/plot_string.py` & `gdpx-0.0.7/src/gdpx/colvar/plot_string.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/plotstring.py` & `gdpx-0.0.7/src/gdpx/colvar/plotstring.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/reweight.py` & `gdpx-0.0.7/src/gdpx/colvar/reweight.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/colvar/rmsd.py` & `gdpx-0.0.7/src/gdpx/colvar/rmsd.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/__init__.py` & `gdpx-0.0.7/src/gdpx/comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/cartesian.py` & `gdpx-0.0.7/src/gdpx/comparator/cartesian.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/comparator.py` & `gdpx-0.0.7/src/gdpx/comparator/comparator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/coordination.py` & `gdpx-0.0.7/src/gdpx/comparator/coordination.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/graph.py` & `gdpx-0.0.7/src/gdpx/comparator/graph.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/interface.py` & `gdpx-0.0.7/src/gdpx/comparator/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/reaction.py` & `gdpx-0.0.7/src/gdpx/comparator/reaction.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/comparator/singlepoint.py` & `gdpx-0.0.7/src/gdpx/comparator/singlepoint.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/__init__.py` & `gdpx-0.0.7/src/gdpx/computation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/asedriver.py` & `gdpx-0.0.7/src/gdpx/computation/asedriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,19 +241,37 @@
             taup=taup * units.fs,
             compressibility_au=compressibility / units.bar,
         )
 
         return
 
 
+@dataclasses.dataclass
+class MonteCarloController(Controller):
+
+    name: str = "monte_carlo"
+
+    def __post_init__(self):
+        """"""
+        maxstepsize = self.params.get("maxstepsizes", 0.2)  # Ang
+
+        self.conv_params = dict(
+            maxstepsize=maxstepsize,
+            rng=None,
+        )
+
+        return
+
+
 controllers = dict(
     # - nvt
     berendsen_nvt=BerendsenThermostat,
     langevin_nvt=LangevinThermostat,
-    nosehoover_nvt=NoseHooverThermostat,
+    nose_hoover_nvt=NoseHooverThermostat,
+    monte_carlo_nvt=MonteCarloController,
     # - npt
     berendsen_npt=BerendsenBarostat,
 )
 
 
 @dataclasses.dataclass
 class AseDriverSetting(DriverSetting):
@@ -293,14 +311,16 @@
                 thermostat = thermo_cls(**self.controller)
                 if thermostat.name == "berendsen":
                     from ase.md.nvtberendsen import NVTBerendsen as driver_cls
                 elif thermostat.name == "langevin":
                     from ase.md.langevin import Langevin as driver_cls
                 elif thermostat.name == "nose_hoover":
                     from .md.nosehoover import NoseHoover as driver_cls
+                elif thermostat.name == "monte_carlo":
+                    from .mc.tfmc import TimeStampedMonteCarlo as driver_cls
                 else:
                     raise RuntimeError(f"Unknown thermostat {thermostat}.")
                 thermo_params = thermostat.conv_params
                 _init_md_params = dict(
                     fixcm=self.fix_cm,
                     timestep=self.timestep * units.fs,
                     temperature_K=self.temp,
```

### Comparing `gdpx-0.0.6/src/gdpx/computation/cp2k.py` & `gdpx-0.0.7/src/gdpx/computation/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/driver.py` & `gdpx-0.0.7/src/gdpx/computation/driver.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/espresso.py` & `gdpx-0.0.7/src/gdpx/computation/espresso.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/interface.py` & `gdpx-0.0.7/src/gdpx/computation/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class DriverVariable(Variable):
 
     def __init__(self, **kwargs):
         """"""
         # - compat
         copied_params = copy.deepcopy(kwargs)
         merged_params = dict(
-            task=copied_params.get("task", "min"),
+            # task=copied_params.get("task", "min"),
             backend=copied_params.get("backend", "external"),
             ignore_convergence=copied_params.get("ignore_convergence", False),
         )
         merged_params.update(**copied_params.get("init", {}))
         merged_params.update(**copied_params.get("run", {}))
 
         initial_value = self._broadcast_drivers(merged_params)
```

### Comparing `gdpx-0.0.6/src/gdpx/computation/lammps.py` & `gdpx-0.0.7/src/gdpx/computation/lammps.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/lasp.py` & `gdpx-0.0.7/src/gdpx/computation/lasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/md/md_utils.py` & `gdpx-0.0.7/src/gdpx/computation/md/md_utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/md/nosehoover.py` & `gdpx-0.0.7/src/gdpx/computation/md/nosehoover.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/utils.py` & `gdpx-0.0.7/src/gdpx/computation/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/computation/vasp.py` & `gdpx-0.0.7/src/gdpx/computation/vasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/config.py` & `gdpx-0.0.7/src/gdpx/config.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/node.py` & `gdpx-0.0.7/src/gdpx/core/node.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/operation.py` & `gdpx-0.0.7/src/gdpx/core/operation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/placeholder.py` & `gdpx-0.0.7/src/gdpx/core/placeholder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/register.py` & `gdpx-0.0.7/src/gdpx/core/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
 
     #: Regions.
     region: Register = Register("region")
 
     #: Builders.
     builder: Register = Register("builder")
 
+    #: Bias.
+    bias: Register = Register("bias")
+
     #: Colvars.
     colvar: Register = Register("colvar")
 
     #: Modifiers.
     modifier: Register = Register("modifier")
 
     #: Reactors.
@@ -157,14 +160,16 @@
     # - working components.
     # -- schedulers
     ("gdpx", ["scheduler"]),
     # -- managers (potentials)
     ("gdpx.potential", ["managers"]),
     # -- dataloaders (datasets)
     ("gdpx.data", ["dataset"]),
+    # -- bias
+    ("gdpx", ["bias"]),
     # -- builders
     ("gdpx", ["builder"]),
     # -- genetic-algorithm-related
     ("gdpx.builder", ["crossover", "mutation"]),
     # -- colvar
     ("gdpx", ["colvar"]),
     # -- selectors
```

### Comparing `gdpx-0.0.6/src/gdpx/core/session/active.py` & `gdpx-0.0.7/src/gdpx/core/session/active.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/session/basic.py` & `gdpx-0.0.7/src/gdpx/core/session/basic.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/session/interface.py` & `gdpx-0.0.7/src/gdpx/core/session/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,103 +13,87 @@
 import omegaconf
 from omegaconf import OmegaConf
 
 from .. import config
 from .utils import create_variable, create_operation
 
 
-#: GLOBAL ATTR.
-cache_nodes = {}
+class SessionInitialiser:
 
-# def instantiate_variable(vx_name, vx_params):
-#     """"""
-#     print(f"----- {vx_name} -----")
-#     params = {}
-#     for k, v in vx_params.items():
-#         print(k, v)
-#         ...
-#
-#     return
-#
-# def resolve_variables(variables: dict):
-#     """"""
-#     for vx_name, vx_params in variables.items():
-#         vx = instantiate_variable(vx_name, vx_params)
-#         ...
-#
-#     return
-
-
-def instantiate_operation(op_name, op_params):
-    """"""
-    params = {}
-    for k, v in op_params.items():
-        params[k] = v  # resolve one by one...
-    op = create_operation(op_name, op_params)
-
-    return op
-
-
-def resolve_operations(config: dict):
-    """"""
-    operations = {}
-    for op_name, op_params in config.items():
-        op = instantiate_operation(op_name, op_params)
-        operations[op_name] = op
-        cache_nodes[op_name] = op
+    #: Shared node objects.
+    cache_nodes = {}
 
-    return operations
-
-
-def register_custom_resolvers():
-    """"""
-
-    # - add resolvers
-    def create_vx_instance(vx_name, _root_):
+    @staticmethod
+    def instantiate_operation(op_name, op_params):
         """"""
-        if vx_name not in cache_nodes:
-            vx_params = OmegaConf.to_object(_root_.variables.get(vx_name))
-            vx = create_variable(vx_name, vx_params)
-            cache_nodes[vx_name] = vx
-            return vx
-        else:
-            return cache_nodes[vx_name]
-
-    OmegaConf.register_new_resolver("vx", create_vx_instance, use_cache=False)
-
-    def create_op_instance(op_name, _root_):
+        params = {}
+        for k, v in op_params.items():
+            params[k] = v  # resolve one by one...
+        op = create_operation(op_name, op_params)
+    
+        return op
+    
+    @staticmethod
+    def resolve_operations(config: dict):
         """"""
-        if op_name not in cache_nodes:
-            op_params = OmegaConf.to_object(_root_.operations.get(op_name))
-            op = create_operation(op_name, op_params)
-            cache_nodes[op_name] = op
-            return op
-        else:
-            return cache_nodes[op_name]
-
-    OmegaConf.register_new_resolver("op", create_op_instance, use_cache=False)
-
-    # --
-    def read_json(input_file):
-        with open(input_file, "r") as fopen:
-            input_dict = json.load(fopen)
-
-        return input_dict
-
-    OmegaConf.register_new_resolver("json", read_json)
-
-    def read_yaml(input_file):
-        with open(input_file, "r") as fopen:
-            input_dict = yaml.safe_load(fopen)
-
-        return input_dict
-
-    OmegaConf.register_new_resolver("yaml", read_yaml)
-
-    return
+        operations = {}
+        for op_name, op_params in config.items():
+            op = SessionInitialiser.instantiate_operation(op_name, op_params)
+            operations[op_name] = op
+            SessionInitialiser.cache_nodes[op_name] = op
+    
+        return operations
+    
+    @staticmethod
+    def register_custom_resolvers():
+        """"""
+    
+        # - add resolvers
+        def create_vx_instance(vx_name, _root_):
+            """"""
+            if vx_name not in SessionInitialiser.cache_nodes:
+                vx_params = OmegaConf.to_object(_root_.variables.get(vx_name))
+                vx = create_variable(vx_name, vx_params)
+                SessionInitialiser.cache_nodes[vx_name] = vx
+                return vx
+            else:
+                return SessionInitialiser.cache_nodes[vx_name]
+    
+        OmegaConf.register_new_resolver("vx", create_vx_instance, use_cache=False)
+    
+        def create_op_instance(op_name: str, _root_):
+            """"""
+            if op_name not in SessionInitialiser.cache_nodes:
+                op_params = OmegaConf.to_object(_root_.operations.get(op_name))
+                op = create_operation(op_name, op_params)
+                SessionInitialiser.cache_nodes[op_name] = op
+                return op
+            else:
+                return SessionInitialiser.cache_nodes[op_name]
+    
+        OmegaConf.register_new_resolver("op", create_op_instance, use_cache=False)
+    
+        # --
+        def read_json(input_file):
+            with open(input_file, "r") as fopen:
+                input_dict = json.load(fopen)
+    
+            return input_dict
+    
+        OmegaConf.register_new_resolver("json", read_json)
+    
+        def read_yaml(input_file):
+            with open(input_file, "r") as fopen:
+                input_dict = yaml.safe_load(fopen)
+    
+            return input_dict
+    
+        OmegaConf.register_new_resolver("yaml", read_yaml)
+    
+        return
 
 
 def run_session_once(config_dict: dict, feed_command=None, directory="./"):
     """Configure session with omegaconfig."""
     # - set directory
     directory = pathlib.Path(directory)
 
@@ -140,15 +124,15 @@
 
     # - resolve sessions
     # container = OmegaConf.to_object(conf.sessions)
     # for k, v in container.items():
     #    print(k, v)
 
     try:
-        operations = resolve_operations(conf["operations"])
+        operations = SessionInitialiser.resolve_operations(conf["operations"])
     except omegaconf.errors.InterpolationResolutionError as err:
         config._debug(traceback.format_exc())
         err_key = (str(err).strip().split("\n")[1]).strip().split(":")[1]
         config._print(f"FAILED TO PARSE `{err_key}` KEY.")
         err_info_tail = traceback.format_exc().split("\n")[-10:]
         for e in err_info_tail:
             config._print(f"{e}")
@@ -235,19 +219,20 @@
         with open(config_filepath, "r") as fopen:
             config_dict = yaml.safe_load(fopen)
     else:
         raise RuntimeError(f"Fail to load config `{str(config_filepath)}`")
 
     raw_config_dict = config_dict
 
-    register_custom_resolvers()
+    SessionInitialiser.register_custom_resolvers()
 
     # -
     if timewait > 0:
         for i in range(1000):
+            SessionInitialiser.cache_nodes = {} # Clear cache before a new run.
             config._print(f"Monitor is running step {i}!!!")
             config_dict = copy.deepcopy(raw_config_dict)
             is_finished = run_session_once(config_dict, feed_command, directory)
             if is_finished:
                 break
             else:
                 config._print(f"Monitor is sleeping for {timewait} seconds.")
```

### Comparing `gdpx-0.0.6/src/gdpx/core/session/session.py` & `gdpx-0.0.7/src/gdpx/core/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
                 # - check whether this node' not ready due to previous nodes are broken.
                 broken_states = []
                 for input_node in node.input_nodes:
                     if isinstance(input_node, Operation):
                         broken_states.append(input_node.is_about_to_exit())
                     else:
                         broken_states.append(False)
+                self._debug(f"{node.input_nodes =}")
+                self._debug(f"{broken_states =}")
                 is_broken = any(broken_states)
                 if not is_broken:
                     self.state = "StepToContinue"
                     self._print("  wait previous nodes to finish...")
                 else:
                     # The `broken` status is contagious
                     node.status = "exit"
```

### Comparing `gdpx-0.0.6/src/gdpx/core/session/utils.py` & `gdpx-0.0.7/src/gdpx/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/core/variable.py` & `gdpx-0.0.7/src/gdpx/core/variable.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/ClusterAndCUR.py` & `gdpx-0.0.7/src/gdpx/data/ClusterAndCUR.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/analyser.py` & `gdpx-0.0.7/src/gdpx/data/analyser.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/array.py` & `gdpx-0.0.7/src/gdpx/data/array.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/cleave_deviation.py` & `gdpx-0.0.7/src/gdpx/data/cleave_deviation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/convert.py` & `gdpx-0.0.7/src/gdpx/data/convert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/correction.py` & `gdpx-0.0.7/src/gdpx/data/correction.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/database.py` & `gdpx-0.0.7/src/gdpx/data/database.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/dataset.py` & `gdpx-0.0.7/src/gdpx/data/dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/extatoms.py` & `gdpx-0.0.7/src/gdpx/data/extatoms.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/extract_evolution.py` & `gdpx-0.0.7/src/gdpx/data/extract_evolution.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/interface.py` & `gdpx-0.0.7/src/gdpx/data/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/operators.py` & `gdpx-0.0.7/src/gdpx/data/operators.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/system.py` & `gdpx-0.0.7/src/gdpx/data/system.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/data/utils.py` & `gdpx-0.0.7/src/gdpx/data/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/describer/describer.py` & `gdpx-0.0.7/src/gdpx/describer/describer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/describer/interface.py` & `gdpx-0.0.7/src/gdpx/describer/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/describer/soap.py` & `gdpx-0.0.7/src/gdpx/describer/soap.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/describer/spc.py` & `gdpx-0.0.7/src/gdpx/describer/spc.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/__init__.py` & `gdpx-0.0.7/src/gdpx/expedition/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/af/afir.py` & `gdpx-0.0.7/src/gdpx/expedition/af/afir.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/expedition.py` & `gdpx-0.0.7/src/gdpx/expedition/expedition.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/ga/engine.py` & `gdpx-0.0.7/src/gdpx/expedition/ga/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ):
         """Initialise engine.
 
         Args:
             builder: Define the system to explore.
 
         """
-        ga_dict = params # For compat
+        ga_dict = params  # For compat
 
         # --- database ---
         self.db_name = ga_dict.get("database", "mydb.db")
 
         # -
         self.directory = directroy
 
@@ -174,26 +174,24 @@
                 atoms.get_potential_energy()
                 for atoms in all_relaxed_candidates
                 if atoms.info["key_value_pairs"]["generation"] == i
             ]
             self._print(energies)
             data.append([i, energies])
 
-        import matplotlib as mpl
-
-        mpl.use("Agg")  # silent mode
-        from matplotlib import pyplot as plt
+        import matplotlib.pyplot as plt
 
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12, 8))
-        ax.set_title("Population Evolution", fontsize=20, fontweight="bold")
+        ax.set_title("Population Evolution")
 
         for i, energies in data:
             ax.scatter([i] * len(energies), energies)
 
-        plt.savefig(results / "pop.png")
+        fig.savefig(results / "pop.png")
+        plt.close()
 
         return
 
     def update_active_params(self, prev_wdir, *args, **kwargs):
         """"""
         candidates = read(prev_wdir / "results" / "all_candidates.xyz", ":")
 
@@ -211,37 +209,38 @@
         """
         # - outputs
         assert self.worker is not None, "GA has not set its worker properly."
         self.worker.directory = self.directory / self.CALC_DIRNAME
         self.pop_manager._print = self._print
 
         # - search target
-        self._print(f"\n\n===== Genetic Algorithm =====")
+        self._print(f"===== Genetic Algorithm =====")
         target = self.prop_dict["target"]
-        self._print(f"\nTarget of Global Optimisation is {target}")
+        self._print(f"Target of Global Optimisation is {target}")
 
         # - worker info
-        self._print("\n\n===== register worker =====")
+        self._print("===== register worker =====")
 
         # - generator info
-        self._print("\n\n===== register builder =====")
-        self._print(self.generator)
+        self._print("===== register builder =====")
+        for l in str(self.generator).split("\n"):
+            self._print(l)
         self._print(f"random_state: f{self.generator.random_seed}")
 
         # NOTE: check database existence and generation number to determine restart
         self._debug(f"database path: {str(self.db_path)}")
         if not self.db_path.exists():
             self._print("----- create a new database -----")
             self._create_initial_population()
         else:
             self._print("restart the database...")
             self.da = DataConnection(self.db_path)
 
         # --- mutation and comparassion operators
-        self._print("\n\n===== register operators =====")
+        self._print("===== register operators =====")
         self._register_operators()
 
         # - run
         for i in range(1000):
             self._check_generation()
             if self.read_convergence():
                 self._print("reach maximum generation...")
@@ -291,42 +290,43 @@
     def _irun(self):
         """main procedure"""
         if not hasattr(self, "cur_gen"):
             raise RuntimeError(
                 "The current genertion is unknown. Check generation before."
             )
         # - generation
-        self._print("\n\n===== Generation Info =====")
+        self._print("===== Generation Info =====")
         self._print(f"current generation number: {self.cur_gen}")
         self._print(f"number of relaxed in current generation: {self.num_relaxed_gen}")
         self._print(convert_indices(sorted(self.relaxed_confids)))
         self._print(
             f"number of unrelaxed in current generation: {self.num_unrelaxed_gen}"
         )
         self._print(convert_indices(sorted(self.unrelaxed_confids)))
         self._print(f"end of current generation: {self.end_of_gen}")
 
         # - population
-        self._print("\n\n===== Population Info =====")
+        self._print("===== Population Info =====")
         content = "For generation > 0,\n"
         content += "{:>8s}  {:>8s}  {:>8s}  {:>8s}\n".format(
             "Reprod", "Random", "Mutate", "Total"
         )
         content += "{:>8d}  {:>8d}  {:>8d}  {:>8d}\n".format(
             self.pop_manager.gen_rep_size,
             self.pop_manager.gen_ran_size,
             self.pop_manager.gen_mut_size,
             self.pop_manager.gen_size,
         )
         content += "Note: Reproduced structure has a chance (pmut) to mutate.\n"
-        self._print(content)
+        for l in content.split("\n"):
+            self._print(l)
 
         # - minimise
         if self.cur_gen == 0:
-            self._print("\n\n===== Initial Population Calculation =====")
+            self._print("===== Initial Population Calculation =====")
             frames_to_work = []
             while (
                 self.da.get_number_of_unrelaxed_candidates()
             ):  # NOTE: this uses GADB get_atoms which adds extra_info
                 # calculate structures from init population
                 atoms = self.da.get_an_unrelaxed_candidate()
                 frames_to_work.append(atoms)
@@ -337,15 +337,15 @@
             if frames_to_work:
                 self.worker.directory = (
                     self.directory / self.CALC_DIRNAME / f"gen{self.cur_gen}"
                 )
                 _ = self.worker.run(frames_to_work)  # retrieve later
         else:
             # --- update population
-            self._print("\n\n===== Update Population =====")
+            self._print("===== Update Population =====")
             # - create the population used for crossover and mutation
             candidate_groups, num_paired, num_mutated, num_random = (
                 self.pop_manager._get_current_candidates(
                     database=self.da, curr_gen=self.cur_gen
                 )
             )
             # candidate_groups, num_paired, num_mutated, num_random = self.pop_manager._get_current_candidates(
@@ -451,15 +451,15 @@
         # --- check if there were finished jobs
         curr_convergence = False
         self.worker.directory = (
             self.directory / self.CALC_DIRNAME / f"gen{self.cur_gen}"
         )
         self.worker.inspect(resubmit=True)
         if self.worker.get_number_of_running_jobs() == 0:
-            self._print("\n\n===== Retrieve Relaxed Population =====")
+            self._print("===== Retrieve Relaxed Population =====")
             converged_candidates = [
                 t[-1] for t in self.worker.retrieve(use_archive=self.use_archive)
             ]
             for cand in converged_candidates:
                 self._print(cand)
                 self._print(cand.info)
                 # update extra info
```

### Comparing `gdpx-0.0.6/src/gdpx/expedition/ga/population.py` & `gdpx-0.0.7/src/gdpx/expedition/ga/population.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,58 +13,58 @@
 from ase.io import read, write
 from ase.ga.population import Population
 from ase.ga.data import DataConnection
 
 #: Retained keys in key_value_pairs when get_atoms from the database.
 RETAINED_KEYS: List[str] = ["extinct", "origin"]
 
+
 def clean_seed_structures(prev_frames: List[Atoms]):
     """"""
     curr_frames = []
     energies, forces = [], []
     for i, prev_atoms in enumerate(prev_frames):
         # - copy geometry
         curr_atoms = Atoms(
             symbols=copy.deepcopy(prev_atoms.get_chemical_symbols()),
             positions=copy.deepcopy(prev_atoms.get_positions()),
             cell=copy.deepcopy(prev_atoms.get_cell(complete=True)),
             pbc=copy.deepcopy(prev_atoms.get_pbc()),
-            tags = prev_atoms.get_tags() # retain this for molecules
+            tags=prev_atoms.get_tags(),  # retain this for molecules
         )
-        #if prev_atoms.get_kinetic_energy() > 0.: # retain this for MD
-        #    curr_atoms.set_momenta(prev_atoms.get_momenta()) 
+        # if prev_atoms.get_kinetic_energy() > 0.: # retain this for MD
+        #    curr_atoms.set_momenta(prev_atoms.get_momenta())
         curr_frames.append(curr_atoms)
 
         # - save properties
         try:
             ene = prev_atoms.get_potential_energy()
             energies.append(ene)
         except:
             raise RuntimeError(f"Cannot get energy for seed structure {i}.")
 
         try:
             frc = prev_atoms.get_forces()
             forces.append(frc)
         except:
             raise RuntimeError(f"Cannot get forces for seed structure {i}.")
-    
+
     for a, e, f in zip(curr_frames, energies, forces):
         calc = SinglePointCalculator(a, energy=e, forces=f)
         a.calc = calc
 
     return curr_frames
 
 
-class AbstractPopulationManager():
-
+class AbstractPopulationManager:
     """An abstract population manager for evolutionary algorithms.
 
-    For structure exploration, there are generally two formulations. ASE forms 
-    current population from all candidates while USPEX forms it based on the 
-    previous generation. Furthermore, USPEX uses fracGene, fracRand, fracTopRand, 
+    For structure exploration, there are generally two formulations. ASE forms
+    current population from all candidates while USPEX forms it based on the
+    previous generation. Furthermore, USPEX uses fracGene, fracRand, fracTopRand,
     fracPerm, fracAtomsMut, fracRotMut, fracLatMut, fracSpinMut...
 
     Example:
         Parameters needed
 
         $ cat ga.yaml
         population:
@@ -87,122 +87,143 @@
     MAX_ATTEMPTS_MULTIPLIER: int = 10
 
     def __init__(self, params: dict, rng=np.random.default_rng()) -> None:
         """"""
         self.rng = rng
 
         # - gen params
-        gen_params = params.get(
-            "gen", dict(
-                size = 20,
-                reproduce = 20,
-                random = 0
-            )
-        )
+        gen_params = params.get("gen", dict(size=20, reproduce=20, random=0))
         self.gen_size = gen_params.get("size", None)
-        assert isinstance(self.gen_size, int), "size of generaton needs to be an integer."
+        assert isinstance(
+            self.gen_size, int
+        ), "size of generaton needs to be an integer."
 
         self.gen_ran_size = gen_params.get("random", 0)
-        self.gen_ran_max_try = gen_params.get("max_random_try", self.gen_ran_size*self.MAX_ATTEMPTS_MULTIPLIER)
+        self.gen_ran_max_try = gen_params.get(
+            "max_random_try", self.gen_ran_size * self.MAX_ATTEMPTS_MULTIPLIER
+        )
 
-        self.gen_rep_size = gen_params.get("reprod", self.gen_size-self.gen_ran_size)
-        self.gen_rep_max_try = gen_params.get("max_reprod_try", self.gen_rep_size*self.MAX_ATTEMPTS_MULTIPLIER)
+        self.gen_rep_size = gen_params.get("reprod", self.gen_size - self.gen_ran_size)
+        self.gen_rep_max_try = gen_params.get(
+            "max_reprod_try", self.gen_rep_size * self.MAX_ATTEMPTS_MULTIPLIER
+        )
 
-        self.gen_mut_size = gen_params.get("mutate", self.gen_size-self.gen_ran_size-self.gen_rep_size)
+        self.gen_mut_size = gen_params.get(
+            "mutate", self.gen_size - self.gen_ran_size - self.gen_rep_size
+        )
 
         # - init params
-        init_params = params.get(
-            "init", dict(
-                size = 20,
-                seed_file = None
-            )
-        )
+        init_params = params.get("init", dict(size=20, seed_file=None))
         self.init_size = init_params.get("size", None)
         self.init_seed_file = init_params.get("seed_file", None)
 
         # - check if params were valid
-        assert (self.gen_rep_size+self.gen_ran_size+self.gen_mut_size) == self.gen_size, "In each generation, the sum of each component does not equal the total size."
-        assert self.gen_ran_size <= self.gen_size, "In each generation, the random size should not be larger than the total size."
-        assert self.gen_rep_size <= self.gen_size, "In each generation, the reprod size should not be larger than the total size."
-        assert self.gen_mut_size <= self.gen_size, "In each generation, the mutate size should not be larger than the total size."
+        assert (
+            self.gen_rep_size + self.gen_ran_size + self.gen_mut_size
+        ) == self.gen_size, "In each generation, the sum of each component does not equal the total size."
+        assert (
+            self.gen_ran_size <= self.gen_size
+        ), "In each generation, the random size should not be larger than the total size."
+        assert (
+            self.gen_rep_size <= self.gen_size
+        ), "In each generation, the reprod size should not be larger than the total size."
+        assert (
+            self.gen_mut_size <= self.gen_size
+        ), "In each generation, the mutate size should not be larger than the total size."
 
         # - mutation
         self.pmut = params.get("pmut", 0.5)
 
         return
-    
+
     def _get_current_candidates(self, database: DataConnection, curr_gen: int):
         """Get offsprings in the current generation.
 
         Mutataed candidates do not have `generation` keyword.
 
         Args:
             database: DataConnection.
             curr_gen: The current generation number.
 
         """
         candidate_groups = {"paired": [], "random": [], "mutated": []}
         num_paired, num_mutated, num_random = 0, 0, 0
 
-        #unrelaxed_strus_gen_ = list(database.c.select(f"relaxed=0"))
-        unrelaxed_strus_gen_ = list(database.c.select(f"relaxed=0,generation={curr_gen}"))
+        # unrelaxed_strus_gen_ = list(database.c.select(f"relaxed=0"))
+        unrelaxed_strus_gen_ = list(
+            database.c.select(f"relaxed=0,generation={curr_gen}")
+        )
         for row in unrelaxed_strus_gen_:
             if row.formula:
-                #print(row["gaid"], row)
+                # print(row["gaid"], row)
                 confid = row["gaid"]
-                curr_rows = sorted(database.c.select(f"relaxed=0,gaid={confid}"), key=lambda x: x.mtime)
+                curr_rows = sorted(
+                    database.c.select(f"relaxed=0,gaid={confid}"), key=lambda x: x.mtime
+                )
                 curr_rows = [x for x in curr_rows if x.formula]
                 # - get atoms
                 curr_atoms = database.get_atoms(curr_rows[-1].id, add_info=True)
                 # NOTE: candidates should not have description info...
                 #       otherwise, queued row also has them and failed in
                 #       database.c.get_participation_in_pairing()
-                kvp = {k: v for k, v in curr_atoms.info["key_value_pairs"].items() if k in RETAINED_KEYS}
-                data = curr_atoms.info.get("data", {}) # not every cand has data that stores parents
-                curr_atoms.info = {"key_value_pairs": kvp, "data": data, "confid": confid}
-                #print(curr_atoms)
+                kvp = {
+                    k: v
+                    for k, v in curr_atoms.info["key_value_pairs"].items()
+                    if k in RETAINED_KEYS
+                }
+                data = curr_atoms.info.get(
+                    "data", {}
+                )  # not every cand has data that stores parents
+                curr_atoms.info = {
+                    "key_value_pairs": kvp,
+                    "data": data,
+                    "confid": confid,
+                }
+                # print(curr_atoms)
                 # - count and add atoms
                 if "Pairing" in curr_rows[0]["origin"]:
                     num_paired += 1
                     candidate_groups["paired"].append(curr_atoms)
                 elif "Mutation" in curr_rows[0]["origin"]:
                     num_mutated += 1
                     candidate_groups["mutated"].append(curr_atoms)
                 elif "Random" in curr_rows[0]["origin"]:
                     num_random += 1
                     candidate_groups["random"].append(curr_atoms)
                 else:
                     ...
 
         return candidate_groups, num_paired, num_mutated, num_random
-    
-    def _prepare_initial_population(
-            self, generator
-        ) -> List[Atoms]:
-        self._print("\n\n===== Prepare Initial Population =====")
+
+    def _prepare_initial_population(self, generator) -> List[Atoms]:
+        self._print("===== Prepare Initial Population =====")
         starting_population = []
 
         # - try to read seed structures
         # NOTE: seed structures would be re-optimised by the worker
-        self._print("\n----- try to add seed structures -----")
+        self._print("----- try to add seed structures -----")
         seed_frames = []
         if self.init_seed_file is not None:
             self._print(str(self.init_seed_file))
             if isinstance(self.init_seed_file, str):
                 seed_frames = read(self.init_seed_file, ":")
             elif isinstance(self.init_seed_file, pathlib.Path):
                 seed_frames = read(self.init_seed_file, ":")
-            elif isinstance(self.init_seed_file, list): # List[Atoms]
+            elif isinstance(self.init_seed_file, list):  # List[Atoms]
                 seed_frames = self.init_seed_file
             else:
-                raise RuntimeError(f"Init_seed_file {self.init_seed_file} formst is unsuppoted.")
+                raise RuntimeError(
+                    f"Init_seed_file {self.init_seed_file} formst is unsuppoted."
+                )
             seed_frames = clean_seed_structures(seed_frames)
             seed_size = len(seed_frames)
             self._print(f"number of seed frames: {seed_size}")
-            assert (seed_size > 0 and seed_size <= self.init_size), "The number of seed structures is invalid."
+            assert (
+                seed_size > 0 and seed_size <= self.init_size
+            ), "The number of seed structures is invalid."
         else:
             seed_size = 0
 
         # TODO: seed structures will be calculated again??
         # TODO: check atom permutation
         for i, atoms in enumerate(seed_frames):
             # TODO: check atom order
@@ -211,186 +232,226 @@
             atoms.info["key_value_pairs"]["origin"] = "seed {}".format(i)
             atoms.info["key_value_pairs"]["raw_score"] = -atoms.get_potential_energy()
             # TODO: check geometric convergence
         self._print(f"number of seed structures: {len(seed_frames)}")
         starting_population.extend(seed_frames)
 
         # - generate random structures
-        self._print("\n----- try to generate random structures -----")
+        self._print("----- try to generate random structures -----")
         random_frames = generator.run(size=self.init_size - seed_size)
         self._print(f"number of random structures: {len(random_frames)}")
         starting_population.extend(random_frames)
 
         if len(starting_population) != self.init_size:
-            raise RuntimeError("It fails to generate the initial population. Check the seed file and the system setting.")
+            raise RuntimeError(
+                "It fails to generate the initial population. Check the seed file and the system setting."
+            )
 
         self._print(f"finished creating initial population...")
 
         return starting_population
 
     def _prepare_current_population(
-        self, database: DataConnection, curr_gen, population, generator, pairing, mutations,
-        candidate_groups: dict={}, num_paired=0, num_mutated=0, num_random=0,
+        self,
+        database: DataConnection,
+        curr_gen,
+        population,
+        generator,
+        pairing,
+        mutations,
+        candidate_groups: dict = {},
+        num_paired=0,
+        num_mutated=0,
+        num_random=0,
     ):
         """Prepare current population.
 
-        Usually, it should be the same as the initial size. However, for variat 
+        Usually, it should be the same as the initial size. However, for variat
         composition search, a large init size can be useful.
 
         """
         current_candidates = []
 
         # - reproduction and then mutation
         rest_rep_size = self.gen_rep_size - num_paired
         paired_structures = []
         paired_structures.extend(candidate_groups.get("paired", []))
-        if rest_rep_size > 0 and num_random == 0: 
+        if rest_rep_size > 0 and num_random == 0:
             # pair finished but not enough, random already starts...
             for i in range(self.gen_rep_max_try):
                 atoms = self._reproduce(database, population, pairing, mutations)
                 if atoms is not None:
                     paired_structures.append(atoms)
                     self._print(f"  --> {atoms.info}")
-                    self._print("  --> confid %d\n" %(atoms.info["confid"]))
+                    self._print("  --> confid %d\n" % (atoms.info["confid"]))
                 if len(paired_structures) == self.gen_rep_size:
                     break
             else:
-                self._print(f"There is not enough paired structures after {self.gen_rep_max_try} attempts.")
+                self._print(
+                    f"There is not enough paired structures after {self.gen_rep_max_try} attempts."
+                )
         else:
             ...
         current_candidates.extend(paired_structures)
 
         # - random
         if len(paired_structures) < self.gen_rep_size:
             self._print("There is not enough reproduced (paired) structures.")
-            self._print(f"Only {len(paired_structures)} are reproduced. The rest would be generated randomly.")
+            self._print(
+                f"Only {len(paired_structures)} are reproduced. The rest would be generated randomly."
+            )
             curr_ran_size = self.gen_size - len(paired_structures) - self.gen_mut_size
         else:
             curr_ran_size = self.gen_ran_size
 
         rest_ran_size = curr_ran_size - num_random
-        gen_ran_max_try = rest_ran_size*self.MAX_ATTEMPTS_MULTIPLIER
+        gen_ran_max_try = rest_ran_size * self.MAX_ATTEMPTS_MULTIPLIER
 
         random_structures = []
         random_structures.extend(candidate_groups.get("random", []))
         if rest_ran_size > 0 and num_mutated == 0:
             # random finished but not enough, mutation already starts...
             for i in range(gen_ran_max_try):
                 frames = generator.run(size=1, soft_error=True)
                 if frames:
                     atoms = frames[0]
                     self._print("  reproduce randomly ")
                     atoms.info["key_value_pairs"] = {
-                        "extinct": 0, "origin": "RandomCandidateUnrelaxed"
+                        "extinct": 0,
+                        "origin": "RandomCandidateUnrelaxed",
                     }
                     atoms.info["data"] = {}
                     confid = database.c.write(
-                        atoms, origin="RandomCandidateUnrelaxed",
-                        relaxed=0, extinct=0, generation=curr_gen, 
-                        key_value_pairs=atoms.info["key_value_pairs"], 
-                        data=atoms.info["data"]
+                        atoms,
+                        origin="RandomCandidateUnrelaxed",
+                        relaxed=0,
+                        extinct=0,
+                        generation=curr_gen,
+                        key_value_pairs=atoms.info["key_value_pairs"],
+                        data=atoms.info["data"],
                     )
                     database.c.update(confid, gaid=confid)
                     atoms.info["confid"] = confid
 
-                    self._print("  --> confid %d\n" %(atoms.info["confid"]))
+                    self._print("  --> confid %d\n" % (atoms.info["confid"]))
                     random_structures.append(atoms)
                 if len(random_structures) == curr_ran_size:
                     break
             else:
-                if self.gen_ran_size > 0: # NOTE: no break when random size is 0
-                    self._print(f"There is not enough random structures after {self.gen_ran_max_try} attempts.")
+                if self.gen_ran_size > 0:  # NOTE: no break when random size is 0
+                    self._print(
+                        f"There is not enough random structures after {self.gen_ran_max_try} attempts."
+                    )
         else:
             ...
         current_candidates.extend(random_structures)
 
         # - mutate
-        if len(current_candidates) < (self.gen_rep_size+self.gen_ran_size):
+        if len(current_candidates) < (self.gen_rep_size + self.gen_ran_size):
             self._print("There is not enough reproduced+random structures.")
-            self._print(f"Only {len(current_candidates)} are generated. The rest would be generated by mutations.")
+            self._print(
+                f"Only {len(current_candidates)} are generated. The rest would be generated by mutations."
+            )
             curr_mut_size = self.gen_size - len(current_candidates)
         else:
             curr_mut_size = self.gen_mut_size
 
         rest_mut_size = curr_mut_size - num_mutated
-        gen_mut_max_try = rest_mut_size*self.MAX_ATTEMPTS_MULTIPLIER
+        gen_mut_max_try = rest_mut_size * self.MAX_ATTEMPTS_MULTIPLIER
 
         mutated_structures = []
         mutated_structures.extend(candidate_groups.get("mutated", []))
         for i in range(gen_mut_max_try):
             atoms = population.get_one_candidate(with_history=True)
             a3, desc = mutations.get_new_individual([atoms])
             if atoms is not None:
                 database.add_unrelaxed_step(a3, desc)
                 self._print("  Mutate cand{} by {}".format(atoms.info["confid"], desc))
-                self._print("  --> confid %d\n" %(a3.info["confid"]))
+                self._print("  --> confid %d\n" % (a3.info["confid"]))
                 mutated_structures.append(a3)
             if len(mutated_structures) == curr_mut_size:
                 break
         else:
-            if self.gen_mut_size > 0: # NOTE: no break when random size is 0
-                self._print(f"There is not enough mutated structures after {gen_mut_max_try} attempts.")
+            if self.gen_mut_size > 0:  # NOTE: no break when random size is 0
+                self._print(
+                    f"There is not enough mutated structures after {gen_mut_max_try} attempts."
+                )
         current_candidates.extend(mutated_structures)
 
         if len(current_candidates) != self.gen_size:
             self._print("Not enough candidates for the next generation.")
             raise RuntimeError("Not enough candidates for the next generation.")
 
         return current_candidates
-    
+
     def _update_generation_settings(self, population, mutations, pairing):
         """Update some generation-specific settings."""
         # - operations at the end of each generation
         cur_pop = population.get_current_population()
-        #find_strain = False
-        #from ase.ga.standardmutations import StrainMutation
+        # find_strain = False
+        # from ase.ga.standardmutations import StrainMutation
         for mut in mutations.oplist:
-            #if issubclass(mut, StrainMutation):
+            # if issubclass(mut, StrainMutation):
             #    find_strain = True
             #    mut.update_scaling_volume(cur_pop, w_adapt=0.5, n_adapt=0)
             #    self._print(f"StrainMutation Scaling Volume: {mut.scaling_volume}")
             if hasattr(mut, "update_scaling_volume"):
                 mut.update_scaling_volume(cur_pop, w_adapt=0.5, n_adapt=0)
-                self._print(f"{mut.__class__.__name__} Scaling Volume: {mut.scaling_volume}")
+                self._print(
+                    f"{mut.__class__.__name__} Scaling Volume: {mut.scaling_volume}"
+                )
         if hasattr(pairing, "update_scaling_volume"):
             pairing.update_scaling_volume(cur_pop, w_adapt=0.5, n_adapt=0)
-            self._print(f"{pairing.__class__.__name__} Scaling Volume: {pairing.scaling_volume}")
-        
+            self._print(
+                f"{pairing.__class__.__name__} Scaling Volume: {pairing.scaling_volume}"
+            )
+
         return
-    
+
     def _reproduce(self, database, population, pairing, mutations) -> Atoms:
         """Reproduce a structure from the current population."""
         a3 = None
         for i in range(self.MAX_REPROC_TRY):
             # try 10 times
             parents = population.get_two_candidates()
-            a3, desc = pairing.get_new_individual(parents) # NOTE: this also adds key_value_pairs to a.info
+            a3, desc = pairing.get_new_individual(
+                parents
+            )  # NOTE: this also adds key_value_pairs to a.info
             if a3 is not None:
                 database.add_unrelaxed_candidate(
-                    a3, description=desc # here, desc is used to add "pairing": 1 to database
-                ) # if mutation happens, it will not be relaxed
+                    a3,
+                    description=desc,  # here, desc is used to add "pairing": 1 to database
+                )  # if mutation happens, it will not be relaxed
 
                 mut_desc = ""
                 curr_prob = self.rng.random()
                 if curr_prob < self.pmut:
                     a3_mut, mut_desc = mutations.get_new_individual([a3])
                     if a3_mut is not None:
                         self._print(f"a3_mut: {a3_mut.info}")
                         database.add_unrelaxed_step(a3_mut, mut_desc)
-                        #write("./pairs.xyz", a3, append=True)
-                        #write("./muts.xyz", a3_mut, append=True)
+                        # write("./pairs.xyz", a3, append=True)
+                        # write("./muts.xyz", a3_mut, append=True)
                         a3 = a3_mut
                     else:
                         mut_desc = ""
-                self._print(f"  reproduce offspring with {desc} and ({curr_prob}) {mut_desc} after {i+1} attempts..." )
+                self._print(
+                    f"  reproduce offspring with {desc} and ({curr_prob}) {mut_desc} after {i+1} attempts..."
+                )
                 break
             else:
                 mut_desc = ""
-                self._print(f"  failed to reproduce offspring with {desc} {mut_desc} after {i+1} attempts..." )
+                self._print(
+                    f"  failed to reproduce offspring with {desc} {mut_desc} after {i+1} attempts..."
+                )
         else:
-            self._print("cannot reproduce offspring a3 after {0} attempts".format(self.MAX_REPROC_TRY))
+            self._print(
+                "cannot reproduce offspring a3 after {0} attempts".format(
+                    self.MAX_REPROC_TRY
+                )
+            )
 
         return a3
 
 
 if __name__ == "__main__":
-    pass
+    pass
```

### Comparing `gdpx-0.0.6/src/gdpx/expedition/interface.py` & `gdpx-0.0.7/src/gdpx/expedition/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/basin_hopping.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/basin_hopping.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/monte_carlo.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/monte_carlo.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from .. import dict2str
 from ..expedition import AbstractExpedition
 from .operators import select_operator, parse_operators, save_operator, load_operator
 
 """This module tries to offer a base class for all MonteCarlo-like methods.
 """
 
+MC_EARLYSTOP_FNAME = "MC_EARLY_STOPPED"
+
 
 def convert_blmin_to_str(blmin: dict) -> str:
     """"""
     elements = []
     for k in blmin.keys():
         elements.extend(k)
     elements = set(elements)
@@ -107,20 +109,14 @@
             builder = registers.create(
                 "builder", builder_method, convert_name=False, **builder_params
             )
         else:
             builder = builder
         self.builder = builder
 
-        frames = builder.run()
-        assert (
-            len(frames) == 1
-        ), f"{self.__class__.__name__} only accepts one structure."
-        self.atoms = frames[0]
-
         # - create worker
         self.worker = None
 
         # - parse operators
         self.operators, self.op_probs = parse_operators(operators)
 
         # - parse convergence
@@ -189,29 +185,27 @@
                 )
             step_converged = True
         else:
             step_converged = False
 
         return step_converged
 
-    def _attach_bond_length_minimum_list(
-        self,
-    ):
-        """"""
+    def _attach_bond_length_minimum_list(self):
+        """Find possible elements in the simulation and build a bond-distance list."""
         type_list = []
         for op in self.operators:
             # TODO: wee need further unify the names here
             if hasattr(op, "particles"):
                 for p in op.particles:
                     type_list.extend(list(Formula(p).count().keys()))
             elif hasattr(op, "reservoir"):
                 type_list.extend(list(Formula(op.reservoir["species"]).count().keys()))
             else:
                 ...
-        type_list = list(set(type_list))
+        type_list = list(set(type_list + self.atoms.get_chemical_symbols()))
         self._print(f"{type_list =}")
         unique_atomic_numbers = [data.atomic_numbers[a] for a in type_list]
 
         for op in self.operators:
             op.blmin = closest_distances_generator(
                 atom_numbers=unique_atomic_numbers,
                 ratio_of_covalent_radii=op.covalent_min,
@@ -236,14 +230,23 @@
             self._print("Convert a DriverBasedWorker to a SingleWorker.")
             self.worker = SingleWorker.from_a_worker(self.worker)
         assert isinstance(
             self.worker, SingleWorker
         ), f"{self.__class__.__name__} only supports SingleWorker (set use_single=True)."
         self.worker.directory = self.directory
 
+        # - create an atoms during the run-time
+        #   If it is created in init, it will be re-used in active-learning loop.
+        #   Thus, we create a new one every run time.
+        frames = self.builder.run()
+        assert (
+            len(frames) == 1
+        ), f"{self.__class__.__name__} only accepts one structure."
+        self.atoms = frames[0]
+
         # - prepare logger and output some basic info...
         if not self.directory.exists():
             self.directory.mkdir(parents=True)
 
         # - show operator information
         self._print("===== MonteCarlo Operators (Modifiers) =====\n")
 
@@ -287,31 +290,43 @@
                 return
             else:
                 self.start_step += 1
 
             # - run mc steps
             curr_step = self.start_step  # start_step
             while True:
+                # -- check exit-loop conditions
                 if curr_step > self.convergence["steps"]:
+                    self._print("Monte Carlo reaches the maximum step.")
+                    break
+                if (self.directory/MC_EARLYSTOP_FNAME).exists():
+                    self._print("Monte Carlo reaches the earlystopping.")
                     break
+                # -- run step
                 step_state = self._irun(curr_step)
+                # -- state-specific
                 if step_state == "UNFINISHED":
                     self._print("Wait MC step to finish.")
                     break
                 elif step_state == "FINISHED":
                     # -- save checkpoint
                     self._save_checkpoint(step=curr_step)
                     # -- clean up
                     if (
                         (self.directory / f"{self.WDIR_PREFIX}{curr_step}").exists()
                     ) and (curr_step % self.dump_period != 0):
                         shutil.rmtree(self.directory / f"{self.WDIR_PREFIX}{curr_step}")
                     curr_step += 1
                 elif step_state == "FAILED":
                     self._print(f"RETRY STEP {curr_step}.")
+                elif step_state == "EARLYSTOPPED":
+                    # We need a file flag to indicate the simutlation is finshed
+                    # when read_convergence is called.
+                    with open(self.directory/MC_EARLYSTOP_FNAME, "w") as fopen:
+                        fopen.write(f"{step_state =}")
                 else:
                     ...  # This should not happen.
         else:
             self._print("Monte Carlo is converged.")
 
         return
 
@@ -368,22 +383,49 @@
                     self.atoms = curr_atoms
                     self._print("success...")
                 else:
                     self._print("failure...")
                 write(self.directory / self.TRAJ_NAME, self.atoms, append=True)
 
                 step_state = "FINISHED"
+
+                # -- check earlystopping
+                step_state = self._check_earlystop(self.atoms)
             else:
                 step_state = "UNFINISHED"
         else:
             # save the previous structure as the current operation gives no structure.
             step_state = "FAILED"
 
         return step_state
 
+    def _check_earlystop(self, atoms: Atoms) -> str:
+        """Check whether earlystopping should be done to avoid unphysical structures.
+
+        Returns:
+            A state string `FINISHED` or `EARLYSTOPPED`.
+
+        """
+        es_dict = self.convergence.get("earlystop", None)
+        if es_dict is not None:
+            prop = es_dict.get("property", None)
+            if prop == "energy_per_atom":
+                ae_min, ae_max = es_dict["range"]
+                energy_per_atom = atoms.get_potential_energy() / len(atoms)
+                if ae_min <= energy_per_atom < ae_max:
+                    es_state = "FINISHED"
+                else:
+                    es_state = "EARLYSTOPPED"
+            else:
+                raise NotImplementedError(f"Unknown earlystop: {es_dict =}.")
+        else:
+            es_state = "FINISHED"
+
+        return es_state
+
     def _veri_checkpoint(self) -> bool:
         """Verify checkpoints."""
         ckpt_wdirs = list(self.directory.glob("checkpoint.*"))
         nwdirs = len(ckpt_wdirs)
 
         verified = True
         if nwdirs > 0:
@@ -491,14 +533,16 @@
         converged = False
         if (self.directory / self.TRAJ_NAME).exists():
             mctraj = read(self.directory / self.TRAJ_NAME, ":")
             nframes = len(mctraj)
             # self.start_step = nframes
             if nframes > self.convergence["steps"]:
                 converged = True
+            if (self.directory/MC_EARLYSTOP_FNAME).exists():
+                converged = True
         else:
             ...
 
         return converged
 
     def get_workers(self):
         """Get all workers used by this expedition."""
```

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/__init__.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/exchange.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/exchange.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/move.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/move.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/operator.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/operator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/react.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/react.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/swap.py` & `gdpx-0.0.7/src/gdpx/expedition/monte_carlo/operators/swap.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/expedition/simulated_annealing/simulated_annealing.py` & `gdpx-0.0.7/src/gdpx/expedition/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/comparison.py` & `gdpx-0.0.7/src/gdpx/graph/comparison.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/creator.py` & `gdpx-0.0.7/src/gdpx/graph/creator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/graph_main.py` & `gdpx-0.0.7/src/gdpx/graph/graph_main.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/molecule.py` & `gdpx-0.0.7/src/gdpx/graph/molecule.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/sites.py` & `gdpx-0.0.7/src/gdpx/graph/sites.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/surface.py` & `gdpx-0.0.7/src/gdpx/graph/surface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/graph/utils.py` & `gdpx-0.0.7/src/gdpx/graph/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/main.py` & `gdpx-0.0.7/src/gdpx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,16 @@
         help="a structure file that stores one or more structures"
     )
     parser_compute.add_argument(
         "-b", "--batch", default=None, type=int,
         help="run selected batch number (useful when queue run)"
     )
     parser_compute.add_argument(
-        "-o", "--output", default="last", choices=["last","traj"],
-        help="retrieve last frame or entire trajectory"
-    )
-    parser_compute.add_argument(
         "--spawn", action="store_true",
-        help="If the computation is spawned, it will not save results when all jobs are finished."
+        help="If the computation is spawned, it will not save results until all jobs are finished."
     )
     parser_compute.add_argument(
         "--archive", action="store_true",
         help="whether archive computation folders when retrieve"
     )
 
     # --- expedition interface
@@ -251,18 +247,18 @@
         build_config = parse_input_file(args.CONFIG)
         from .builder.interface import build_structures
         build_structures(build_config, args.substrates, args.number, args.directory)
     elif args.subcommand == "select":
         from gdpx.selector.interface import run_selection
         run_selection(args.CONFIG, args.structure, args.directory)
     elif args.subcommand == "compute":
-        from gdpx.worker.interface import run_worker
+        from .cli.compute import run_worker
         run_worker(
-            args.STRUCTURE, args.directory, potter, args.output, args.batch, 
-            args.spawn, args.archive
+            args.STRUCTURE, potter, batch=args.batch, 
+            spawn=args.spawn, archive=args.archive, directory=args.directory
         )
     elif args.subcommand == "explore":
         from .expedition.interface import run_expedition
         params = parse_input_file(args.CONFIG)
         run_expedition(params, args.wait, args.directory, potter)
     elif args.subcommand == "valid":
         from gdpx.validator import run_validation
```

### Comparing `gdpx-0.0.6/src/gdpx/nanoparticle.py` & `gdpx-0.0.7/src/gdpx/nanoparticle.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/calculators/dummy.py` & `gdpx-0.0.7/src/gdpx/potential/calculators/dummy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/calculators/mixer.py` & `gdpx-0.0.7/src/gdpx/potential/calculators/mixer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/interface.py` & `gdpx-0.0.7/src/gdpx/potential/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/manager.py` & `gdpx-0.0.7/src/gdpx/potential/manager.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/__init__.py` & `gdpx-0.0.7/src/gdpx/potential/managers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,17 @@
 from .espresso import EspressoManager
 registers.manager.register(EspressoManager)
 
 from .vasp import VaspManager
 registers.manager.register(VaspManager)
 
 # --- FFs
+from .asepot import AsePotManager
+registers.manager.register("AseManager")(AsePotManager)
+
 from .eam import EamManager
 registers.manager.register(EamManager)
 
 from .emt import EmtManager
 registers.manager.register(EmtManager)
 
 from .reax import ReaxManager
@@ -102,8 +105,8 @@
 
 from .gp.sgp import SGPTrainer
 registers.trainer.register("SgpTrainer")(SGPTrainer)
 
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/bias.py` & `gdpx-0.0.7/src/gdpx/potential/managers/bias.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 
 import copy
 
 from . import registers
 from . import AbstractPotentialManager, DummyCalculator
-from gdpx.bias import bias_register
 
-"""This manager registers ALL jax-based bias calculators."""
+
+"""This manager registers ALL bias calculators."""
 
 
 class BiasManager(AbstractPotentialManager):
 
     name = "bias"
     implemented_backends = ["ase"]
 
@@ -22,15 +22,15 @@
     ]
 
     def __init__(self) -> None:
         """"""
         super().__init__()
 
         return
-    
+
     def register_calculator(self, calc_params, *agrs, **kwargs) -> None:
         """"""
         super().register_calculator(calc_params, *agrs, **kwargs)
 
         # - parse params
         bias_type = calc_params.get("type", None)
         assert bias_type is not None, "Bias must have a type."
@@ -47,18 +47,19 @@
             ...
         if colvar_ is not None:
             calc_params["colvar"] = colvar_
 
         # - instantiate calculator
         calc = DummyCalculator()
         if self.calc_backend == "ase":
-            calc = bias_register[bias_type](**calc_params)
+            bias_cls = registers.bias[bias_type]
+            calc = bias_cls(**calc_params)
         else:
             ...
-        
+
         self.calc = calc
 
         return
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/cp2k.py` & `gdpx-0.0.7/src/gdpx/potential/managers/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/deepmd/calculator.py` & `gdpx-0.0.7/src/gdpx/potential/managers/deepmd/calculator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/deepmd/convert.py` & `gdpx-0.0.7/src/gdpx/potential/managers/deepmd/convert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/deepmd/deepmd.py` & `gdpx-0.0.7/src/gdpx/potential/managers/deepmd/deepmd.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/dftd3.py` & `gdpx-0.0.7/src/gdpx/potential/managers/dftd3.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/eam.py` & `gdpx-0.0.7/src/gdpx/potential/managers/eam.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/emt.py` & `gdpx-0.0.7/src/gdpx/potential/managers/emt.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/espresso.py` & `gdpx-0.0.7/src/gdpx/potential/managers/espresso.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/gp/bench.py` & `gdpx-0.0.7/src/gdpx/potential/managers/gp/bench.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/gp/fgp.py` & `gdpx-0.0.7/src/gdpx/potential/managers/gp/fgp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/gp/gptools.py` & `gdpx-0.0.7/src/gdpx/potential/managers/gp/gptools.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/gp/representation.py` & `gdpx-0.0.7/src/gdpx/potential/managers/gp/representation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/gp/sgp.py` & `gdpx-0.0.7/src/gdpx/potential/managers/gp/sgp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/grid.py` & `gdpx-0.0.7/src/gdpx/potential/managers/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/lasp.py` & `gdpx-0.0.7/src/gdpx/potential/managers/lasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/mace.py` & `gdpx-0.0.7/src/gdpx/potential/managers/mace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*
 
 
 import copy
 import itertools
 import pathlib
-from typing import Union, List
+import shutil
+from typing import Union, List, Optional
 
 
 from ase.io import read, write
 
 
 from . import AbstractPotentialManager, AbstractTrainer
 from . import DummyCalculator, CommitteeCalculator
@@ -152,32 +153,48 @@
             ...
 
         # - misc
         import torch
 
         train_config["device"] = "cuda" if torch.cuda.is_available() else "cpu"
 
-        train_config["restart_latest"] = True
+        restart_latest = train_config.get("restart_latest", True)
+        train_config["restart_latest"] = restart_latest
+
+        init_latest = train_config.get("init_latest", None)
+        if init_latest is not None and init_latest:
+            train_config["init_latest"] = init_latest
+            del train_config["restart_latest"]
 
         train_config["save_cpu"] = True
 
         # - pop unused...
         train_config.pop("log_dir", None)
         train_config.pop("model_dir", None)
         train_config.pop("checkpoints_dir", None)
         train_config.pop("results_dir", None)
 
         return train_config
 
+    def get_checkpoint(self):
+        """"""
+
+        return pathlib.Path(self.directory/"checkpoints").resolve()
+
     def _train_from_the_restart(self, dataset, init_model) -> str:
-        """Train from the restart"""
-        if init_model is not None:
-            raise NotImplementedError(
-                f"{self.name} does not support initialising from a previous model."
-            )
+        """Train from the restart.
+
+        Args:
+            init_model: The path of the checkpoints folder.
+
+        """
+        # if init_model is not None:
+        #     raise NotImplementedError(
+        #         f"{self.name} does not support initialising from a previous model."
+        #     )
 
         def _add_command_options(command, config) -> str:
             """"""
             # - convert to command line options...
             command = command + " "
             for k, v in config.items():
                 if isinstance(v, bool):
@@ -186,39 +203,98 @@
                 elif isinstance(v, int) or isinstance(v, float):
                     command += f"--{k}={str(v)}  "
                 else:
                     command += f"--{k}='{str(v)}'  "
 
             return command
 
+        def _check_latest_checkpoint(ckpt_dir, model_name) -> Optional[int]:
+            """"""
+            ckpts = [p for p in ckpt_dir.glob(f"{model_name}*")]
+            # ckpt_models = [c for c in ckpts if c.name.endswith(".model")]
+            ckpt_models = [c for c in ckpts if c.name.endswith(".pt")]
+            num_ckpts = len(ckpt_models)
+            assert num_ckpts <= 1
+            if num_ckpts == 1:
+                ckpt_model = ckpt_models[0]
+                prev_seed = int(ckpt_model.name.split("-")[1].split("_")[0])
+            else:
+                prev_seed = None
+
+            return prev_seed
+
+        def _get_latest_checkpoint(ckpt_dir, model_name):
+            """"""
+            ckpts = [p for p in ckpt_dir.glob(f"{model_name}*")]
+            ckpt_models = [c for c in ckpts if c.name.endswith(".pt")]
+            num_ckpts = len(ckpt_models)
+            assert num_ckpts <= 1
+            if num_ckpts == 1:
+                ckpt_model = ckpt_models[0]
+            else:
+                ckpt_model = None
+
+            return ckpt_model
+
+        # Check dataset type and convert it if necessary
+        dataset = self._prepare_dataset(dataset)
+
         train_config = self._update_config(dataset)
 
+        # make command
+        raw_command = self._train_from_the_scratch(dataset, init_model)
+
+        ckpt_dir = self.directory / "checkpoints"
         if not self.directory.exists():
-            command = self._train_from_the_scratch(dataset, init_model)
             if init_model is not None:
+                model_name = train_config["name"]
+                init_model = pathlib.Path(init_model)
+                assert init_model.name == "checkpoints"
+                self._print(f"init_model: {str(init_model)}")
+                ckpt_path = _get_latest_checkpoint(init_model, model_name)
+                if ckpt_path is not None:
+                    ckpt_dir.mkdir()
+                    curr_seed = train_config["seed"]
+                    (ckpt_dir/f"{model_name}_run-{curr_seed}_epoch-0.pt").symlink_to(ckpt_path)
+                    train_config.pop("restart_latest")
+                    train_config["init_latest"] = True
+                else:
+                    self._print(f"FAILED to init from `{str(init_model)}`.")
+            else:
+                # train from the scratch and no config needs update
                 ...
-            command = _add_command_options(command, train_config)
         else:
-            command = self._train_from_the_scratch(dataset, init_model)
-            ckpt_dir = self.directory / "checkpoints"
             if ckpt_dir.exists():
-                model_name = train_config["name"]
-                ckpts = [p for p in ckpt_dir.glob(f"{model_name}*")]
-                self._print(ckpts)
-                ckpt_models = [c for c in ckpts if c.name.endswith(".model")]
-                if len(ckpt_models) > 0:
-                    ckpt_model = ckpt_models[0]
-                    self._print(f"{ckpt_model =}")
-                    prev_seed = int(ckpt_model.name.split("-")[-1][:-6])
-                    self._print(f"{prev_seed =}")
+                # continue from the latest checkpoint
+                prev_seed = _check_latest_checkpoint(ckpt_dir, train_config["name"])
+                self._print(f"{prev_seed =}")
+                if prev_seed is not None:
                     train_config["seed"] = prev_seed
+                    train_config.pop("init_latest")
+                    train_config["restart_latest"] = True
             else:
-                # train from the scratch and no config needs update
-                ...
-            command = _add_command_options(command, train_config)
+                if init_model is not None:
+                    model_name = train_config["name"]
+                    init_model = pathlib.Path(init_model)
+                    assert init_model.name == "checkpoints"
+                    self._print(f"init_model: {str(init_model)}")
+                    ckpt_path = _get_latest_checkpoint(init_model, model_name)
+                    if ckpt_path is not None:
+                        ckpt_dir.mkdir()
+                        curr_seed = train_config["seed"]
+                        (ckpt_dir/f"{model_name}_run-{curr_seed}_epoch-0.pt").symlink_to(ckpt_path)
+                        train_config.pop("restart_latest")
+                        train_config["init_latest"] = True
+                    else:
+                        self._print(f"FAILED to init from `{str(init_model)}`.")
+                else:
+                    # train from the scratch and no config needs update
+                    ...
+
+        command = _add_command_options(raw_command, train_config)
 
         return command
 
     def _prepare_dataset(self, dataset, *args, **kwargs):
         """Prepare a reann dataset for training.
 
         Currently, it only supports converting xyz dataset.
@@ -279,17 +355,20 @@
 
         return converged
 
 
 class MaceManager(AbstractPotentialManager):
 
     name = "mace"
-    implemented_backends = ["ase"]
+    implemented_backends = ["ase", "jax"]
 
-    valid_combinations = (("ase", "ase"),)
+    valid_combinations = (
+        ("ase", "ase"),
+        ("jax", "ase"),
+    )
 
     def __init__(self):
         """"""
 
         return
 
     def register_calculator(self, calc_params, *agrs, **kwargs):
@@ -331,41 +410,65 @@
             try:
                 import torch
                 from mace.calculators import MACECalculator
             except:
                 raise ModuleNotFoundError(
                     "Please install mace and torch to use the ase interface."
                 )
+            device = "cuda" if torch.cuda.is_available() else "cpu"
+            # print(f"mace device: {device}")
             calcs = []
             for m in models:
                 # print("device", torch.device("cuda" if torch.cuda.is_available() else torch.device("cpu")))
                 curr_calc = MACECalculator(
                     model_paths=m,
-                    device="cuda" if torch.cuda.is_available() else "cpu",
+                    device=device,
                     default_dtype=precision,
                 )
                 calcs.append(curr_calc)
-            if len(calcs) == 1:
-                calc = calcs[0]
-            elif len(calcs) > 1:
-                if estimate_uncertainty:
-                    calc = CommitteeCalculator(calcs)
-                else:
-                    calc = calcs[0]
-            else:
-                ...
+            calc = self._process_committee(calcs, estimate_uncertainty)
+        elif self.calc_backend == "jax":
+            try:
+                import jax
+                from mace_jax.calculators.mace import MACEJAXCalculator
+            except:
+                raise ModuleNotFoundError(
+                    "Please install mace-jax and jax to use the jax interface."
+                )
+            # calcs = []
+            # for m in models:
+            #     curr_calc = MACEJAXCalculator(
+            #
+            #     )
+            raise NotImplementedError("The JAX backend for MACE is under development.")
         elif self.calc_backend == "lammps":
-            raise RuntimeError("The LAMMPS backend for MACE is under development.")
+            raise NotImplementedError(
+                "The LAMMPS backend for MACE is under development."
+            )
         else:
             ...
 
         self.calc = calc
 
         return
 
+    def _process_committee(self, calcs, estimate_uncertainty: bool):
+        """"""
+        if len(calcs) == 1:
+            calc = calcs[0]
+        elif len(calcs) > 1:
+            if estimate_uncertainty:
+                calc = CommitteeCalculator(calcs)
+            else:
+                calc = calcs[0]
+        else: # Empty list
+            calc = DummyCalculator()
+
+        return calc
+
     def switch_uncertainty_estimation(self, status: bool = True):
         """Switch on/off the uncertainty estimation."""
         # NOTE: Sometimes the manager loads several models and supports uncertainty
         #       by committee but the user disables it. We need change the calc to
         #       the correct one as the loaded one is just a single calculator.
         if not hasattr(self, "calc"):
             raise RuntimeError(
```

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/mixer.py` & `gdpx-0.0.7/src/gdpx/potential/managers/mixer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/nequip.py` & `gdpx-0.0.7/src/gdpx/potential/managers/nequip.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed.py` & `gdpx-0.0.7/src/gdpx/potential/managers/plumed/calculators/plumed.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed2.py` & `gdpx-0.0.7/src/gdpx/potential/managers/plumed/calculators/plumed2.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/plumed/plumed.py` & `gdpx-0.0.7/src/gdpx/potential/managers/plumed/plumed.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/reann/beann.py` & `gdpx-0.0.7/src/gdpx/potential/managers/reann/beann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/reann/calculators/reann.py` & `gdpx-0.0.7/src/gdpx/potential/managers/reann/calculators/reann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/reann/reann.py` & `gdpx-0.0.7/src/gdpx/potential/managers/reann/reann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/reax.py` & `gdpx-0.0.7/src/gdpx/potential/managers/reax.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/schnet.py` & `gdpx-0.0.7/src/gdpx/potential/managers/schnet.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/vasp.py` & `gdpx-0.0.7/src/gdpx/potential/managers/vasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/managers/xtb.py` & `gdpx-0.0.7/src/gdpx/potential/managers/xtb.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/potential/trainer.py` & `gdpx-0.0.7/src/gdpx/potential/trainer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/__init__.py` & `gdpx-0.0.7/src/gdpx/reactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/AccCons.py` & `gdpx-0.0.7/src/gdpx/reactor/future/AccCons.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/AccHop.py` & `gdpx-0.0.7/src/gdpx/expedition/accelerated_dynamics/prev_example.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/AccNEB.py` & `gdpx-0.0.7/src/gdpx/reactor/future/AccNEB.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/cmp_mep.py` & `gdpx-0.0.7/src/gdpx/reactor/future/cmp_mep.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/constrain.py` & `gdpx-0.0.7/src/gdpx/reactor/future/constrain.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/crs.py` & `gdpx-0.0.7/src/gdpx/reactor/future/crs.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/diffusion3.py` & `gdpx-0.0.7/src/gdpx/reactor/future/diffusion3.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/find_adsorption.py` & `gdpx-0.0.7/src/gdpx/reactor/future/find_adsorption.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/find_inter.py` & `gdpx-0.0.7/src/gdpx/reactor/future/find_inter.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/muller-brown.py` & `gdpx-0.0.7/src/gdpx/reactor/future/muller-brown.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/future/test_mh.py` & `gdpx-0.0.7/src/gdpx/reactor/future/test_mh.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/interface.py` & `gdpx-0.0.7/src/gdpx/utils/command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,219 +1,235 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import copy
 import time
-from typing import Optional, List, Mapping
-
-from ase import Atoms
+import subprocess
+from pathlib import Path
+from itertools import groupby
+from operator import itemgetter
+
+from typing import Any, Union, List
+
+import json
+import yaml
+
+
+def dict2str(d: dict, indent: int = 2):
+    """Convert a nested dict to str."""
+
+    def _dict2str(d_: dict, indent_: int):
+        """Recursive function."""
+        content = ""
+        for k, v in d_.items():
+            if isinstance(v, dict):
+                content += f"{k}:\n" + _dict2str(v, indent_ + indent)
+            else:
+                content += " " * indent_ + f"{k}: {v}\n"
 
-from ..core.register import registers
-from ..core.variable import Variable
-from ..core.operation import Operation
-from ..data.array import AtomsNDArray
-from ..worker.react import ReactorBasedWorker
+        return content
 
+    content = _dict2str(d, 0)
 
-@registers.variable.register
-class ReactorVariable(Variable):
+    return content
 
-    """Create a ReactorBasedWorker.
 
-    TODO:
-        Broadcast driver params to give several workers?
+class CustomTimer:
 
-    """
-
-    def __init__(self, potter, driver: dict, scheduler={}, batchsize=1, directory="./", *args, **kwargs):
+    def __init__(self, name="code", func=print):
         """"""
-        # - save state by all nodes
-        self.potter = self._load_potter(potter)
-        self.driver = self._load_driver(driver)
-        self.scheduler = self._load_scheduler(scheduler)
-
-        self.batchsize = batchsize
-
-        # - create a reactor
-        #reactor = self.potter.create_reactor(kwargs)
-        workers = self._create_workers(self.potter, self.driver, self.scheduler, self.batchsize)
-
-        super().__init__(initial_value=workers, directory=directory)
+        self.name = name
+        self._print = func
 
         return
 
-    def _load_potter(self, inp):
+    def __call__(self, func) -> Any:
         """"""
-        potter = None
-        if isinstance(inp, Variable):
-            potter = inp.value
-        elif isinstance(inp, dict):
-            potter_params = copy.deepcopy(inp)
-            name = potter_params.get("name", None)
-            potter = registers.create(
-                "manager", name, convert_name=True,
-            )
-            potter.register_calculator(potter_params.get("params", {}))
-            potter.version = potter_params.get("version", "unknown")
-        else:
-            raise RuntimeError(f"Unknown {inp} for the potter.")
 
-        return potter
-
-    def _load_driver(self, inp) -> List[dict]:
-        """Load drivers from a Variable or a dict."""
-        #print("driver: ", inp)
-        drivers = [] # params
-        if isinstance(inp, Variable):
-            drivers = inp.value
-        elif isinstance(inp, dict): # assume it only contains one driver
-            driver_params = copy.deepcopy(inp)
-            #driver = self.potter.create_driver(driver_params) # use external backend
-            drivers = [driver_params]
-        else:
-            raise RuntimeError(f"Unknown {inp} for drivers.")
-
-        return drivers
-
-    def _load_scheduler(self, inp):
-        """"""
-        scheduler = None
-        if isinstance(inp, Variable):
-            scheduler = inp.value
-        elif isinstance(inp, dict):
-            scheduler_params = copy.deepcopy(inp)
-            backend = scheduler_params.pop("backend", "local")
-            scheduler = registers.create(
-                "scheduler", backend, convert_name=True, **scheduler_params
+        def func_timer(*args, **kwargs):
+            st = time.time()
+            ret = func(*args, **kwargs)
+            et = time.time()
+            content = (
+                "*** " + self.name + " time: " + "{:>8.4f}".format(et - st) + " ***"
             )
-        else:
-            raise RuntimeError(f"Unknown {inp} for the scheduler.")
-
-        return scheduler
-    
-    def _create_workers(self, potter, drivers: List[dict], scheduler, batchsize: int=1, *args, **kwargs):
-        """"""
-        workers = []
-        for driver_params in drivers:
-            driver = potter.create_reactor(driver_params)
-            worker = ReactorBasedWorker(potter, driver, scheduler)
-            workers.append(worker)
-        
-        for worker in workers:
-            worker.batchsize = batchsize
-
-        return workers
-
+            self._print(content)
 
-@registers.operation.register
-class pair_stru(Operation):
+            return ret
 
-    status: str = "finished"
+        return func_timer
 
-    def __init__(self, structures, method="couple", pairs=None, directory="./") -> None:
+    def __enter__(self):
         """"""
-        super().__init__(input_nodes=[structures], directory=directory)
+        self.st = time.time()  # start time
 
-        assert method in ["couple", "concat", "custom"], "pair method should be either couple or concat."
-        self.method = method
-        self.pairs = pairs
+        return self
 
-        return
-    
-    def forward(self, structures: AtomsNDArray) -> List[List[Atoms]]:
+    def __exit__(self, *args):
         """"""
-        super().forward()
-
-        # NOTE: assume this is a 1-D array
-        print(f"structures: {structures}")
-        intermediates = structures.get_marked_structures()
-
-        nframes = len(intermediates)
-        rankings = list(range(nframes))
-
-        if self.method == "couple":
-            pair_indices = [rankings[0::2], rankings[1::2]]
-        elif self.method == "concat":
-            pair_indices = [rankings[:-1], rankings[1:]]
-        elif self.method == "custom":
-            pair_indices = self.pairs
-        else:
-            ...
+        self.et = time.time()  # end time
 
-        pair_structures = []
-        for p in pair_indices:
-            pair_structures.append([intermediates[i] for i in p])
-
-        return AtomsNDArray(pair_structures)
+        content = (
+            "*** "
+            + self.name
+            + " time: "
+            + "{:>8.4f}".format(self.et - self.st)
+            + " ***"
+        )
+        self._print(content)
 
+        return
 
-@registers.operation.register
-class react(Operation):
 
-    def __init__(self, structures, reactor, batchsize: Optional[int]=None, directory="./") -> None:
-        """"""
-        super().__init__(input_nodes=[structures, reactor], directory=directory)
+def check_path(target_dir: Union[str, Path]) -> bool:
+    """check path existence, if so skip the following
+    TODO: add output option
+    make this into a context?
+    """
+    target_dir = Path(target_dir)
+    if not target_dir.exists():
+        target_dir.mkdir(parents=True)
+    else:
+        print(f"  {target_dir.name} exists, so next...")
+
+    return
 
-        self.batchsize = batchsize
 
-        return
-    
-    def forward(self, structures: List[AtomsNDArray], reactors):
-        """"""
-        super().forward()
-
-        if isinstance(structures, list):
-            # - from list_nodes operation
-            structures = AtomsNDArray([x.tolist() for x in structures])
-        else:
-            # - from pair operation
-            structures = AtomsNDArray(structures)
-        print(f"structures: {structures}")
-        print(f"structures: {structures[0]}")
-
-        # - assume structures contain a List of trajectory/frames pair
-        #   take the last frame out since it is minimised?
-        #structures = [[x[-1] for x in s] for s in structures]
-        nreactions = len(structures)
-
-        # - create reactors
-        for i, reactor in enumerate(reactors):
-            reactor.directory = self.directory / f"r{i}"
-            if self.batchsize is not None:
-                reactor.batchsize = self.batchsize
+def find_backups(dpath, fname, prefix="bak"):
+    """find a series of files in a dir
+    such as fname, bak.0.fname, bak.1.fname
+    """
+    dpath = Path(dpath)
+    fpath = dpath / fname
+    if not fpath.exists():
+        raise FileNotFoundError(f"fpath does not exist.")
+
+    backups = list(dpath.glob(prefix + ".[0-9]*." + fname))
+    backups = sorted(backups, key=lambda x: int(x.name.split(".")[1]))
+    backups.append(fpath)
+
+    return backups
+
+
+def run_command(directory, command, comment="", timeout=None):
+    proc = subprocess.Popen(
+        command,
+        shell=True,
+        cwd=directory,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        encoding="utf-8",
+    )
+    if timeout is None:
+        errorcode = proc.wait()
+    else:
+        errorcode = proc.wait(timeout=timeout)
+
+    msg = "Message: " + "".join(proc.stdout.readlines())
+    print(msg)
+    if errorcode:
+        raise RuntimeError("Error in %s at %s." % (comment, directory))
+
+    return msg
+
+
+def convert_indices(indices: Union[str, List[int]], index_convention="lmp"):
+    """parse indices for reading xyz by ase, get start for counting
+    constrained indices followed by lammps convention
+    "2:4 3:8"
+    convert [1,2,3,6,7,8] to "1:3 6:8"
+    lammps convention starts from 1 and includes end
+    ---
+    input can be either py or lmp
+    output for indices is in py since it can be used to access atoms
+    output for text is in lmp since it can be used in lammps or sth
+    """
+    ret = []
+    if isinstance(indices, str):
+        # string to List[int]
+        for x in indices.strip().split():
+            cur_range = list(map(int, x.split(":")))
+            if len(cur_range) == 1:
+                start, end = cur_range[0], cur_range[0]
             else:
-                reactor.batchsize = nreactions
-        nreactors = len(reactors)
-
-        if nreactors == 1:
-            reactors[0].directory = self.directory
+                start, end = cur_range
+            if index_convention == "lmp":
+                ret.extend([i - 1 for i in list(range(start, end + 1))])
+            elif index_convention == "py":
+                ret.extend(list(range(start, end)))
+            else:
+                pass
+    elif isinstance(indices, list):
+        # List[int] to string
+        indices = sorted(indices)
+        if index_convention == "lmp":
+            pass
+        elif index_convention == "py":
+            indices = [i + 1 for i in indices]
+        ret = []
+        # ranges = []
+        for k, g in groupby(enumerate(indices), lambda x: x[0] - x[1]):
+            group = map(itemgetter(1), g)
+            group = list(map(int, group))
+            # ranges.append((group[0],group[-1]))
+            if group[0] == group[-1]:
+                ret.append(str(group[0]))
+            else:
+                ret.append("{}:{}".format(group[0], group[-1]))
+        ret = " ".join(ret)
+    else:
+        pass
+
+    return ret
+
+
+def parse_input_file(
+    input_fpath: Union[str, Path],
+    write_json: bool = False,  # write readin dict to check if alright
+):
+    """"""
+    input_dict = None
+
+    # - parse input type
+    if isinstance(input_fpath, dict):
+        input_dict = input_fpath
+        json_path = Path.cwd()
+    else:
+        if isinstance(input_fpath, str):
+            input_file = Path(input_fpath)
+            json_path = input_file.parent
+        elif isinstance(input_fpath, Path):
+            input_file = input_fpath
+            json_path = input_file.parent
+        else:
+            return None
 
-        # - align structures
-        reactor_status = []
-        for i, reactor in enumerate(reactors):
-            flag_fpath = reactor.directory/"FINISHED"
-            self._print(f"run reactor {i} for {nreactions} nframes")
-            if not flag_fpath.exists():
-                reactor.run(structures)
-                reactor.inspect(resubmit=True)
-                if reactor.get_number_of_running_jobs() == 0:
-                    with open(flag_fpath, "w") as fopen:
-                        fopen.write(
-                            f"FINISHED AT {time.asctime( time.localtime(time.time()) )}."
-                        )
-                    reactor_status.append(True)
-                else:
-                    reactor_status.append(False)
+        # --- read dict from files
+        try:
+            if input_file.suffix == ".json":
+                with open(input_file, "r") as fopen:
+                    input_dict = json.load(fopen)
+            elif input_file.suffix == ".yaml":
+                with open(input_file, "r") as fopen:
+                    input_dict = yaml.safe_load(fopen)
             else:
-                with open(flag_fpath, "r") as fopen:
-                    content = fopen.readlines()
-                self._print(content)
-                reactor_status.append(True)
-        
-        if all(reactor_status):
-            self.status = "finished"
+                ...
+        except FileNotFoundError as e:
+            # NOTE: There is json or yaml in the string but it is not a file though.
+            input_dict = None
+
+    # NOTE: recursive read internal json or yaml files
+    if input_dict is not None:
+        for key, value in input_dict.items():
+            key_dict = parse_input_file(value, write_json=False)
+            if key_dict is not None:
+                input_dict[key] = key_dict
+
+    if input_dict and write_json:
+        with open(json_path / "params.json", "w") as fopen:
+            json.dump(input_dict, fopen, indent=4)
+        print("See params.json for values of all parameters...")
 
-        return reactors
+    return input_dict
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.6/src/gdpx/reactor/reactor.py` & `gdpx-0.0.7/src/gdpx/reactor/reactor.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/string/cp2k.py` & `gdpx-0.0.7/src/gdpx/reactor/string/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/string/grid.py` & `gdpx-0.0.7/src/gdpx/reactor/string/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/string/pathway.py` & `gdpx-0.0.7/src/gdpx/reactor/string/pathway.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/reactor/string/string.py` & `gdpx-0.0.7/src/gdpx/reactor/string/string.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
     #: Period to save the restart file.
     ckpt_period: int = 100
 
     #: Number of images along the pathway.
     nimages: int = 7
 
-    #: Align IS and FS based on the mic.
-    mic: bool = True
+    #: Methods that interpolates structures.
+    interpolation: dict = dataclasses.field(default_factory=dict)
 
     #: Optimiser.
     optimiser: str = "bfgs"
 
     #: Spring constant, eV/Ang2.
     k: float = 5.0
 
@@ -237,49 +237,60 @@
 
         Returns:
             A List of Atoms structures.
 
         """
         nstructures = len(structures)
         if nstructures == 2:
+            self._print("Interpolate a pathway.")
             # - check lattice consistency
             ini_atoms, fin_atoms = structures
             c1, c2 = ini_atoms.get_cell(complete=True), fin_atoms.get_cell(
                 complete=True
             )
             assert np.allclose(c1, c2), "Inconsistent unit cell..."
 
-            # - align structures
+            cons_text = run_params.pop("constraint", None)
+            self._preprocess_constraints(ini_atoms, cons_text)
+            self._preprocess_constraints(fin_atoms, cons_text)
+
+            # - 
+            use_mic = self.setting.interpolation.get("mic", True)
+            idpp_params = self.setting.interpolation.get("idpp", {})
+
+            # - linear interpolate
             shifts = fin_atoms.get_positions() - ini_atoms.get_positions()
-            if self.setting.mic:
+            if use_mic:
                 self._print("Align IS and FS based on MIC.")
                 curr_vectors, curr_distances = find_mic(shifts, c1, pbc=True)
-                self._debug(f"curr_vectors: {curr_vectors}")
+                # self._debug(f"curr_vectors: {curr_vectors}")
                 self._print(f"disp: {np.linalg.norm(curr_vectors)}")
                 fin_atoms.positions = ini_atoms.get_positions() + curr_vectors
             else:
                 self._print(f"disp: {np.linalg.norm(shifts)}")
 
-            cons_text = run_params.pop("constraint", None)
-            self._preprocess_constraints(ini_atoms, cons_text)
-            self._preprocess_constraints(fin_atoms, cons_text)
-
-            # - find mep
             nimages = self.setting.nimages
             images = [ini_atoms]
             images += [ini_atoms.copy() for i in range(nimages - 2)]
             images.append(fin_atoms)
 
             interpolate(
                 images=images,
                 mic=False,
                 interpolate_cell=False,
                 use_scaled_coord=False,
                 apply_constraint=False,
             )
+
+            if idpp_params:
+                # FIXME: make idpp a manager?
+                idpp_interpolate(
+                    images=images, traj=str(self.directory/"idpp_images.traj"),
+                    log=str(self.directory/"idpp.log"), mic=use_mic, **idpp_params
+                )
         else:
             self._print("Use a pre-defined pathway.")
             images = [a.copy() for a in structures]
 
         return images
 
     def read_trajectory(self, *args, **kwargs):
```

### Comparing `gdpx-0.0.6/src/gdpx/reactor/string/vasp.py` & `gdpx-0.0.7/src/gdpx/reactor/string/vasp.py`

 * *Files 19% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         verified = super()._verify_checkpoint()
         if verified:
             vasprun = self.directory / "01" / "OUTCAR"
             if vasprun.exists() and vasprun.stat().st_size != 0:
                 temp_frames = read(vasprun, ":")
                 try:
                     _ = temp_frames[0].get_forces()
+                    verified = True
                 except:
                     verified = False
             else:
                 verified = False
         else:
             verified = False
 
@@ -139,31 +140,54 @@
         """"""
         try:
             # --
             run_params = self.setting.get_run_params(**kwargs)
             run_params.update(**self.setting.get_init_params())
 
             if ckpt_wdir is None:  # start from the scratch
+                self._print("interpolate input images...")
                 images = self._align_structures(structures, run_params)
-                write(self.directory / "images.xyz", images)
             else:
+                self._print("update input images...")
                 # - update structures
                 rep_dirs = sorted(
-                    [x.name for x in sorted(self.directory.glob(r"[0-9][0-9]"))]
+                    ckpt_wdir.glob(r"[0-9][0-9]"), key=lambda x: int(x.name)
                 )
 
                 frames_ = []
                 for x in rep_dirs[1:-1]:
-                    frames_.append(read(self.directory / x / "OUTCAR", ":"))
-                nframes = min([len(x) for x in frames_])
+                    frames_.append(read(x / "OUTCAR", ":"))
+                nframes_per_image = [len(x) for x in frames_]
+                nframes = min(nframes_per_image)
                 assert nframes > 0, "At least one step finished before resume..."
                 intermediates_ = [x[nframes - 1] for x in frames_]
-                images = [structures[0]] + intermediates_ + [structures[-1]]
 
-                run_params.update(steps=self.setting.steps - nframes)
+                # -- sort frames from outcar
+                if (ckpt_wdir / ASE_VASP_SORT_FNAME).exists():
+                    sort, resort = read_sort(ckpt_wdir, ASE_VASP_SORT_FNAME)
+                else:
+                    natoms = len(structures[0])
+                    sort, resort = list(range(natoms)), list(range(natoms))
+
+                intermediates = []
+                for a in intermediates_:
+                    sorted_atoms = resort_atoms_with_spc(
+                        a, resort, "vasp", print_func=self._print, debug_func=self._debug
+                    )
+                    intermediates.append(sorted_atoms)
+
+                images = [structures[0]] + intermediates + [structures[-1]]
+
+                # the param keys have been proprocessed to vasp ones
+                run_params.update(nsw=self.setting.steps + 1 - nframes)
+
+                # constraint info has already been in OUTCAR
+                run_params.pop("constraint")
+
+            write(self.directory / "images.xyz", images)
 
             # - update input
             self.calc.set(**run_params)
 
             atoms = images[0]
             atoms.calc = self.calc
 
@@ -280,8 +304,7 @@
             frames.append(curr_frames)
 
         return frames
 
 
 if __name__ == "__main__":
     ...
-
```

### Comparing `gdpx-0.0.6/src/gdpx/reactor/utils.py` & `gdpx-0.0.7/src/gdpx/reactor/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/__init__.py` & `gdpx-0.0.7/src/gdpx/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/interface.py` & `gdpx-0.0.7/src/gdpx/scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/local.py` & `gdpx-0.0.7/src/gdpx/scheduler/local.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/lsf.py` & `gdpx-0.0.7/src/gdpx/scheduler/lsf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/pbs.py` & `gdpx-0.0.7/src/gdpx/scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/scheduler.py` & `gdpx-0.0.7/src/gdpx/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/scheduler/slurm.py` & `gdpx-0.0.7/src/gdpx/scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/__init__.py` & `gdpx-0.0.7/src/gdpx/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/basin.py` & `gdpx-0.0.7/src/gdpx/selector/basin.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/compare.py` & `gdpx-0.0.7/src/gdpx/selector/compare.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/composition.py` & `gdpx-0.0.7/src/gdpx/selector/composition.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/cur.py` & `gdpx-0.0.7/src/gdpx/selector/cur.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/descriptor.py` & `gdpx-0.0.7/src/gdpx/selector/descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,35 +191,38 @@
             ...
 
         if features.shape[0] > 1:
             reducer = PCA(n_components=2)
             reducer.fit(features)
             proj = reducer.transform(features)
 
+            fig, ax = plt.subplots(1, 1, figsize=(12, 8))
+
             for grp_name, inds in groups.items():
-                sc = plt.scatter(
+                sc = ax.scatter(
                     proj[others[grp_name], 0],
                     proj[others[grp_name], 1],
                     marker="o",
                     alpha=0.25,
                     label=f"grp-{grp_name} {len(others[grp_name])} -> {len(inds)}",
                 )
                 # --
                 selected_proj = reducer.transform(np.array([features[i] for i in inds]))
-                plt.scatter(
+                ax.scatter(
                     selected_proj[:, 0],
                     selected_proj[:, 1],
                     marker="*",
                     alpha=0.5,
                     color="r",
                 )
-            plt.legend(fontsize=12)
-            plt.axis("off")
-            plt.savefig(self.info_fpath.parent / (self.info_fpath.stem + ".png"))
+            ax.legend(fontsize=12)
+            ax.axis("off")
+            fig.savefig(self.info_fpath.parent / (self.info_fpath.stem + ".png"))
+            plt.close()
         else:
-            ... # Cannot plot PCA with only one structure...
+            ...  # Cannot plot PCA with only one structure...
 
         return
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.6/src/gdpx/selector/graph.py` & `gdpx-0.0.7/src/gdpx/selector/graph.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/interface.py` & `gdpx-0.0.7/src/gdpx/selector/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/interval.py` & `gdpx-0.0.7/src/gdpx/selector/interval.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/invariant.py` & `gdpx-0.0.7/src/gdpx/selector/invariant.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/locate.py` & `gdpx-0.0.7/src/gdpx/selector/locate.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/property.py` & `gdpx-0.0.7/src/gdpx/selector/property.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import abc
 import copy
 import dataclasses
 import itertools
-from typing import NoReturn, Union, List, Callable
+from typing import NoReturn, Optional, Union, List, Mapping, Callable
 
 import numpy as np
 
 from ase import Atoms
 from ase.io import read, write
 
 from ..data.array import AtomsNDArray
 from .selector import AbstractSelector
 from .cur import stat_str2val, boltz_selection, hist_selection
 
 
+def get_metric_func(metric_name: str):
+    """"""
+    if metric_name == "fabs":
+        metric_func = np.fabs
+    elif metric_name == "max":
+        metric_func = np.max
+    elif metric_name == "min":
+        metric_func = np.min
+    else:
+        raise NotImplementedError(f"Unknown metric function {metric_name}.")
+
+    return metric_func
+
+
 @dataclasses.dataclass
 class PropertyItem:
 
     #: Property name that can be found in atoms.info or atoms.arrays.
     name: str
 
     #: metric config...
     metric: Union[str, List[str]] = None
 
     #: List of functions, min, max, average and ...
     _metric: List[Callable] = dataclasses.field(init=False, default_factory=list)
 
-    # metric_params
+    #: Apply group selection.
+    group: Optional[str] = None
 
     #: Sparsifiction method. [filter, sort, hist, boltz]
     sparsify: str = "filter"
 
     #: Whether reverse the sparsifiction behaviour.
     reverse: bool = False
 
@@ -46,15 +61,15 @@
     #: Property maximum.
     pmax: float = dataclasses.field(init=False, default=np.inf)
 
     #: Number of bins for histogram-based sparsification.
     nbins: int = 20
 
     #: Boltzmann temperature (eV).
-    kBT: float = None
+    kBT: Optional[float] = None
 
     # expression
     # weight
 
     # worker_config: dataclasses.InitVar[str] = None
 
     def __post_init__(self):
@@ -171,40 +186,100 @@
                 for k, v in itertools.groupby(data.markers, key=lambda x: x[self.axis]):
                     if k in marker_groups:
                         marker_groups[k].extend(list(v))
                     else:
                         marker_groups[k] = list(v)
             self._debug(f"marker_groups: {marker_groups}")
 
-            selected_markers = []
-            for grp_name, curr_markers in marker_groups.items():
-                curr_frames = data.get_marked_structures(curr_markers)
-                curr_nframes = len(curr_frames)
-
-                # --
-                if curr_nframes > 0:
-                    scores, selected_indices = self._sparsify(prop_item, curr_frames)
-                    self._print(f"number of structures: {len(selected_indices)}")
-                    curr_selected_markers = [curr_markers[i] for i in selected_indices]
-                    selected_markers.extend(curr_selected_markers)
-
-                    # - add score to atoms
-                    for score, i in zip(scores, selected_indices):
-                        curr_frames[i].info["score"] = score
-
-                else:
-                    ...
+            if prop_item.group is None:
+                selected_markers = self._mark_group_separate(
+                    data, prop_item, marker_groups
+                )
+            else:
+                selected_markers = self._mark_group_represent(
+                    data, prop_item, marker_groups
+                )
 
             data.markers = np.array(selected_markers)
 
             if len(selected_markers) == 0:
                 break
 
         return
 
+    def _mark_group_represent(self, data, prop_item: PropertyItem, marker_groups):
+        """Mark a group of structures based on a representative structure's property."""
+
+        metric_func = get_metric_func(prop_item.group)
+
+        rep_counter = 0
+        rep_groups = []  # data for representative groups
+        for grp_name, curr_markers in marker_groups.items():
+            curr_frames = data.get_marked_structures(curr_markers)
+            curr_nframes = len(curr_frames)
+
+            if curr_nframes > 0:
+                curr_values = self._extract_property(curr_frames, prop_item)
+                metric_val = metric_func(curr_values)
+                # FIXME: how to find index if structures with same properties?
+                rep_frame = curr_frames[curr_values.index(metric_val)]
+                rep_groups.append((grp_name, rep_counter, rep_frame, metric_val))
+                rep_counter += 1
+            else:
+                ...
+        rep_groups = sorted(rep_groups, key=lambda x: x[3])
+
+        rep_frames = [x[2] for x in rep_groups]
+
+        selected_markers = []
+        scores, selected_indices = self._sparsify(prop_item, rep_frames)
+        self._print(f"number of groups: {len(selected_indices)}")
+
+        _counter = 0
+        for grp_name, rep_index, _, _ in rep_groups:
+            if rep_index in selected_indices:
+                curr_selected_markers = marker_groups[grp_name]
+                selected_markers.extend(curr_selected_markers)
+                curr_score = scores[selected_indices.index(rep_index)]
+                curr_selected_frames = data.get_marked_structures(curr_selected_markers)
+                for a in curr_selected_frames:
+                    a.info["score"] = curr_score
+                num_curr_frames = len(curr_selected_frames)
+                self._debug(f"group: {grp_name} -> {num_curr_frames}")
+                _counter += num_curr_frames
+            else:
+                ...
+
+        assert _counter == len(selected_markers)
+
+        return selected_markers
+
+    def _mark_group_separate(self, data, prop_item: PropertyItem, marker_groups):
+        """Mark a group of structures based on a structure's own property."""
+        selected_markers = []
+        for grp_name, curr_markers in marker_groups.items():
+            curr_frames = data.get_marked_structures(curr_markers)
+            curr_nframes = len(curr_frames)
+
+            # --
+            if curr_nframes > 0:
+                scores, selected_indices = self._sparsify(prop_item, curr_frames)
+                self._print(f"number of structures: {len(selected_indices)}")
+                curr_selected_markers = [curr_markers[i] for i in selected_indices]
+                selected_markers.extend(curr_selected_markers)
+
+                # - add score to atoms
+                for score, i in zip(scores, selected_indices):
+                    curr_frames[i].info["score"] = score
+
+            else:
+                ...
+
+        return selected_markers
+
     def _extract_property(self, frames: List[Atoms], prop_item: PropertyItem):
         """Extract property values from frames.
 
         Returns:
             property values: List[float] or 1d-np.array.
 
         """
```

### Comparing `gdpx-0.0.6/src/gdpx/selector/random.py` & `gdpx-0.0.7/src/gdpx/selector/random.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/scf.py` & `gdpx-0.0.7/src/gdpx/selector/scf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/selector/selector.py` & `gdpx-0.0.7/src/gdpx/selector/selector.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/trainer/__init__.py` & `gdpx-0.0.7/src/gdpx/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/trainer/interface.py` & `gdpx-0.0.7/src/gdpx/trainer/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/atomUtils.py` & `gdpx-0.0.7/src/gdpx/utils/atomUtils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/cleave_cluster.py` & `gdpx-0.0.7/src/gdpx/utils/cleave_cluster.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/cmdrun.py` & `gdpx-0.0.7/src/gdpx/utils/cmdrun.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/cmp_refdat.py` & `gdpx-0.0.7/src/gdpx/utils/cmp_refdat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/comparision.py` & `gdpx-0.0.7/src/gdpx/utils/comparision.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/dputils/DeepPot.py` & `gdpx-0.0.7/src/gdpx/utils/dputils/DeepPot.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/dputils/acquire_dmat.py` & `gdpx-0.0.7/src/gdpx/utils/dputils/acquire_dmat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/geometry.py` & `gdpx-0.0.7/src/gdpx/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/plot_dimer.py` & `gdpx-0.0.7/src/gdpx/utils/plot_dimer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/reduce_dataset.py` & `gdpx-0.0.7/src/gdpx/utils/reduce_dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/second_reduce.py` & `gdpx-0.0.7/src/gdpx/utils/second_reduce.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/split-dataset.py` & `gdpx-0.0.7/src/gdpx/utils/split-dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/utils/strucopy.py` & `gdpx-0.0.7/src/gdpx/utils/strucopy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/__init__.py` & `gdpx-0.0.7/src/gdpx/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/diffusion_coefficient.py` & `gdpx-0.0.7/src/gdpx/validator/diffusion_coefficient.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/dimer.py` & `gdpx-0.0.7/src/gdpx/validator/dimer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/eos.py` & `gdpx-0.0.7/src/gdpx/validator/eos.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/interface.py` & `gdpx-0.0.7/src/gdpx/validator/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/mdf.py` & `gdpx-0.0.7/src/gdpx/validator/mdf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/melting_point.py` & `gdpx-0.0.7/src/gdpx/validator/melting_point.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/minima.py` & `gdpx-0.0.7/src/gdpx/validator/minima.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/rank.py` & `gdpx-0.0.7/src/gdpx/validator/rank.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/rdf.py` & `gdpx-0.0.7/src/gdpx/validator/rdf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/rxn.py` & `gdpx-0.0.7/src/gdpx/validator/rxn.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/spc.py` & `gdpx-0.0.7/src/gdpx/validator/spc.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/surface_energy.py` & `gdpx-0.0.7/src/gdpx/validator/surface_energy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/validator/validator.py` & `gdpx-0.0.7/src/gdpx/validator/validator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/drive.py` & `gdpx-0.0.7/src/gdpx/worker/drive.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/explore.py` & `gdpx-0.0.7/src/gdpx/worker/explore.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/grid.py` & `gdpx-0.0.7/src/gdpx/worker/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/react.py` & `gdpx-0.0.7/src/gdpx/worker/react.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/single.py` & `gdpx-0.0.7/src/gdpx/worker/single.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/train.py` & `gdpx-0.0.7/src/gdpx/worker/train.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/utils.py` & `gdpx-0.0.7/src/gdpx/worker/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx/worker/worker.py` & `gdpx-0.0.7/src/gdpx/worker/worker.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.6/src/gdpx.egg-info/PKG-INFO` & `gdpx-0.0.7/src/gdpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automate computational chemistry/materials sciance and machine learning interatomic potential training workflow.
 Author-email: Jiayan Xu <ahcigar@foxmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdpx-0.0.6/src/gdpx.egg-info/SOURCES.txt` & `gdpx-0.0.7/src/gdpx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,31 @@
 src/gdpx.egg-info/PKG-INFO
 src/gdpx.egg-info/SOURCES.txt
 src/gdpx.egg-info/dependency_links.txt
 src/gdpx.egg-info/entry_points.txt
 src/gdpx.egg-info/requires.txt
 src/gdpx.egg-info/top_level.txt
 src/gdpx/bias/__init__.py
-src/gdpx/bias/afir.py
 src/gdpx/bias/bias.py
-src/gdpx/bias/gaussian.py
-src/gdpx/bias/harmonic.py
+src/gdpx/bias/bondboost.py
 src/gdpx/bias/nuclei.py
+src/gdpx/bias/timeio.py
+src/gdpx/bias/afir/__init__.py
+src/gdpx/bias/afir/afir.py
+src/gdpx/bias/gaussian/__init__.py
+src/gdpx/bias/gaussian/bond.py
+src/gdpx/bias/gaussian/com.py
+src/gdpx/bias/gaussian/gaussian.py
+src/gdpx/bias/gaussian/rmsd.py
+src/gdpx/bias/harmonic/__init__.py
+src/gdpx/bias/harmonic/distance.py
+src/gdpx/bias/harmonic/harmonic.py
+src/gdpx/bias/harmonic/plane.py
+src/gdpx/bias/utils/__init__.py
+src/gdpx/bias/utils/bondpair.py
 src/gdpx/builder/__init__.py
 src/gdpx/builder/builder.py
 src/gdpx/builder/cleave_group.py
 src/gdpx/builder/cleave_surface.py
 src/gdpx/builder/constraints.py
 src/gdpx/builder/crossover.py
 src/gdpx/builder/dimer.py
@@ -38,14 +50,15 @@
 src/gdpx/builder/zoom.py
 src/gdpx/builder/graph/__init__.py
 src/gdpx/builder/graph/exchange.py
 src/gdpx/builder/graph/insert.py
 src/gdpx/builder/graph/modifier.py
 src/gdpx/builder/graph/remove.py
 src/gdpx/builder/mutation/__init__.py
+src/gdpx/cli/compute.py
 src/gdpx/colvar/__init__.py
 src/gdpx/colvar/compute_reweight.py
 src/gdpx/colvar/coordination.py
 src/gdpx/colvar/distance.py
 src/gdpx/colvar/fingerprint.py
 src/gdpx/colvar/plot_meta.py
 src/gdpx/colvar/plot_string.py
@@ -68,14 +81,15 @@
 src/gdpx/computation/espresso.py
 src/gdpx/computation/interface.py
 src/gdpx/computation/lammps.py
 src/gdpx/computation/lasp.py
 src/gdpx/computation/reann.py
 src/gdpx/computation/utils.py
 src/gdpx/computation/vasp.py
+src/gdpx/computation/mc/tfmc.py
 src/gdpx/computation/md/md_utils.py
 src/gdpx/computation/md/nosehoover.py
 src/gdpx/core/__init__.py
 src/gdpx/core/node.py
 src/gdpx/core/operation.py
 src/gdpx/core/placeholder.py
 src/gdpx/core/register.py
@@ -105,14 +119,15 @@
 src/gdpx/describer/describer.py
 src/gdpx/describer/interface.py
 src/gdpx/describer/soap.py
 src/gdpx/describer/spc.py
 src/gdpx/expedition/__init__.py
 src/gdpx/expedition/expedition.py
 src/gdpx/expedition/interface.py
+src/gdpx/expedition/accelerated_dynamics/prev_example.py
 src/gdpx/expedition/af/afir.py
 src/gdpx/expedition/ga/engine.py
 src/gdpx/expedition/ga/population.py
 src/gdpx/expedition/monte_carlo/__init__.py
 src/gdpx/expedition/monte_carlo/basin_hopping.py
 src/gdpx/expedition/monte_carlo/monte_carlo.py
 src/gdpx/expedition/monte_carlo/operators/__init__.py
@@ -133,14 +148,15 @@
 src/gdpx/potential/__init__.py
 src/gdpx/potential/interface.py
 src/gdpx/potential/manager.py
 src/gdpx/potential/trainer.py
 src/gdpx/potential/calculators/dummy.py
 src/gdpx/potential/calculators/mixer.py
 src/gdpx/potential/managers/__init__.py
+src/gdpx/potential/managers/asepot.py
 src/gdpx/potential/managers/bias.py
 src/gdpx/potential/managers/cp2k.py
 src/gdpx/potential/managers/dftd3.py
 src/gdpx/potential/managers/eam.py
 src/gdpx/potential/managers/emt.py
 src/gdpx/potential/managers/espresso.py
 src/gdpx/potential/managers/grid.py
@@ -169,15 +185,14 @@
 src/gdpx/potential/managers/reann/reann.py
 src/gdpx/potential/managers/reann/calculators/reann.py
 src/gdpx/reactor/__init__.py
 src/gdpx/reactor/interface.py
 src/gdpx/reactor/reactor.py
 src/gdpx/reactor/utils.py
 src/gdpx/reactor/future/AccCons.py
-src/gdpx/reactor/future/AccHop.py
 src/gdpx/reactor/future/AccNEB.py
 src/gdpx/reactor/future/cmp_mep.py
 src/gdpx/reactor/future/constrain.py
 src/gdpx/reactor/future/crs.py
 src/gdpx/reactor/future/diffusion3.py
 src/gdpx/reactor/future/find_adsorption.py
 src/gdpx/reactor/future/find_inter.py
```

