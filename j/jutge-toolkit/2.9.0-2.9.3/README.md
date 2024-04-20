# Comparing `tmp/jutge-toolkit-2.9.0.tar.gz` & `tmp/jutge-toolkit-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jutge-toolkit-2.9.0.tar", last modified: Fri May 20 13:00:03 2022, max compression
+gzip compressed data, was "jutge-toolkit-2.9.3.tar", last modified: Thu Jan 26 09:23:50 2023, max compression
```

## Comparing `jutge-toolkit-2.9.0.tar` & `jutge-toolkit-2.9.3.tar`

### file list

```diff
@@ -1,37 +1,240 @@
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2022-05-20 13:00:03.532572 jutge-toolkit-2.9.0/
--rw-r--r--   0 jpetit     (501) staff       (20)    11368 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/LICENSE.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       28 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/MANIFEST.in
--rw-r--r--   0 jpetit     (501) staff       (20)      450 2022-05-20 13:00:03.532165 jutge-toolkit-2.9.0/PKG-INFO
--rwxr-xr-x   0 jpetit     (501) staff       (20)     1682 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/README.md
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2022-05-20 13:00:03.506216 jutge-toolkit-2.9.0/jutge/
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2022-05-20 13:00:03.512911 jutge-toolkit-2.9.0/jutge/toolkit/
--rwxr-xr-x   0 jpetit     (501) staff       (20)     3872 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/code_metrics.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)    16028 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/commented_code_detector.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)    35171 2022-05-20 08:54:14.000000 jutge-toolkit-2.9.0/jutge/toolkit/compilers.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)    21273 2022-05-18 13:55:34.000000 jutge-toolkit-2.9.0/jutge/toolkit/problems.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)    11393 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/quizzes.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)     2685 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/start.py
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2022-05-20 13:00:03.521529 jutge-toolkit-2.9.0/jutge/toolkit/sty/
--rw-r--r--   0 jpetit     (501) staff       (20)    42021 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/html.sty
--rwxr-xr-x   0 jpetit     (501) staff       (20)     5338 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/jutge.sty
--rw-r--r--   0 jpetit     (501) staff       (20)     1659 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.ca.sty
--rw-r--r--   0 jpetit     (501) staff       (20)     1907 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.de.sty
--rw-r--r--   0 jpetit     (501) staff       (20)     1618 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.en.sty
--rw-r--r--   0 jpetit     (501) staff       (20)     1710 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.es.sty
--rw-r--r--   0 jpetit     (501) staff       (20)     1697 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.fr.sty
--rw-r--r--   0 jpetit     (501) staff       (20)    17674 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/jutge/toolkit/sty/picins.sty
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2022-05-20 13:00:03.529265 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/
--rw-r--r--   0 jpetit     (501) staff       (20)      450 2022-05-20 13:00:02.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 jpetit     (501) staff       (20)      805 2022-05-20 13:00:03.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        1 2022-05-20 13:00:03.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jpetit     (501) staff       (20)      323 2022-05-20 13:00:03.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        1 2022-05-20 08:51:21.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 jpetit     (501) staff       (20)       50 2022-05-20 13:00:03.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/requires.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        6 2022-05-20 13:00:03.000000 jutge-toolkit-2.9.0/jutge_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2022-05-20 13:00:03.531589 jutge-toolkit-2.9.0/scripts/
--rwxr-xr-x   0 jpetit     (501) staff       (20)     1387 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/scripts/jutge-install-verilog
--rwxr-xr-x   0 jpetit     (501) staff       (20)     1000 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/scripts/jutge-install-vinga
--rwxr-xr-x   0 jpetit     (501) staff       (20)     1272 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/scripts/jutge-run
--rwxr-xr-x   0 jpetit     (501) staff       (20)      523 2020-09-18 14:41:58.000000 jutge-toolkit-2.9.0/scripts/jutge-submit
--rw-r--r--   0 jpetit     (501) staff       (20)       38 2022-05-20 13:00:03.532669 jutge-toolkit-2.9.0/setup.cfg
--rwxr-xr-x   0 jpetit     (501) staff       (20)     1470 2022-05-20 12:59:22.000000 jutge-toolkit-2.9.0/setup.py
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:50.060622 jutge-toolkit-2.9.3/
+-rw-r--r--   0 jpetit     (501) staff       (20)       68 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/.gitignore
+-rw-r--r--   0 jpetit     (501) staff       (20)    11368 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/LICENSE.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       28 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/MANIFEST.in
+-rw-r--r--   0 jpetit     (501) staff       (20)      126 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/Makefile
+-rw-r--r--   0 jpetit     (501) staff       (20)      431 2023-01-26 09:23:50.060134 jutge-toolkit-2.9.3/PKG-INFO
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     1682 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/README.md
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.701375 jutge-toolkit-2.9.3/documentation/
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      582 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/documentation/code_metrics.md
+-rw-r--r--   0 jpetit     (501) staff       (20)    22966 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/documentation/jutge-toolkit.png
+-rwxr-xr-x   0 jpetit     (501) staff       (20)    24106 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/documentation/problems.md
+-rw-r--r--   0 jpetit     (501) staff       (20)     6073 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/documentation/quick-start.md
+-rw-r--r--   0 jpetit     (501) staff       (20)     7763 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/documentation/quizzes.md
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.681098 jutge-toolkit-2.9.3/examples/
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.680692 jutge-toolkit-2.9.3/examples/problems/
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.703687 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.712107 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/
+-rw-r--r--   0 jpetit     (501) staff       (20)       35 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      371 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       71 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       22 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/sample-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       32 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/sample-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       99 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/ca/solution.cc
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.716800 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/
+-rw-r--r--   0 jpetit     (501) staff       (20)       35 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      364 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      105 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       23 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/sample-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       31 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/sample-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       94 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/en/solution.cc
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.721166 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/
+-rw-r--r--   0 jpetit     (501) staff       (20)       35 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      364 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/problem.es.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      104 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/problem.es.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       23 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/sample-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       34 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/sample-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       95 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/es/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       36 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/bon-dia.pbm/tags.yml
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.754884 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)       40 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/award.html
+-rw-r--r--   0 jpetit     (501) staff       (20)    23773 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/award.png
+-rw-r--r--   0 jpetit     (501) staff       (20)    66576 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/campanar.eps
+-rw-r--r--   0 jpetit     (501) staff       (20)    22070 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/campanar.png
+-rw-r--r--   0 jpetit     (501) staff       (20)      201 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/generate.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       50 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     2127 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       80 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     1989 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      119 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       55 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/sample.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      677 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/slow.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      832 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/tags.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       90 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/test-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)  1430160 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/test-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       12 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/test-2.ops
+-rw-r--r--   0 jpetit     (501) staff       (20)        0 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-1.pbm/test-b.inp
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.778898 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)    24001 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/award.png
+-rw-r--r--   0 jpetit     (501) staff       (20)    66576 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/campanar.eps
+-rw-r--r--   0 jpetit     (501) staff       (20)    22070 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/campanar.png
+-rw-r--r--   0 jpetit     (501) staff       (20)      301 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/generate.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      280 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/generate2.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       35 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     2066 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       92 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     2000 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      131 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       63 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/sample.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     1026 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/slow.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)     1036 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/tags.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)   102971 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/test-a.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)   112921 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/test-b.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     1129 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/test100.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)    12316 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-2.pbm/test1000.inp
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.799372 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)       40 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/award.html
+-rw-r--r--   0 jpetit     (501) staff       (20)    24047 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/award.png
+-rw-r--r--   0 jpetit     (501) staff       (20)   712485 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/campanar.eps
+-rw-r--r--   0 jpetit     (501) staff       (20)    22070 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/campanar.png
+-rw-r--r--   0 jpetit     (501) staff       (20)      368 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/escriu.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      201 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/generate.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       82 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/generate.py
+-rw-r--r--   0 jpetit     (501) staff       (20)       35 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)   199530 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/llarg.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     2583 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       91 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     2583 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      130 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       33 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/sample.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      677 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/slow.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      973 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/tags.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)        0 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/campanar-3.pbm/test-b.inp
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.813518 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)       18 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/gran.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       90 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)        9 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/ma-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       12 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/ma-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/ma-3.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/ma-4.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       17 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/ma-5.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       24 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/ma-6.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      378 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       68 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      359 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      105 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       15 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/sample.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      645 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       52 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/permutacions.pbm/tags.yml
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.839003 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)       55 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/gran.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/gran.ops
+-rw-r--r--   0 jpetit     (501) staff       (20)      134 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)        7 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       53 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-10.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       26 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-3.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       25 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-4.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       24 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-5.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-6.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       23 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-7.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-8.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       20 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/ma-9.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      379 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       71 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      350 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      104 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       15 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/sample.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      594 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       52 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/subconjunts-1.pbm/tags.yml
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.875561 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)     1862 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/atzar.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)    51278 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/award.png
+-rw-r--r--   0 jpetit     (501) staff       (20)      505 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/generate-1.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      505 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/generate-2.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      505 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/generate-3.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      505 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/generate-4.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       35 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       23 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       20 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       24 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-3.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       64 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-4.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       97 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-5.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       29 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-6.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       29 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-7.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       26 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-8.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     1235 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-9.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     2562 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-91.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      564 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/ma-92.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     1081 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       78 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     1149 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      115 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      716 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/random-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     1811 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/random-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     1056 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/random-3.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)     4188 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/random-4.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       57 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/sample-1.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       53 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/sample-2.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)       48 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/sample-3.inp
+-rw-r--r--   0 jpetit     (501) staff       (20)      889 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       13 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/tags.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tresors-1.pbm/un.inp
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.884652 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/
+-rw-r--r--   0 jpetit     (501) staff       (20)      324 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/generate-inputs.py
+-rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     1560 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/main.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)      725 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/problem.ca.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)       64 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/problem.ca.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      736 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/problem.en.tex
+-rw-r--r--   0 jpetit     (501) staff       (20)      101 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      668 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/solution.cc
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/tags.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)    32636 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/problems/tuples1.pbm/test.inp
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.681326 jutge-toolkit-2.9.3/examples/quizzes/
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.682193 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.912533 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/
+-rw-r--r--   0 jpetit     (501) staff       (20)     1194 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/FillIn1.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      450 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/FillIn2.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      256 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/Matchings.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       78 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/MultipleChoice.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      253 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/MultipleChoice.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      103 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/OpenEnded.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      117 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/OpenEnded.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      224 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/Ordering.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      132 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/SingleChoice.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      305 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/SingleChoice.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       14 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       62 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/problem.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      749 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/ca/quiz.yml
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:50.032357 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/
+-rw-r--r--   0 jpetit     (501) staff       (20)     1194 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/FillIn1.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      450 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/FillIn2.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      277 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/Matchings.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       78 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/MultipleChoice.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      253 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/MultipleChoice.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      103 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/OpenEnded.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      141 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/OpenEnded.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      224 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/Ordering.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      132 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/SingleChoice.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      305 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/SingleChoice.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)     2466 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/award.png
+-rw-r--r--   0 jpetit     (501) staff       (20)       13 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/handler.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)       62 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/problem.en.yml
+-rw-r--r--   0 jpetit     (501) staff       (20)      714 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/examples/quizzes/demo.pbm/en/quiz.yml
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:49.682996 jutge-toolkit-2.9.3/jutge/
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:50.038603 jutge-toolkit-2.9.3/jutge/toolkit/
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     3872 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/code_metrics.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)    16028 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/commented_code_detector.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)    36769 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/compilers.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)    21273 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/problems.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)    11393 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/quizzes.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     2685 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/start.py
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:50.044972 jutge-toolkit-2.9.3/jutge/toolkit/sty/
+-rw-r--r--   0 jpetit     (501) staff       (20)    42021 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/html.sty
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     5338 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/jutge.sty
+-rw-r--r--   0 jpetit     (501) staff       (20)     1659 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.ca.sty
+-rw-r--r--   0 jpetit     (501) staff       (20)     1907 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.de.sty
+-rw-r--r--   0 jpetit     (501) staff       (20)     1618 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.en.sty
+-rw-r--r--   0 jpetit     (501) staff       (20)     1710 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.es.sty
+-rw-r--r--   0 jpetit     (501) staff       (20)     1697 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.fr.sty
+-rw-r--r--   0 jpetit     (501) staff       (20)    17674 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/jutge/toolkit/sty/picins.sty
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:50.056418 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/
+-rw-r--r--   0 jpetit     (501) staff       (20)      431 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jpetit     (501) staff       (20)     8884 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)      323 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 jpetit     (501) staff       (20)       50 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/requires.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        6 2023-01-26 09:23:49.000000 jutge-toolkit-2.9.3/jutge_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-01-26 09:23:50.059516 jutge-toolkit-2.9.3/scripts/
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     1387 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/scripts/jutge-install-verilog
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     1000 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/scripts/jutge-install-vinga
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     1272 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/scripts/jutge-run
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      523 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/scripts/jutge-submit
+-rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-01-26 09:23:50.060756 jutge-toolkit-2.9.3/setup.cfg
+-rwxr-xr-x   0 jpetit     (501) staff       (20)     1470 2023-01-26 09:23:47.000000 jutge-toolkit-2.9.3/setup.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      425 2023-01-26 09:21:18.000000 jutge-toolkit-2.9.3/upload.sh
```

### Comparing `jutge-toolkit-2.9.0/LICENSE.txt` & `jutge-toolkit-2.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/README.md` & `jutge-toolkit-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/code_metrics.py` & `jutge-toolkit-2.9.3/jutge/toolkit/code_metrics.py`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/commented_code_detector.py` & `jutge-toolkit-2.9.3/jutge/toolkit/commented_code_detector.py`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/compilers.py` & `jutge-toolkit-2.9.3/jutge/toolkit/compilers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import os
 import shutil
 import signal
 import subprocess
 import sys
 import time
 import timeit
