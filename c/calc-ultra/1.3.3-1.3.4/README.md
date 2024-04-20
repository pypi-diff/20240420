# Comparing `tmp/calc_ultra-1.3.3.tar.gz` & `tmp/calc_ultra-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calc_ultra-1.3.3.tar", last modified: Wed Mar 27 08:08:38 2024, max compression
+gzip compressed data, was "calc_ultra-1.3.4.tar", last modified: Sat Apr 20 14:13:33 2024, max compression
```

## Comparing `calc_ultra-1.3.3.tar` & `calc_ultra-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-03-27 08:08:38.803169 calc_ultra-1.3.3/
--rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.3/LICENSE
--rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.3/MANIFEST.in
--rw-r--r--   0 Huatao     (502) staff       (20)     4442 2024-03-27 08:08:38.802813 calc_ultra-1.3.3/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)     3711 2024-03-27 07:57:34.000000 calc_ultra-1.3.3/README.md
--rw-r--r--   0 Huatao     (502) staff       (20)      862 2024-03-26 08:21:28.000000 calc_ultra-1.3.3/pyproject.toml
--rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-03-27 08:08:38.803233 calc_ultra-1.3.3/setup.cfg
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-03-27 08:08:38.798061 calc_ultra-1.3.3/src/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-03-27 08:06:42.000000 calc_ultra-1.3.3/src/.DS_Store
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-03-27 08:08:38.799292 calc_ultra-1.3.3/src/calc_ultra/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-03-27 08:06:34.000000 calc_ultra-1.3.3/src/calc_ultra/.DS_Store
--rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.3/src/calc_ultra/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)    35036 2024-03-27 08:06:22.000000 calc_ultra-1.3.3/src/calc_ultra/main.py
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-03-27 08:08:38.801952 calc_ultra-1.3.3/src/calc_ultra/texts/
--rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.3/src/calc_ultra/texts/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.3/src/calc_ultra/texts/algcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.3/src/calc_ultra/texts/derivacalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      825 2024-03-19 08:26:51.000000 calc_ultra-1.3.3/src/calc_ultra/texts/intecalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.3/src/calc_ultra/texts/limcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)     1360 2024-03-27 08:03:30.000000 calc_ultra-1.3.3/src/calc_ultra/texts/main_screen.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-03-07 13:47:38.000000 calc_ultra-1.3.3/src/calc_ultra/texts/settings.txt
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-03-27 08:08:38.802304 calc_ultra-1.3.3/src/calc_ultra.egg-info/
--rw-r--r--   0 Huatao     (502) staff       (20)     4442 2024-03-27 08:08:38.000000 calc_ultra-1.3.3/src/calc_ultra.egg-info/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-03-27 08:08:38.000000 calc_ultra-1.3.3/src/calc_ultra.egg-info/SOURCES.txt
--rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-03-27 08:08:38.000000 calc_ultra-1.3.3/src/calc_ultra.egg-info/dependency_links.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       71 2024-03-27 08:08:38.000000 calc_ultra-1.3.3/src/calc_ultra.egg-info/requires.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-03-27 08:08:38.000000 calc_ultra-1.3.3/src/calc_ultra.egg-info/top_level.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.601904 calc_ultra-1.3.4/
+-rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.4/LICENSE
+-rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.4/MANIFEST.in
+-rw-r--r--   0 Huatao     (502) staff       (20)     4443 2024-04-20 14:13:33.601584 calc_ultra-1.3.4/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)     3712 2024-04-20 14:13:03.000000 calc_ultra-1.3.4/README.md
+-rw-r--r--   0 Huatao     (502) staff       (20)      862 2024-04-20 14:11:37.000000 calc_ultra-1.3.4/pyproject.toml
+-rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-04-20 14:13:33.601971 calc_ultra-1.3.4/setup.cfg
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.596156 calc_ultra-1.3.4/src/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-04-20 14:11:29.000000 calc_ultra-1.3.4/src/.DS_Store
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.597346 calc_ultra-1.3.4/src/calc_ultra/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-04-13 13:31:29.000000 calc_ultra-1.3.4/src/calc_ultra/.DS_Store
+-rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.4/src/calc_ultra/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)    36559 2024-04-20 14:13:02.000000 calc_ultra-1.3.4/src/calc_ultra/main.py
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.600786 calc_ultra-1.3.4/src/calc_ultra/texts/
+-rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.4/src/calc_ultra/texts/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.4/src/calc_ultra/texts/algcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.4/src/calc_ultra/texts/derivacalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      761 2024-04-14 10:36:05.000000 calc_ultra-1.3.4/src/calc_ultra/texts/intecalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.4/src/calc_ultra/texts/limcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)     1212 2024-04-14 10:36:57.000000 calc_ultra-1.3.4/src/calc_ultra/texts/main_screen.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-04-14 10:37:09.000000 calc_ultra-1.3.4/src/calc_ultra/texts/settings.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.601173 calc_ultra-1.3.4/src/calc_ultra.egg-info/
+-rw-r--r--   0 Huatao     (502) staff       (20)     4443 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/SOURCES.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/dependency_links.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       71 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/requires.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/top_level.txt
```

### Comparing `calc_ultra-1.3.3/LICENSE` & `calc_ultra-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.3/PKG-INFO` & `calc_ultra-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.3
+Version: 1.3.4
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
@@ -17,23 +17,23 @@
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: rich>=13.7.1
 Requires-Dist: scipy>=1.12.0
 
 # calc-ultra
 
