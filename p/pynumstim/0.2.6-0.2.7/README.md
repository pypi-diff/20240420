# Comparing `tmp/pynumstim-0.2.6.tar.gz` & `tmp/pynumstim-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.6.tar` & `pynumstim-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.6/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.6/LICENSE
--rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.6/README.md
--rw-r--r--   0        0        0      362 2024-04-15 15:24:22.103263 pynumstim-0.2.6/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.6/pynumstim/_data_sets.py
--rw-r--r--   0        0        0     7878 2024-04-15 15:23:44.146633 pynumstim-0.2.6/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.6/pynumstim/_number.py
--rw-r--r--   0        0        0     9404 2024-04-15 14:02:41.097568 pynumstim-0.2.6/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.6/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.6/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4513 2024-04-15 13:57:57.608656 pynumstim-0.2.6/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.6/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.6/trial_list.txt
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.7/LICENSE
+-rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.7/README.md
+-rw-r--r--   0        0        0      362 2024-04-20 11:24:43.126941 pynumstim-0.2.7/pynumstim/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-18 16:18:12.229886 pynumstim-0.2.7/pynumstim/_data_sets.py
+-rw-r--r--   0        0        0    12942 2024-04-20 11:24:17.654382 pynumstim-0.2.7/pynumstim/_mplist.py
+-rw-r--r--   0        0        0     3344 2024-04-18 14:51:30.308979 pynumstim-0.2.7/pynumstim/_number.py
+-rw-r--r--   0        0        0     9720 2024-04-18 17:53:40.832655 pynumstim-0.2.7/pynumstim/_problem.py
+-rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.7/pynumstim/datasets/Ahren_Jackson_79.toml
+-rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.7/pynumstim/datasets/Lindemann_Tira_10.toml
+-rw-r--r--   0        0        0     4513 2024-04-18 16:18:12.229886 pynumstim-0.2.7/pynumstim/image.py
+-rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.7/trial_list.txt
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.7/PKG-INFO
```

### Comparing `pynumstim-0.2.6/.gitignore` & `pynumstim-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.6/LICENSE` & `pynumstim-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.6/README.md` & `pynumstim-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.6/pynumstim/_data_sets.py` & `pynumstim-0.2.7/pynumstim/_data_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     @classmethod
     def Lindemann_Tira_10(cls) -> MathProblemList:
         return cls.read_dataset("Lindemann_Tira_10.toml")
 
     @staticmethod
     def problem_space(operation: str,
-                      operant1: List[int],
-                      operant2: List[int],
+                      operand1: List[int],
+                      operand2: List[int],
                       incorrect_deviations: Optional[List[int]] = None,
                       decade_results=True,
                       tie_problem=True,
                       negative_results=True,
                       carry_problems=True,
                       properties: Optional[TProperties] = None) -> MathProblemList:
         """creates a MathProblemList comprising the defined problem space
@@ -39,16 +39,16 @@
         if incorrect_deviations is None:
             inc_dev = set()
         else:
             inc_dev = set(incorrect_deviations)
         inc_dev.add(0)  # correct result
 
         rtn = MathProblemList()
-        for op1 in operant1:
-            for op2 in operant2:
+        for op1 in operand1:
+            for op2 in operand2:
                 if tie_problem or op1 != op2:
                     for dev in inc_dev:
                         p = MathProblem(op1, operation, op2)
                         correct = p.calc()
                         result = correct + dev
                         if not decade_results and (result % 10 == 0 or correct % 10 == 0):
                             continue
```

### Comparing `pynumstim-0.2.6/pynumstim/_number.py` & `pynumstim-0.2.7/pynumstim/_number.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,29 +49,27 @@
         return Num(self.py_number / Num(val2).py_number)
 
     __rmul__ = __mul__
 
     @property
     def py_number(self) -> TPyNum:
         """returns Python Rational (int, Fraction) or float  for calculations"""
-        if isinstance(self.numerator, Num):
-            n = self.numerator.py_number
+        if self.denominator == 1: # is not fraction
+            return self.numerator
+        elif isinstance(self.numerator, float) or isinstance(self.denominator, float):
+            return self.numerator / self.denominator
         else:
-            n = self.numerator
-        if isinstance(self.denominator, Num):
-            d = self.denominator.py_number
-        else:
-            d = self.denominator
+            return Fraction(self.numerator, self.denominator)
 
-        if d == 1:
-            return n
-        if isinstance(n, float) or isinstance(d, float):
-            return n / d
+    @property
+    def number_type(self) -> type:
+        if self.denominator != 1:
+            return Fraction
         else:
-            return Fraction(n, d)
+            return type(self.numerator)
 
     def is_fraction(self):
         return self.denominator != 1
 
     def tex(self) -> str:
         if self.is_fraction():
             return f"\\frac{{{self.numerator}}}{{{self.denominator}}}"
```

### Comparing `pynumstim-0.2.6/pynumstim/_problem.py` & `pynumstim-0.2.7/pynumstim/_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 from copy import copy
 from fractions import Fraction
 from hashlib import md5
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Set
 
 from ._number import Num, TNum, TPyNum
 
 LATEX_TIMES = "\\times"  # "\\cdot"
 LATEX_SYMBOL_NAMES = {"=": "equal",
                 "+": "plus",
                 LATEX_TIMES: "multiply",
@@ -21,43 +21,43 @@
 class MathProblem(object):
 
     LABEL_MULTI = "t"  # multiplication, times
     LABEL_DIVIDE = "d"  # divide
     OPERATIONS = ["+", "-", "*", "/", LABEL_MULTI, LABEL_DIVIDE]
 
     def __init__(self,
-                 operant1: TNum,
+                 operand1: TNum,
                  operation: str,
-                 operant2: TNum,
+                 operand2: TNum,
                  result: Optional[TNum] = None,
                  properties: Optional[TProperties] = None) -> None:
         """properties: dict of properties.
                         Keys repesent the property name and must be text strings
         """
 
         self.operation = operation
-        self.operant1 = operant1
-        self.operant2 = operant2
+        self.operand1 = operand1
+        self.operand2 = operand2
         self.result = result
         self.properties = copy(properties)
 
     @property
-    def operant1(self) -> Num:
+    def operand1(self) -> Num:
         return self._op1
 
-    @operant1.setter
-    def operant1(self, val: TNum):
+    @operand1.setter
+    def operand1(self, val: TNum):
         self._op1 = Num(val)
 
     @property
-    def operant2(self) -> Num:
+    def operand2(self) -> Num:
         return self._op2
 
-    @operant2.setter
-    def operant2(self, val: TNum):
+    @operand2.setter
+    def operand2(self, val: TNum):
         self._op2 = Num(val)
 
     @property
     def result(self) -> Optional[Num]:
         return self._result
 
     @result.setter
@@ -78,14 +78,23 @@
         if val == MathProblem.LABEL_MULTI:
             self._operation = "*"
         elif val == MathProblem.LABEL_DIVIDE:
             self._operation = "/"
         else:
             self._operation = val
 
+    @property
+    def number_types(self) -> Set[type]:
+        rtn = set((self.operand1.number_type, self.operand2.number_type))
+        if self.result is not None:
+            rtn.add(self.result.number_type)
+            return rtn
+        else:
+            return rtn
+
     def operation_label(self):
         if self._operation == "*":
             return self.LABEL_MULTI
         elif self._operation == "/":
             return self.LABEL_DIVIDE
         else:
             return self._operation
@@ -209,25 +218,25 @@
             return False
         return self.calc() == self._result.py_number
 
     def n_carry(self) -> Optional[int]:
         """number of carry operations for addition and subtraction
         else None"""
 
-        if self.operant1.is_fraction() or self.operant2.is_fraction():
+        if self.operand1.is_fraction() or self.operand2.is_fraction():
             return None
         if self.operation == "+":
             subtraction = False
         elif self.operation == "-":
             subtraction = True
         else:
             return None
 
-        str_op1 = str(self.operant1)
-        str_op2 = str(self.operant2)
+        str_op1 = str(self.operand1)
+        str_op2 = str(self.operand2)
         # Get the length of the longer number
         max_length = max(len(str_op1), len(str_op2))
         # Add leading zeros to make the numbers have the same length
         str_op1 = str_op1.zfill(max_length)
         str_op2 = str_op2.zfill(max_length)
 
         current_carry = 0
@@ -246,15 +255,15 @@
                 current_carry = 1
             else:
                 current_carry = 0
 
         return ncarry
 
     def problem_size(self) -> float:
-        return (_size(self.operant1) + _size(self.operant1)) / 2.0
+        return (_size(self.operand1) + _size(self.operand2)) / 2.0
 
     @staticmethod
     def parse(txt: str, properties: Optional[TProperties] = None) -> MathProblem:
         """fractions have to presented like in labels: frac5_6
         can also convert labels to problems
         """
         x = txt.split("=")
@@ -275,35 +284,35 @@
 
             if None not in (op1, op2, operation):
                 return MathProblem(
                     op1, operation, op2, result, properties)  # type: ignore
 
         raise ValueError(f"Can't convert '{txt}' to MathProblem.")
 
-    def is_tie(self) -> bool:
-        return self.operant1 == self.operant2
+    def same_operands(self) -> bool:
+        return self.operand1.py_number == self.operand2.py_number
 
-    def has_decade_solution(self) -> bool:
+    def decade_solution(self) -> bool:
         return self.calc() % 10 == 0
 
-    def has_same_parities(self) -> bool:
-        return self.operant1.py_number % 2 == self.operant2.py_number % 2
+    def same_parities(self) -> bool:
+        return self.operand1.py_number % 2 == self.operand2.py_number % 2
 
 
 def _split_after_digit(txt: str, letter: str):
     # splits txt at letter only if a digit proceeds the letter
-    if letter in ["+", "*", "\\"]:
+    if letter in ["+", "*", "\\"]: # escaping required
         letter = f"\\{letter}"
     a = re.search(f"\\d\\s*{letter}", txt)
     if a is not None:
         return txt[:a.span()[0]+1], txt[a.span()[1]:]
     else:
         return txt
 
 
 def _size(num: Num) -> TPyNum:
     """helper for calculation problem size with fractions.