+
 import turtle_pil
+import yogi
 
 from colorama import Fore, Style
 from jutge import util
 
 # Maximum time to compile
 max_compilation_time = 30
 
@@ -901,14 +903,77 @@
         except CompilationTooLong:
             print(Style.BRIGHT + Fore.RED + 'Compilation time exceeded!' + Style.RESET_ALL)
             return False
         self.del_wrapper()
         return True
 
 
+class Compiler_Codon(Compiler):
+    compilers.append('Codon')
+
+    def name(self):
+        return 'Codon'
+
+    def type(self):
+        return 'compiler'
+
+    def executable(self):
+        return self.name + '.codon.exe'
+
+    def language(self):
+        return 'Python'
+
+    def version(self):
+        return self.get_version('codon --version', 0)
+
+    def flags1(self):
+        return '-release'
+
+    def flags2(self):
+        return '-release'
+
+    def extension(self):
+        return 'codon'
+
+    def execute(self, tst, correct, iterations=1):
+
+        ext = 'cor' if correct else 'codon.out'
+        cmd = f"./{self.executable()} < {tst}.inp > {tst}.{ext}"
+        print(cmd)
+
+        def func():
+            os.system(cmd)
+
+        time = timeit.timeit(func, number=iterations) / iterations
+
+        return time
+
+    def compile(self):
+        # TBD: compile no main
+        return self.compile_normal()
+
+    def compile_normal(self):
+        util.del_file(self.executable())
+
+        # hack to use yogi
+        if not os.path.exists('yogi.codon'):
+            shutil.copy(os.path.dirname(yogi.__file__) + '/yogi.codon', '.')
+
+        try:
+            self.execute_compiler('codon build -exe ' + self.flags1() + ' ' + self.name + '.codon')
+        except CompilationTooLong:
+            print(Style.BRIGHT + Fore.RED + 'Compilation time exceeded!' + Style.RESET_ALL)
+            util.del_file(self.executable())
+            return False
+        if not util.file_exists(self.name):
+            return False
+        util.move_file(self.name, self.executable())
+        return True
+
+
 class Compiler_R(Compiler):
     compilers.append('R')
 
     def name(self):
         return 'R'
 
     def type(self):