-[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.3-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
+[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.4-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic)
 
-The Calc-ULTRA calculus calculator, but as a module!
+The Calc-Ultra calculus calculator, but as a module!
 
-- Little Python background knowledge needed!
+- Little Python background knowledge is needed!
 
 Supports:
 
 - Derivatives
 - Partials
 - Implicit differentiation
 - Antiderivatives
@@ -42,38 +42,38 @@
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
 ## Note
 
-This is the module package of the Calc-ULTRA calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
+This is the module package of the Calc-Ultra calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
 Command line: `pip3 install calc-ultra`.
-Due to Python import identifiers restrictions, please import Calc-ULTRA as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
+Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
 
 To run the calculator, import Calc-ULTRA as `calc_ultra` like so:
 
 `from calc_ultra import main`
 
 Make sure you have the latest version installed. To update calc-ultra, run `pip3 install --upgrade calc-ultra`.
 
 ## Requirements
 
-This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built in to most Python IDEs.
+This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built into most Python IDEs.
 
 ## Warnings
 
 ### Function limitations
 
-Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions are also limited due to SymPy limitations. While some composed functions work, others don't. 😟
+Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions is also limited due to SymPy limitations. While some composed functions work, others don't. 😟
 
 ## Test PYPI
 
 Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>.
 
 ## Acknowledgements
 
@@ -83,30 +83,30 @@
 And... a SPECIAL THANK-YOU to @Haobot for troubleshooting and feedback! 👍❤️
 
 This program was made using SymPy and Scipy for calculation and Matplotlib and NumPy for graphing.
 
 ## Gallery
 
 DerivaCalc derivative with graph demo:
-![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/22f7f674-81b4-4e5f-9bff-586d94c1976f "derivacalc_demo")
+![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
-![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/1035a5af-cf04-46c1-b2e3-ec5eff08c58d "intecalc_demo_1")
+![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
 
 InteCalc definite integral with graph demo:
-![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/42a127af-17f6-4608-a6aa-9029cf00e973 "intecalc_demo_2")
+![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b8294186-92f5-4df3-a000-d63f6fff93b0 "intecalc_demo_2")
 
 LimCalc limit demo:
-![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/bb08db05-9b1b-4204-9d98-d4a3baa2167d "limcalc_demo")
+![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/12db6a7b-a836-43ce-8cef-7bcf707051f7 "limcalc_demo")
 
 AlgCalc equation solver demo:
-![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7d2bdad0-572c-4eec-8644-2837a0689154 "algcalc_demo_1")
+![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/e4cfa016-52bf-43b5-a839-af9f42546468 "algcalc_demo_1")
 
 AlgCalc vector operation demo:
-![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/28c5143b-93fc-4165-b8d9-572d1ab00da8 "algcalc_demo_2")
+![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7f043cb2-6b0a-4460-ab35-30f09632b1c3 "algcalc_demo_2")
 
 AlgCalc matrix operation demo:
-![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b6d11f38-b5b8-42ed-b4b3-664c65207664 "algcalc_demo_3")
+![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/a9a5d56e-424a-4ef8-beb9-a9b64ce1a3f5 "algcalc_demo_3")
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `calc_ultra-1.3.3/README.md` & `calc_ultra-1.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # calc-ultra
 
-[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.3-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
+[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.4-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic)
 
-The Calc-ULTRA calculus calculator, but as a module!
+The Calc-Ultra calculus calculator, but as a module!
 
-- Little Python background knowledge needed!
+- Little Python background knowledge is needed!
 
 Supports:
 
 - Derivatives
 - Partials
 - Implicit differentiation
 - Antiderivatives
@@ -21,38 +21,38 @@
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
 ## Note
 
-This is the module package of the Calc-ULTRA calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
+This is the module package of the Calc-Ultra calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
 Command line: `pip3 install calc-ultra`.
-Due to Python import identifiers restrictions, please import Calc-ULTRA as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
+Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
 
 To run the calculator, import Calc-ULTRA as `calc_ultra` like so:
 
 `from calc_ultra import main`
 
 Make sure you have the latest version installed. To update calc-ultra, run `pip3 install --upgrade calc-ultra`.
 
 ## Requirements
 
-This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built in to most Python IDEs.
+This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built into most Python IDEs.
 
 ## Warnings
 
 ### Function limitations
 
-Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions are also limited due to SymPy limitations. While some composed functions work, others don't. 😟
+Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions is also limited due to SymPy limitations. While some composed functions work, others don't. 😟
 
 ## Test PYPI
 
 Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>.
 
 ## Acknowledgements
 
@@ -62,30 +62,30 @@
 And... a SPECIAL THANK-YOU to @Haobot for troubleshooting and feedback! 👍❤️
 
 This program was made using SymPy and Scipy for calculation and Matplotlib and NumPy for graphing.
 
 ## Gallery
 
 DerivaCalc derivative with graph demo:
-![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/22f7f674-81b4-4e5f-9bff-586d94c1976f "derivacalc_demo")
+![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
-![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/1035a5af-cf04-46c1-b2e3-ec5eff08c58d "intecalc_demo_1")
+![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
 
 InteCalc definite integral with graph demo:
-![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/42a127af-17f6-4608-a6aa-9029cf00e973 "intecalc_demo_2")
+![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b8294186-92f5-4df3-a000-d63f6fff93b0 "intecalc_demo_2")
 
 LimCalc limit demo:
-![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/bb08db05-9b1b-4204-9d98-d4a3baa2167d "limcalc_demo")
+![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/12db6a7b-a836-43ce-8cef-7bcf707051f7 "limcalc_demo")
 
 AlgCalc equation solver demo:
-![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7d2bdad0-572c-4eec-8644-2837a0689154 "algcalc_demo_1")
+![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/e4cfa016-52bf-43b5-a839-af9f42546468 "algcalc_demo_1")
 
 AlgCalc vector operation demo:
-![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/28c5143b-93fc-4165-b8d9-572d1ab00da8 "algcalc_demo_2")
+![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7f043cb2-6b0a-4460-ab35-30f09632b1c3 "algcalc_demo_2")
 
 AlgCalc matrix operation demo:
-![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b6d11f38-b5b8-42ed-b4b3-664c65207664 "algcalc_demo_3")
+![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/a9a5d56e-424a-4ef8-beb9-a9b64ce1a3f5 "algcalc_demo_3")
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `calc_ultra-1.3.3/pyproject.toml` & `calc_ultra-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [wheel]
 supported_platforms = ["macos"]
 
 [project]
 name = "calc_ultra"
-version = "1.3.3"
+version = "1.3.4"
 dependencies = [
   "sympy >= 1.12",
   "numpy >= 1.26.2",
   "matplotlib >= 3.8.3",
   "rich >= 13.7.1",
   "scipy >= 1.12.0"
 ]
```

### Comparing `calc_ultra-1.3.3/src/.DS_Store` & `calc_ultra-1.3.4/src/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 00000230: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00000240: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00000250: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00000260: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00000270: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 00000280: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 00000290: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-000002a0: 1018 7b7b 3438 312c 2032 3634 7d2c 207b  ..{{481, 264}, {
-000002b0: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
+000002a0: 1018 7b7b 3431 362c 2033 3339 7d2c 207b  ..{{416, 339}, {
+000002b0: 3835 352c 2034 3339 7d7d 0908 1523 2f3b  855, 439}}...#/;
 000002c0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 000002d0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 000002e0: 0000 0000 0000 008b 0000 000a 0063 0061  .............c.a
 000002f0: 006c 0063 005f 0075 006c 0074 0072 0061  .l.c._.u.l.t.r.a
 00000300: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.3/src/calc_ultra/.DS_Store` & `calc_ultra-1.3.4/src/calc_ultra/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 00000120: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00000130: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00000140: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000150: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000160: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000170: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000180: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000190: 7208 0908 095f 1018 7b7b 3438 312c 2032  r...._..{{481, 2
-000001a0: 3634 7d2c 207b 3932 302c 2034 3336 7d7d  64}, {920, 436}}
+00000190: 7208 0908 095f 1018 7b7b 3438 302c 2032  r...._..{{480, 2
+000001a0: 3636 7d2c 207b 3932 302c 2034 3336 7d7d  66}, {920, 436}}
 000001b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 000001c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000001e0: 0005 0074 0065 0078 0074 0073 7653 726e  ...t.e.x.t.svSrn
 000001f0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.3/src/calc_ultra/main.py` & `calc_ultra-1.3.4/src/calc_ultra/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 from sympy.core.numbers import pi, E, oo
 from math import floor, ceil
+import math as mt
 from scipy.special import gamma, polygamma, erf
 from rich import print
+from rich.progress import (
+    Progress,
+    SpinnerColumn,
+    BarColumn,
+    MofNCompleteColumn,
+    TimeElapsedColumn,
+    TextColumn,
+)
 from numpy import (
     linspace,
     exp,
     log,
     sqrt,
     abs,
     sin,
@@ -37,15 +46,15 @@
     solve,
     linsolve,
     pprint,
     simplify,
     symbols,
 )
 import matplotlib.pyplot as plt
-import datetime, logging, os, time, warnings
+import datetime, logging, random, os, time, warnings
 
 
 # Disable auto Python warnings
 
 warnings.filterwarnings("ignore")
 
 
@@ -56,57 +65,70 @@
 
     while True:
         expr = input()
 
         try:
             if expr != "q":
                 # Easy to exit unlike VIM ;)
+                result = eval(trig_rep(expr))
                 print("\n[bright_yellow]Result: [/bright_yellow]", end="")
-                if "pi" in expr:
-                    expr = expr.replace("pi", str(np.pi))
-
-                result = eval(replace_bound(expr))
                 pprint(result)
                 print()
 
             else:
                 break
 
         except:
+            print()
             logging.error(f'Could not parse: "{expr}"\n')
 
 
-def derive(function, order):
-    function = replace_expr(function)
+def derive(function: str, order: str):
+    calc = replace_expr(function)
 
     if check_order(order) is True:
         global df
-        df = diff(function, x, order)
+        df = diff(calc, x, order)
 
-        nprint(
-            f"\nDerivative of [bright_magenta]{function}[/bright_magenta] with order {order} is:\n"
+        print(
+            f"\nDerivative of [bright_magenta]{trig_rep(function)}[/bright_magenta] with order {order} is:\n"
         )
         print_expr(df)
 
-        if check_simp(df) is True:
-            nprint("\nSimplify/rewrite:\n")
-            print_expr(simplify(df, evaluate=False))
+        check_simp(df)
 
         df = trig_rep(str(df))
 
         print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
         show = input("(Exit the graph window when you are finished to continue) ")
 
         if show == "y":
             try:
-                print(
-                    "\n[bright_yellow]Loading graph. Might take some time on first startup ...[/bright_yellow]"
-                )
+                print()
+                with Progress(
+                    SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
+                    TextColumn("[bright_yellow]Loading graph...[/bright_yellow]"),
+                    BarColumn(),
+                    TimeElapsedColumn(),
+                    transient=False,
+                ) as progress:
+                    task = progress.add_task("", total=100)
+
+                    while not progress.finished:
+                        progress.update(task, advance=2)
+                        time.sleep(random.randint(2, 5) / 1000)
+
                 x_array = linspace(-50, 50, 200000)
 
+                def f(x):
+                    return eval(trig_rep(calc))
+
+                def dif(x):
+                    return eval(df)
+
                 title = "Function (red) and derivative (blue)"
                 plt.title(title)
                 plt.xlabel("x", weight="bold")
                 plt.ylabel("y", rotation=0, weight="bold")
                 plt.plot(x_array, f(x_array), color="red", label="Function")
                 plt.plot(x_array, dif(x_array), color="blue", label="Derivative")
                 plt.axis([-7.5, 7.5, -7.5, 7.5])
@@ -114,82 +136,97 @@
                 plt.grid()
                 plt.show()
 
                 print("\nExited graph.\n")
 
             except:
                 plt.close()
+                print("\n")
                 logging.warning("Could not graph function.")
                 print("\nExited graph.")
 
 
-def partial_derive(function, var, order):
-    function = replace_expr(function)
+def partial_derive(function: str, var: str, order: str):
+    calc = replace_expr(function)
 
     if check_order(order) is True:
-        df = diff(function, var, order)
+        df = diff(calc, var, order)
 
         print(
-            f"\nPartial derivative of [bright_magenta]{function}[/bright_magenta] in respect to {var} of order {order} is:\n"
+            f"\nPartial derivative of [bright_magenta]{trig_rep(function)}[/bright_magenta] in respect to {var} of order {order} is:\n"
         )
         print_expr(df)
 
-        if check_simp(df) is True:
-            print("\nSimplify/rewrite:\n")
-            print_expr(simplify(df, evaluate=False))
+        check_simp(df)
 
 
-def implicit_derive(circ, order):
-    circ = replace_expr(circ)
+def implicit_derive(circ: str, order: str):
+    calc = replace_expr(circ)
+    left = eval(calc[: calc.find("=")])
+    right = eval(calc[calc.find("=") + 1 :])
 
     if check_order(order) is True:
-        df = idiff(eval(circ), y, x, int(order))
+        df = idiff(left - right, y, x, order)
 
         print(
             f"\nDerivative of [bright_magenta]{circ}[/bright_magenta] with order {order} is:\n"
         )
         print_expr(df)
 
         if str(simplify(df, evaluate=False)) != str(df):
             print("\nSimplify/rewrite:\n")
             print_expr(simplify(df, evaluate=False))
 
 
-def antiderive(function):
-    function = replace_expr(function)
-
-    global F
-    F = Integral(function, x).doit()
+def antiderive(function: str):
+    calc = replace_expr(function)
+    F = Integral(calc, x).doit()
 
     if "Integral" in str(F):
         logging.warning("Cannot compute integral.\n")
         return ""
 
-    print(f"\nAntiderivative of [bright_magenta]{function}[/bright_magenta] is:\n")
+    print(
+        f"\nAntiderivative of [bright_magenta]{trig_rep(function)}[/bright_magenta] is:\n"
+    )
     print_expr(F)
 
-    if check_simp(F) is True:
-        print("\nSimplify/rewrite:\n")
-        print_expr(simplify(F, evaluate=False))
+    check_simp(F)
 
     F = trig_rep(str(F))
 
     print("\n[bold]Don't forget to add a constant![/bold]\n")
 
     print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
     show = input("(Exit the graph window when you are finished to continue) ")
 
     if show == "y":
         try:
-            print(
-                "\n[bright_yellow]Loading graph. Might take some time on first startup ...[/bright_yellow]"
-            )
+            print()
+            with Progress(
+                SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
+                TextColumn("[bright_yellow]Loading graph...[/bright_yellow]"),
+                BarColumn(),
+                TimeElapsedColumn(),
+                transient=False,
+            ) as progress:
+                task = progress.add_task("", total=100)
+
+                while not progress.finished:
+                    progress.update(task, advance=2)
+                    time.sleep(random.randint(2, 5) / 1000)
 
             x_array = linspace(-100, 100, 200000)
 
+            def f(x):
+                return eval(trig_rep(calc))
+
+            def af(x):
+                return eval(F)
+
             title = "Function (red) and antiderivative (blue, C = 0)"
             plt.title(title)
             plt.xlabel("x", weight="bold")
             plt.ylabel("y", rotation=0, weight="bold")
             plt.plot(x_array, f(x_array), color="red", label="Function")
             plt.plot(x_array, af(x_array), color="blue", label="Antiderivative")
             plt.axis([-7.5, 7.5, -7.5, 7.5])
@@ -198,52 +235,51 @@
             plt.grid()
             plt.show()
 
             print("\nExited graph.\n")
 
         except:
             plt.close()
+            print("\n")
             logging.warning("Could not graph function.")
             print("\nExited graph.\n")
 
 
-def def_int(function, low, up):
+def def_int(function: str, low: str, up: str):
     x = symbols("x")
-    function = replace_expr(function)
+    calc = replace_expr(function)
 
-    if check_bound(low) is False:
-        return ""
+    check_bound(low)
 
-    low = eval(low)
+    clow = eval(replace_expr(low))
 
-    if check_bound(up) is False:
-        return ""
+    check_bound(up)
 
-    up = eval(up)
+    cup = eval(replace_expr(up))
 
-    result = integrate(function, (x, low, up))
+    result = integrate(calc, (x, clow, cup))
 
-    up = eval(replace_bound(str(up)))
-    low = eval(replace_bound(str(low)))
+    gup = eval(replace_bound(str(cup)))
+    glow = eval(replace_bound(str(clow)))
 
-    num_result = integrate(function, (x, low, up)).evalf()
+    num_result = integrate(calc, (x, glow, gup)).evalf()
     # Composite functions usually do not have primitive antiderivatives
     # so calc-ultra is equipped with both symbolic and numerical answers.
 
     if (
         (str(result) == "nan")
         or ("I" in str(result))
         and ("Integral" not in str(result))
     ):
         logging.warning("Cannot compute integral because integral does not converge.")
         return ""
 
     if "Integral" not in str(result):
         print(
-            f"\nCalculated integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
+            f"\nCalculated integral of [bright_magenta]{trig_rep(function)}[/bright_magenta] from {low} to {up}. Final area is:\n"
         )
         print_expr(result)
 
     else:
         print("\nCannot express result symbolically.")
 
     nprint("\nNumeral evaluation/approximation:\n")
@@ -251,17 +287,27 @@
 
     print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
 
     show = input("(Exit the graph window when you are finished to continue) ")
 
     if show == "y":
         try:
-            print(
-                "\n[bright_yellow]Loading graph. Might take some time on first startup ...[/bright_yellow]"
-            )
+            print()
+            with Progress(
+                SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
+                TextColumn("[bright_yellow]Loading graph...[/bright_yellow]"),
+                BarColumn(),
+                TimeElapsedColumn(),
+                transient=False,
+            ) as progress:
+                task = progress.add_task("", total=100)
+
+                while not progress.finished:
+                    progress.update(task, advance=2)
+                    time.sleep(random.randint(2, 5) / 1000)
 
             x_array = linspace(-100, 100, 200000)
 
             if "log" in function:
                 x_array = linspace(
                     0.00000001,
                     100,
@@ -274,127 +320,129 @@
                     100,
                     200000,
                 )
 
             # This is just the gamma function shifted one unit left
             # Of course, the factorial is only defined for x >= 0
 
+            def f(x):
+                return eval(trig_rep(calc))
+
             title = "Shaded area beneath function"
             plt.title(title)
             plt.xlabel("x", weight="bold")
             plt.ylabel("y", rotation=0, weight="bold")
             plt.plot(x_array, f(x_array), color="red", label="Function")
 
             plt.fill_between(
                 x_array,
                 f(x_array),
-                where=[(x_array > low) and (x_array < up) for x_array in x_array],
+                where=[(x_array > clow) and (x_array < cup) for x_array in x_array],
                 color="blue",
             )
 
             try:
                 if graph_option == "f":
                     plt.axis([-7.5, 7.5, -7.5, 7.5])
 
                 elif graph_option == "a":
                     # Adjusted graph view is sometimes better for
                     # large graphs with large bounds.
-                    if (float(f(low)) != 0) and (float(f(up)) != 0):
+                    if (float(f(glow)) != 0) and (float(f(gup)) != 0):
                         plt.axis(
                             [
-                                low - 5,
-                                up + 5,
-                                float(f(round(low)))
-                                - (float(f(round(low))) + float(f(round(up)))) / 2
+                                glow - 5,
+                                gup + 5,
+                                float(f(round(glow)))
+                                - (float(f(round(glow))) + float(f(round(gup)))) / 2
                                 - 1,
-                                float(f(round(up)))
-                                + (float(f(round(low))) + float(f(round(up)))) / 2
+                                float(f(round(gup)))
+                                + (float(f(round(glow))) + float(f(round(gup)))) / 2
                                 + 1,
                             ]
                         )
 
-                    elif (float(f(low)) == 0) or (float(f(up)) == 0):
-                        plt.axis([low - 5, up + 5, -(up - low) / 2, (up + low) / 2])
+                    elif (float(f(glow)) == 0) or (float(f(gup)) == 0):
+                        plt.axis(
+                            [glow - 5, gup + 5, -(gup - glow) / 2, (gup + glow) / 2]
+                        )
 
             except:
                 plt.axis([-7.5, 7.5, -7.5, 7.5])
 
             plt.legend(loc="lower left")
             plt.grid()
             plt.show()
 
             return "\nExited graph.\n"
 
         except:
             plt.close()
+            print("\n")
             logging.warning("Could not graph function.")
             return "\nExited graph.\n"
 
     else:
         return "\n[bright_yellow]Exiting Definite Integral Screen ... ... ...[/bright_yellow]\n"
 
 
-def improp_int(function, low, up):
+def improp_int(function: str, low: str, up: str):
     function = replace_expr(function)
 
-    if check_bound(low) is False:
-        return ""
+    check_bound(low)
 
-    low = eval(low)
+    clow = eval(replace_expr(low))
 
-    if check_bound(up) is False:
-        return ""
+    check_bound(up)
 
-    up = eval(up)
+    cup = eval(replace_expr(up))
 
     try:
         improper_area = Integral(
-            function, (x, low, up)
+            function, (x, clow, cup)
         ).principal_value()  # Cauchy Principal Value
 
         if "Integral" not in str(improper_area):
             print(
                 f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
             )
             print_expr(improper_area)
 
         else:
             print("Cannot compute improper integral.")
 
     except ValueError:
-        improper_area = integrate(function, (x, low, up))
+        improper_area = integrate(function, (x, clow, cup))
 
         if "Integral" not in str(improper_area):
             print(
                 f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
             )
             print_expr(improper_area)
 
         else:
             print("Cannot compute improper integral.")
 
     print()
 
 
-def double_int(function, out_low, out_up, in_low, in_up):
+def double_int(function: str, out_low: str, out_up: str, in_low: str, in_up: str):
     function = replace_expr(function)
 
-    if check_bound(out_low) is False:
-        return ""
+    check_bound(out_low)
 
-    out_low = eval(out_low)
+    out_low = eval(replace_expr(out_low))
 
-    if check_bound(out_up) is False:
-        return ""
+    check_bound(out_up)
 
-    out_up = eval(out_up)
+    out_up = eval(replace_expr(out_up))
 
-    in_low = eval(in_low)
+    in_low = eval(replace_expr(in_low))
 
-    in_up = eval(in_up)
+    in_up = eval(replace_expr(in_up))
 
     out_up = eval(replace_bound(str(out_up)))
     out_low = eval(replace_bound(str(out_low)))
     in_up = eval(replace_bound(str(in_up)))
     in_low = eval(replace_bound(str(in_low)))
 
     result = integrate(function, (y, in_low, in_up), (x, out_low, out_up))
@@ -405,27 +453,21 @@
 
     print(
         f"\nDouble integral of [bright_magenta]{function}[/bright_magenta] with inner bounds [bright_cyan]{in_low}[/bright_cyan] and [bright_cyan]{in_up}[/bright_cyan] and outer bounds {out_low} and {out_up} is:\n"
     )
     print_expr(result)
     print("")
 
-    if check_simp(result) is True:
-        print("\nSimplify/rewrite:\n")
-        print_expr(simplify(result, evaluate=False))
-
+    check_simp(result)
 
-def lim(expr, value):
-    if "pi" in expr:
-        expr = expr.replace("pi", str(pi))
 
-    replace_expr(expr)
+def lim(expr: str, value: str):
+    expr = replace_expr(expr)
 
-    if check_bound(value) is False:
-        return ""
+    check_bound(value)
 
     value = float(eval(replace_bound(value)))
 
     l = limit(expr, x, value)
 
     if "Limit" in str(l):
         logging.warning("Cannot compute limit.")
@@ -440,37 +482,32 @@
         )
 
     else:
         print(
             f"\nLimit of [bright_magenta]{expr}[/bright_magenta] as x approaches {value} is:\n"
         )
         print_expr(l)
-        if check_simp(l) is True:
-            print("\nSimplify/rewrite:\n")
-            print_expr(simplify(l, evaluate=False))
+        check_simp(l)
 
 
-def side_lim(expr, value, direction):
-    if "pi" in expr:
-        expr = expr.replace("pi", str(pi))
+def side_lim(expr: str, value: str, direction: str):
+    expr = replace_expr(expr)
 
-    replace_expr(expr)
-
-    if check_bound(value) is False:
-        return ""
+    check_bound(value)
 
     value = float(eval(replace_bound(value)))
 
-    if direction == "left":
+    if direction == "left" or direction == "Left":
         direction_sign = "-"
 
-    elif direction == "right":
+    elif direction == "right" or direction == "Right":
         direction_sign = "+"
 
     else:
+        print()
         logging.error("\nTypeError: Direction is neither right or left.")
         return ""
 
     l = limit(expr, x, value, dir=direction_sign)
 
     if "Limit" in str(l):
         logging.warning("\nCannot compute limit.")
@@ -478,26 +515,32 @@
 
     print(
         f"\nLimit of [bright_magenta]{expr}[/bright_magenta] as x approaches {value} from the [bright_cyan]{direction}[/bright_cyan] is:\n"
     )
     print_expr(l)
 
 
-def eq_solve(mode):
+def eq_solve(mode: int):
     eq_list = []
 
-    if mode == "1":
+    if mode == 1:
         eq1 = input("\nEnter equation: ")
         left = eval(eq1[: eq1.find("=")])
         right = eval(eq1[eq1.find("=") + 1 :])
-        eq_set = solve(left - right)[0]
-        print("\nx:\n")
-        pprint(eq_set)
+        eq_set = solve(left - right)
+        if len(eq_set) == 0:
+            print()
+            logging.error("UnknownError: Cannot solve equation")
+        else:
+            print("\nx:\n")
+            for i in range(0, len(eq_set)):
+                pprint(eq_set[i])
+                print()
 
-    elif mode == "2":
+    elif mode == 2:
         eq1 = input("Enter first equation: ")
         left1 = eval(eq1[: eq1.find("=")])
         right1 = eval(eq1[eq1.find("=") + 1 :])
 
         eq2 = input("Enter second equation: ")
         left2 = eval(eq2[: eq2.find("=")])
         right2 = eval(eq2[eq2.find("=") + 1 :])
@@ -507,15 +550,15 @@
         for value in eqs:
             eq_list.append(value)
 
         result = "".join(eq_list)
         print("\nx, y:\n")
         pprint(result)
 
-    elif mode == "3":
+    elif mode == 3:
         eq1 = input("Enter equation 1: ")
         left1 = eval(eq1[: eq1.find("=")])
         right1 = eval(eq1[eq1.find("=") + 1 :])
 
         eq2 = input("Enter equation 2: ")
         left2 = eval(eq2[: eq2.find("=")])
         right2 = eval(eq2[eq2.find("=") + 1 :])
@@ -534,112 +577,90 @@
             eq_list.append(value)
 
         result = "".join(eq_list)
         print("\nx, y, z:\n")
         pprint(result)
 
 
-def check_simp(expr):
+def check_simp(expr) -> bool:
     if str(simplify(expr, evaluate=False)) != str(expr):
-        return True
+        print("\nSimplify/rewrite:\n")
+        print_expr(simplify(expr, evaluate=False))
 
     else:
         return False
 
 
-def check_order(order):
-    if ("." in order) or (order.isnumeric() == False) or (int(order) <= 0):
+def check_order(order: str) -> bool:
+    if ("." in order) or (order.isnumeric() == False):
+        print()
         logging.error(
             "OrderError: Order of derivative calculation is not a valid number."
         )
         return False
 
     else:
         return True
 
 
-def check_bound(bound):
+def check_bound(bound: str):
     if (
         (bound.isnumeric() is False)
         and ("pi" not in bound)
+        and ("e" not in bound)
         and ("E" not in bound)
         and ("-" not in bound)
         and ("." not in bound)
         and ("sqrt" not in bound)
         and ("oo" not in bound)
         and ("/" not in bound)
     ):
+        print()
         logging.error("TypeError: Integration bound is not a number.")
-        return False
 
-    else:
-        return True
 
+def replace_expr(expr: str) -> str:
+    expr = expr.strip(" ")
 
-def replace_expr(expr):
     if "^" in expr:
         expr = expr.replace("^", "**")
 
+    if "e" in expr:
+        expr = expr.replace("e", "E")
+
+    if "E**" in expr:
+        expr = expr.replace("E**", "exp")
+
+    if "ln" in expr:
+        expr = expr.replace("ln", "log")
+
     if "arc" in expr:
         expr = expr.replace("arc", "a")
-        print(
-            f'[bold bright_red]Showing results for "{expr}". (Did you make a mistake?)[/bold bright_red]'
-        )
+
+    if "abs" in expr:
+        expr = expr.replace("abs", "Abs")
 
     return expr
 
 
-def replace_bound(bound):
+def replace_bound(bound: str) -> str:
     if "pi" in bound:
-        bound = bound.replace("pi", str(pi.evalf()))
+        bound = bound.replace("pi", str(np.pi))
+
     if "E" in bound:
-        bound = bound.replace("E", str(E.evalf()))
+        bound = bound.replace("E", str(np.e))
 
     return bound
 
 
-def f(x):
-    if "Abs" in dfunction:
-        final = dfunction.replace("Abs", "fabs")
-    else:
-        final = dfunction
-
-    if "x" not in final:
-        final = "0 * x + " + final
-
-    final = eval(trig_rep(final))
-
-    return final
-
-
-def dif(x):
-    if "x" not in str(df):
-        final = eval("0 * x + " + trig_rep(str(df)))
-
-    else:
-        final = eval(df)
-
-    return final
-
-
-def af(x):
-    if "x" not in F:
-        final = eval("0 * x + " + F)
-
-    else:
-        final = eval(F)
-
-    return final
-
-
 def factorial(x):
     return gamma(x + 1)
 
 
-def trig_rep(function):
+def trig_rep(function: str) -> str:
     # Sympy and Numpy trig functions are vastly different
     # and uses different prefixes. Thus this replacement
     # algorithm is needed.
     if "asin" in function:
         function = function.replace("asin", "arcsin")
 
     if "acos" in function:
@@ -674,49 +695,56 @@
 
     if "sech" in function:
         function = function.replace("sech", "1/cosh")
 
     if "coth" in function:
         function = function.replace("coth", "1/tanh")
 
-    if "pi" in function:
-        function = function.replace("pi", str(np.pi))
+    if "Abs" in function:
+        function = function.replace("Abs", "fabs")
+
+    if "log" in function and ",x)" in function:
+        function = function.replace("log", "mt.log")
 
-    if "E" in function:
-        function = function.replace("E", str(np.e))
+    if "x" not in function:
+        function = "0 * x + " + function
 
     return function
 
 
-def print_expr(text):
+def print_expr(text: str):
     printing_methods = {"p": lambda t: pprint(text), "n": lambda t: print(text)}
 
     try:
         printing_methods[print_option](text)
 
     except NameError:
         printing_methods["p"](text)
 
 
-def err():
-    nprint(
-        "\n[bold bright_red]Check if your input is valid. You might have made the following mistakes:[/bold bright_red]"
-    )
-    nprint(
-        '[bold bright_red] - Inverse trigs: "arc" instead of "a". "asin(x)" is correct, "arcsin(x)" is not.[/bold bright_red]'
-    )
-    nprint('[bold bright_red] - Base of log: "e" instead of "E".[/bold bright_red]\n')
-
-
-def nprint(text):
+def nprint(text: str):
     print(text)
     time.sleep(0.04)
 
 
 def main():
+    with Progress(
+        SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
+        TextColumn("[green]Handling imports[/green]..."),
+        BarColumn(),
+        MofNCompleteColumn(),
+        TimeElapsedColumn(),
+        transient=False,
+    ) as progress:
+        task = progress.add_task("", total=50)
+
+        while not progress.finished:
+            progress.update(task, advance=1)
+            time.sleep(random.randint(2, 5) / 100)
+
     global x, y, z
     x, y, z = symbols("x, y, z")
 
     while True:
         instruct_path = (
             os.path.dirname(os.path.abspath(__file__))
             + "/texts/main_screen.txt"
@@ -793,59 +821,54 @@
             print("[bright_magenta]Enter Command: [/bright_magenta]", end="")
             cmd = input()
 
             if cmd == "1":
                 nprint(
                     "\n[bold bright_green](Current Screen: Derivative Screen)[/bold bright_green]\n"
                 )
-                global dfunction
-                dfunction = input("Enter a function: ")
+                function = input("Enter a function: ")
                 order = input("Enter order of derivative calculation: ")
-                derive(dfunction, order)
+                derive(function, order)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current Screen: Partial Derivative Screen)[/bold bright_green]\n"
                 )
                 function = input(
                     "Enter a function containing x and y or x and y and z: "
                 )
                 var = input("Enter variable to differentiate in respect to: ")
                 if var != "x" and var != "y" and var != "z":
-                    logging.error(
-                        "[bold bright_red]Variable to differentite in respect to is invalid.[/bold bright_red]"
-                    )
+                    print()
+                    logging.error("Variable to differentite in respect to is invalid.")
                 else:
                     order = input("Enter the order of partial derivative calculation: ")
                     partial_derive(function, var, order)
 
             elif cmd == "3":
                 nprint(
                     "\n[bold bright_green](Current Screen: Implicit Derivative Screen)[/bold bright_green]\n"
                 )
-                circ = input(
-                    "Enter the left side of an equation containing x and y: (right side default as 0) "
-                )
+                circ = input("Enter an equation containing x and y:")
                 order = input("Enter order of implicit derivative calculation: ")
                 implicit_derive(circ, order)
 
             elif cmd == "4":
                 print("\n[bright_yellow]Exiting DerivaCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
                 logging.warning(f'Invalid command:"{cmd}"')
         except:
+            print("\n")
             logging.error("UnknownError: An unknown error occured.")
-            err()
+            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def intecalc():
-    global dfunction
-
     instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/intecalc.txt"
     intecalc = open(instruct_path, mode="r")
     for line in intecalc.readlines():
         line = line.rstrip()
         if ("---" in line) or ("|" in line):
             nprint("[gold1]" + line + " [/gold1]")
         else:
@@ -860,25 +883,25 @@
             print("[bright_magenta]Enter Command: [/bright_magenta]", end="")
             cmd = input()
 
             if cmd == "1":
                 nprint(
                     "\n[bold bright_green](Current Screen: Antiderivative Screen)[/bold bright_green]\n"
                 )
-                dfunction = input("Enter a function: ")
-                antiderive(dfunction)
+                function = input("Enter a function: ")
+                antiderive(function)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current Screen: Definite Integral Screen)[/bold bright_green]\n"
                 )
-                dfunction = input("Enter a function: ")
+                function = input("Enter a function: ")
                 lower_bound = input("\nEnter the lower bound: ")
                 upper_bound = input("Enter the upper bound: ")
-                print(def_int(dfunction, lower_bound, upper_bound))
+                print(def_int(function, lower_bound, upper_bound))
 
             elif cmd == "3":
                 nprint(
                     "\n[bold bright_green](Current Screen: Improper Integral Screen)[/bold bright_green]\n"
                 )
                 function = input("Enter a function: ")
                 lower_bound = input("\nEnter the lower bound: ")
@@ -899,18 +922,17 @@
             elif cmd == "5":
                 print("\n[bright_yellow]Exiting InteCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
                 logging.warning(f'Invalid command: "{cmd}"')
         except:
-            logging.error(
-                "UnknownError: An unknown error occured. Try the following things:"
-            )
-            err()
+            print("\n")
+            logging.error("UnknownError: An unknown error occured.")
+            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def limcalc():
     instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/limcalc.txt"
     limcalc = open(instruct_path, mode="r")
     for line in limcalc.readlines():
         line = line.rstrip()
@@ -949,18 +971,17 @@
                 print("\n[bright_yellow]Exiting LimCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
                 logging.warning(f'Invalid command: "{cmd}"')
 
         except:
-            logging.error(
-                "UnknownError: An unknown error occured. Try the following things:"
-            )
-            err()
+            print("\n")
+            logging.error("UnknownError: An unknown error occured.")
+            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def algcalc():
     instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/algcalc.txt"
     algcalc = open(instruct_path, mode="r")
     for line in algcalc.readlines():
         line = line.rstrip()
@@ -982,15 +1003,15 @@
                 nprint(
                     "\n[bold bright_green](Current screen: Equation Solver Screen)[/bold bright_green]\n"
                 )
                 print(
                     "Enter mode: 1 for one set equation, 2 for two, and 3 for three: ",
                     end="",
                 )
-                mode = input()
+                mode = int(input())
                 eq_solve(mode)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current screen: Vector Calculation Screen)[/bold bright_green]\n"
                 )
 
@@ -1060,28 +1081,28 @@
                             print("\n[bright_yellow]Result: [/bright_yellow]\n")
                             pprint(result)
                             print()
 
                         else:
                             break
                     except:
+                        print("\n")
                         logging.error(f'Could not parse: "{expr}"\n')
 
             elif cmd == "4":
                 print("\n[bright_yellow]Exiting AlgCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
                 logging.warning(f'Invalid command: "{cmd}"')
 
         except:
-            logging.error(
-                "UnknownError: An unknown error occured. Try the following things:"
-            )
-            err()
+            print("\n")
+            logging.error("UnknownError: An unknown error occured.")
+            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def settings():
     while True:
         settings_path = (
             os.path.dirname(os.path.abspath(__file__)) + "/texts/settings.txt"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `calc_ultra-1.3.3/src/calc_ultra/texts/algcalc.txt` & `calc_ultra-1.3.4/src/calc_ultra/texts/algcalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.3/src/calc_ultra/texts/derivacalc.txt` & `calc_ultra-1.3.4/src/calc_ultra/texts/derivacalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.3/src/calc_ultra/texts/intecalc.txt` & `calc_ultra-1.3.4/src/calc_ultra/texts/intecalc.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,9 +16,7 @@
 --> 1: Calculate antiderivative
 --> 2: Calculate definite integral
 --> 3: Calculate improper integral
 --> 4: Calculate double integral
 --> 5: Exit InteCalc
 
 (Absolute value function and factorial function is only supported by definite integral computation)
-
-For definite integral calculation, use E for Euler's Constant.
```

### Comparing `calc_ultra-1.3.3/src/calc_ultra/texts/limcalc.txt` & `calc_ultra-1.3.4/src/calc_ultra/texts/limcalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.3/src/calc_ultra.egg-info/PKG-INFO` & `calc_ultra-1.3.4/src/calc_ultra.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.3
+Version: 1.3.4
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
@@ -17,23 +17,23 @@
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: rich>=13.7.1
 Requires-Dist: scipy>=1.12.0
 
 # calc-ultra
 
-[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.3-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
+[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.4-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic)
 
-The Calc-ULTRA calculus calculator, but as a module!
+The Calc-Ultra calculus calculator, but as a module!
 
-- Little Python background knowledge needed!
+- Little Python background knowledge is needed!
 
 Supports:
 
 - Derivatives
 - Partials
 - Implicit differentiation
 - Antiderivatives
@@ -42,38 +42,38 @@
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
 ## Note
 
-This is the module package of the Calc-ULTRA calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
+This is the module package of the Calc-Ultra calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
 Command line: `pip3 install calc-ultra`.
-Due to Python import identifiers restrictions, please import Calc-ULTRA as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
+Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
 
 To run the calculator, import Calc-ULTRA as `calc_ultra` like so:
 
 `from calc_ultra import main`
 
 Make sure you have the latest version installed. To update calc-ultra, run `pip3 install --upgrade calc-ultra`.
 
 ## Requirements
 
-This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built in to most Python IDEs.
+This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built into most Python IDEs.
 
 ## Warnings
 
 ### Function limitations
 
-Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions are also limited due to SymPy limitations. While some composed functions work, others don't. 😟
+Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions is also limited due to SymPy limitations. While some composed functions work, others don't. 😟
 
 ## Test PYPI
 
 Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>.
 
 ## Acknowledgements
 
@@ -83,30 +83,30 @@
 And... a SPECIAL THANK-YOU to @Haobot for troubleshooting and feedback! 👍❤️
 
 This program was made using SymPy and Scipy for calculation and Matplotlib and NumPy for graphing.
 
 ## Gallery
 
 DerivaCalc derivative with graph demo:
-![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/22f7f674-81b4-4e5f-9bff-586d94c1976f "derivacalc_demo")
+![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
-![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/1035a5af-cf04-46c1-b2e3-ec5eff08c58d "intecalc_demo_1")
+![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
 
 InteCalc definite integral with graph demo:
-![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/42a127af-17f6-4608-a6aa-9029cf00e973 "intecalc_demo_2")
+![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b8294186-92f5-4df3-a000-d63f6fff93b0 "intecalc_demo_2")
 
 LimCalc limit demo:
-![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/bb08db05-9b1b-4204-9d98-d4a3baa2167d "limcalc_demo")
+![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/12db6a7b-a836-43ce-8cef-7bcf707051f7 "limcalc_demo")
 
 AlgCalc equation solver demo:
-![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7d2bdad0-572c-4eec-8644-2837a0689154 "algcalc_demo_1")
+![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/e4cfa016-52bf-43b5-a839-af9f42546468 "algcalc_demo_1")
 
 AlgCalc vector operation demo:
-![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/28c5143b-93fc-4165-b8d9-572d1ab00da8 "algcalc_demo_2")
+![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7f043cb2-6b0a-4460-ab35-30f09632b1c3 "algcalc_demo_2")
 
 AlgCalc matrix operation demo:
-![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b6d11f38-b5b8-42ed-b4b3-664c65207664 "algcalc_demo_3")
+![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/a9a5d56e-424a-4ef8-beb9-a9b64ce1a3f5 "algcalc_demo_3")
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `calc_ultra-1.3.3/src/calc_ultra.egg-info/SOURCES.txt` & `calc_ultra-1.3.4/src/calc_ultra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