-    In this case, return mean of numerator and denomintor"""
+    In this case, return mean of numerator and denominator"""
     if num.is_fraction():
         return (num.numerator + num.denominator) / 2.0
     else:
         return num.py_number
```

### Comparing `pynumstim-0.2.6/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.2.7/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.6/pynumstim/image.py` & `pynumstim-0.2.7/pynumstim/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         _from_tex(f"$${problem.tex()}$$", filename=flname,
                   resolution=resolution, fg=fg, bg=bg)
     else:
         # segmented
         os.makedirs(folder, exist_ok=True)
         _create_latex_symbols(folder, resolution=resolution, fg=fg, bg=bg)
         stim = set()
-        stim.add((problem.operant1.tex(), problem.operant1.label()))
-        stim.add((problem.operant2.tex(), problem.operant2.label()))
+        stim.add((problem.operand1.tex(), problem.operand1.label()))
+        stim.add((problem.operand2.tex(), problem.operand2.label()))
         if problem.result is not None:
             stim.add((problem.result.tex(), problem.result.label()))
         for tex, label in stim:
             print("png: " + label)
             _from_tex(f"$${tex}$$",
                       filename=os.path.join(folder, "n" + f"{label}.png"),
                       resolution=resolution, fg=fg, bg=bg)
@@ -98,16 +98,16 @@
                 done.add(x.label())
     else:
         _create_latex_symbols(folder=folder,
                               resolution=resolution, fg=fg, bg=bg)
         # problem_stimuli
         stim = set()
         for x in problems.list:
-            stim.add((x.operant1.tex(), x.operant1.label()))
-            stim.add((x.operant2.tex(), x.operant2.label()))
+            stim.add((x.operand1.tex(), x.operand1.label()))
+            stim.add((x.operand2.tex(), x.operand2.label()))
             if x.result is not None:
                 stim.add((x.result.tex(), x.result.label()))
 
         for tex, label in stim:
             print("png: " + label)
             _from_tex(f"$${tex}$$",
                       filename=os.path.join(folder, "n" + f"{label}.png"),
```

### Comparing `pynumstim-0.2.6/pyproject.toml` & `pynumstim-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.6/trial_list.txt` & `pynumstim-0.2.7/trial_list.txt`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.6/PKG-INFO` & `pynumstim-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumstim
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python library to create symbolic number and arithmetic stimuli for psychological experiments
 Keywords: experiment control,open science,experimental psychology
 Author-email: Oliver Lindemann <lindemann@essb.eur.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