```

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/problems.py` & `jutge-toolkit-2.9.3/jutge/toolkit/problems.py`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/quizzes.py` & `jutge-toolkit-2.9.3/jutge/toolkit/quizzes.py`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/start.py` & `jutge-toolkit-2.9.3/jutge/toolkit/start.py`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/html.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/html.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/jutge.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/jutge.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.ca.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.ca.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.de.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.de.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.en.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.en.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.es.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.es.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/lang.fr.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/lang.fr.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/jutge/toolkit/sty/picins.sty` & `jutge-toolkit-2.9.3/jutge/toolkit/sty/picins.sty`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/scripts/jutge-install-verilog` & `jutge-toolkit-2.9.3/scripts/jutge-install-verilog`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/scripts/jutge-install-vinga` & `jutge-toolkit-2.9.3/scripts/jutge-install-vinga`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/scripts/jutge-run` & `jutge-toolkit-2.9.3/scripts/jutge-run`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/scripts/jutge-submit` & `jutge-toolkit-2.9.3/scripts/jutge-submit`

 * *Files identical despite different names*

### Comparing `jutge-toolkit-2.9.0/setup.py` & `jutge-toolkit-2.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # coding=utf-8
 
 from setuptools import setup
 from os import system
 
-version = '2.9.0'
+version = '2.9.3'
 
 setup(
     name='jutge-toolkit',
     packages=['jutge.toolkit'],
     install_requires=[
         'jutge-util',
         'pyyaml>=5.1',
```

