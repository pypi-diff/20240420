# Comparing `tmp/numerical_pde_solver-0.1.1.tar.gz` & `tmp/numerical-pde-solver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_pde_solver-0.1.1.tar", last modified: Sat Apr 20 03:37:13 2024, max compression
+gzip compressed data, was "numerical-pde-solver-0.1.3.tar", last modified: Sat Apr 20 03:43:47 2024, max compression
```

## Comparing `numerical_pde_solver-0.1.1.tar` & `numerical-pde-solver-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 03:37:13.458129 numerical_pde_solver-0.1.1/
--rw-rw-rw-   0        0        0      222 2024-04-20 03:37:13.458129 numerical_pde_solver-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-04-20 03:33:24.000000 numerical_pde_solver-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 03:37:13.448130 numerical_pde_solver-0.1.1/numerical_pde_solver/
--rw-rw-rw-   0        0        0        0 2024-04-20 02:54:19.000000 numerical_pde_solver-0.1.1/numerical_pde_solver/__init__.py
--rw-rw-rw-   0        0        0     1106 2024-04-20 02:53:48.000000 numerical_pde_solver-0.1.1/numerical_pde_solver/euler.py
--rw-rw-rw-   0        0        0     1225 2024-04-20 02:53:56.000000 numerical_pde_solver-0.1.1/numerical_pde_solver/milstein.py
-drwxrwxrwx   0        0        0        0 2024-04-20 03:37:13.455129 numerical_pde_solver-0.1.1/numerical_pde_solver.egg-info/
--rw-rw-rw-   0        0        0      222 2024-04-20 03:37:13.000000 numerical_pde_solver-0.1.1/numerical_pde_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-04-20 03:37:13.000000 numerical_pde_solver-0.1.1/numerical_pde_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 03:37:13.000000 numerical_pde_solver-0.1.1/numerical_pde_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-20 03:37:13.000000 numerical_pde_solver-0.1.1/numerical_pde_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-20 03:37:13.000000 numerical_pde_solver-0.1.1/numerical_pde_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 03:37:13.458129 numerical_pde_solver-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      414 2024-04-20 03:35:59.000000 numerical_pde_solver-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 03:37:13.457129 numerical_pde_solver-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-20 02:54:33.000000 numerical_pde_solver-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-20 03:22:43.000000 numerical_pde_solver-0.1.1/tests/test_euler.py
--rw-rw-rw-   0        0        0     1201 2024-04-20 03:25:44.000000 numerical_pde_solver-0.1.1/tests/test_milstein.py
+drwxrwxrwx   0        0        0        0 2024-04-20 03:43:47.636200 numerical-pde-solver-0.1.3/
+-rw-rw-rw-   0        0        0      960 2024-04-20 03:43:47.636200 numerical-pde-solver-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-20 03:33:24.000000 numerical-pde-solver-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 03:43:47.604669 numerical-pde-solver-0.1.3/numerical_pde_solver/
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:54:19.000000 numerical-pde-solver-0.1.3/numerical_pde_solver/__init__.py
+-rw-rw-rw-   0        0        0     1106 2024-04-20 02:53:48.000000 numerical-pde-solver-0.1.3/numerical_pde_solver/euler.py
+-rw-rw-rw-   0        0        0     1225 2024-04-20 02:53:56.000000 numerical-pde-solver-0.1.3/numerical_pde_solver/milstein.py
+drwxrwxrwx   0        0        0        0 2024-04-20 03:43:47.636200 numerical-pde-solver-0.1.3/numerical_pde_solver.egg-info/
+-rw-rw-rw-   0        0        0      960 2024-04-20 03:43:47.000000 numerical-pde-solver-0.1.3/numerical_pde_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-04-20 03:43:47.000000 numerical-pde-solver-0.1.3/numerical_pde_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 03:43:47.000000 numerical-pde-solver-0.1.3/numerical_pde_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 03:43:47.000000 numerical-pde-solver-0.1.3/numerical_pde_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-20 03:43:47.000000 numerical-pde-solver-0.1.3/numerical_pde_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 03:43:47.636200 numerical-pde-solver-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2024-04-20 03:43:42.000000 numerical-pde-solver-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 03:43:47.636200 numerical-pde-solver-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:54:33.000000 numerical-pde-solver-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-04-20 03:22:43.000000 numerical-pde-solver-0.1.3/tests/test_euler.py
+-rw-rw-rw-   0        0        0     1201 2024-04-20 03:25:44.000000 numerical-pde-solver-0.1.3/tests/test_milstein.py
```

### Comparing `numerical_pde_solver-0.1.1/numerical_pde_solver/euler.py` & `numerical-pde-solver-0.1.3/numerical_pde_solver/euler.py`

 * *Files identical despite different names*

### Comparing `numerical_pde_solver-0.1.1/numerical_pde_solver/milstein.py` & `numerical-pde-solver-0.1.3/numerical_pde_solver/milstein.py`

 * *Files identical despite different names*

### Comparing `numerical_pde_solver-0.1.1/tests/test_euler.py` & `numerical-pde-solver-0.1.3/tests/test_euler.py`

 * *Files identical despite different names*

### Comparing `numerical_pde_solver-0.1.1/tests/test_milstein.py` & `numerical-pde-solver-0.1.3/tests/test_milstein.py`

 * *Files identical despite different names*

