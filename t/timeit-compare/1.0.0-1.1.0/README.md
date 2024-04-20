# Comparing `tmp/timeit_compare-1.0.0.tar.gz` & `tmp/timeit_compare-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeit_compare-1.0.0.tar", last modified: Sun Apr 14 07:54:19 2024, max compression
+gzip compressed data, was "timeit_compare-1.1.0.tar", last modified: Sat Apr 20 09:38:21 2024, max compression
```

## Comparing `timeit_compare-1.0.0.tar` & `timeit_compare-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 07:54:19.870986 timeit_compare-1.0.0/
--rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3236 2024-04-14 07:54:19.870986 timeit_compare-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2024-04-14 07:22:46.000000 timeit_compare-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 07:54:19.870986 timeit_compare-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1224 2024-04-14 06:48:02.000000 timeit_compare-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 07:54:19.864973 timeit_compare-1.0.0/timeit_compare.egg-info/
--rw-rw-rw-   0        0        0     3236 2024-04-14 07:54:19.000000 timeit_compare-1.0.0/timeit_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-04-14 07:54:19.000000 timeit_compare-1.0.0/timeit_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 07:54:19.000000 timeit_compare-1.0.0/timeit_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 07:54:19.000000 timeit_compare-1.0.0/timeit_compare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12328 2024-04-14 06:34:06.000000 timeit_compare-1.0.0/timeit_compare.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:38:21.881777 timeit_compare-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4063 2024-04-20 09:38:21.881777 timeit_compare-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3122 2024-04-20 09:22:45.000000 timeit_compare-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 09:38:21.881777 timeit_compare-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2024-04-20 08:45:51.000000 timeit_compare-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:38:21.881777 timeit_compare-1.1.0/timeit_compare.egg-info/
+-rw-rw-rw-   0        0        0     4063 2024-04-20 09:38:21.000000 timeit_compare-1.1.0/timeit_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-04-20 09:38:21.000000 timeit_compare-1.1.0/timeit_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 09:38:21.000000 timeit_compare-1.1.0/timeit_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-20 09:38:21.000000 timeit_compare-1.1.0/timeit_compare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17902 2024-04-20 08:14:24.000000 timeit_compare-1.1.0/timeit_compare.py
```

### Comparing `timeit_compare-1.0.0/LICENSE` & `timeit_compare-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeit_compare-1.0.0/PKG-INFO` & `timeit_compare-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,28 @@
-Metadata-Version: 2.1
-Name: timeit_compare
-Version: 1.0.0
-Summary: A method based on timeit that can help you to call timeit.timeit for several statements and provide comparison results.
-Home-page: https://github.com/AomandeNiuma/timeit_compare
-Author: Liu Wei
-Author-email: 23S112099@stu.hit.edu.cn
-Maintainer: Liu Wei
-Maintainer-email: 23S112099@stu.hit.edu.cn
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # timeit_compare
 
 A method based on timeit that can help you to call timeit.timeit for several
 statements and provide comparison results.
 
 ------------------------------
 
 ## Installation
 
 You can run the following command to install the package
 
-```
+```commandline
 pip install timeit_compare
 ```
 
 ------------------------------
 
 ## Usage
 
-When using the timeit library, I am always more interested in comparing the 
-efficiency of several different methods to solve a problem, rather than simply 
+When using the timeit library, I am always more interested in comparing the
+efficiency of several different methods to solve a problem, rather than simply
 measuring the running time of a single statement. Here is a simple example.
 
 ```python
 from functools import reduce
 from operator import add
 
 n = 100
@@ -77,58 +54,79 @@
 
 def sum5():
     return (1 + n) * n // 2
 ```
 
 The functions above are all used to sum numbers from 1 to 100, which one is the
 most efficient?  
-This problem can be easily solved by the following method:
-
-```python 
-from timeit import timeit
-
-print(timeit(sum1))
-print(timeit(sum2))
-print(timeit(sum3))
-print(timeit(sum4))
-print(timeit(sum5))
-```
-
-and get the results like:
-
-```
-3.2710195999825373
-2.050656799983699
-0.4511557999649085
-2.5759165000054054
-0.066161299997475
-```
-
-Calling timeit multiple times and printing the results makes me feel 
-troublesome, and the results seem to be not intuitive.
-
 By using:
 
 ```python
 from timeit_compare import compare
 
 compare(sum1, sum2, sum3, sum4, sum5)
 ```
 
 you can easily get the results like:
 
 [![output_example.png](https://raw.githubusercontent.com/AomandeNiuma/timeit_compare/main/output_example.png)](
 https://raw.githubusercontent.com/AomandeNiuma/timeit_compare/main/output_example.png)
 
-The output provides detailed results, including the mean, median, minimum, 
+The output provides detailed results, including the mean, median, minimum,
 maximum and standard deviation of each function's running time.
 
 ------------------------------
 
+## Release Notes
+
+### Release 1.1.0
+
+1. The results now show the time of one loop in seconds(s), milliseconds(ms),
+   microseconds(μs), or nanoseconds(ns) instead of the total time of each
+   repetition. The conversion relationship among time units is as follows:
+
+   ```
+   1(s) = 10^3(ms) = 10^6(μs) = 10^9(ns)
+   ```
+
+2. Now the compare function supports setting parameters setup and globals
+   separately for each statement. Keyword parameters setup and globals are
+   now used to set the default parameter values for each statement.
+
+   ```python
+   from timeit_compare import compare
+   
+   stmt = '(1 + n) * n // 2'
+   compare(
+       stmt,
+       (stmt, 'n = 100', {}),
+       (stmt, '', {'n': 100}),
+       setup='n = 100'
+   )
+   ```
+
+3. If parameter number is not given or is less than or equal to 0, it now
+   defaults to a value that makes the total running time not too long. You can
+   intentionally set it to a higher value to make the results more accurate.
+
+4. Command line calls are now supported.
+
+   ```commandline
+   python -m timeit_compare -s "n = 100" "(1 + n) * n / 2" "sum(range(1, n + 1))"
+   ```
+
+   Run the following command for help.
+
+   ```commandline
+   python -m timeit_compare -h
+   ```
+
+------------------------------
+
 ## Contact
 
-If you have any suggestions, please contact me at 
+If you have any suggestions, please contact me at
 [23S112099@stu.hit.edu.cn](mailto:23S112099@stu.hit.edu.cn).
 
 ------------------------------
 
-## End
+## End
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timeit_compare-1.0.0/setup.py` & `timeit_compare-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='timeit_compare',
-    version='1.0.0',
+    version='1.1.0',
     py_modules=['timeit_compare'],
     license='MIT',
     python_requires='>=3.6.0',
     description='A method based on timeit that can help you to call '
                 'timeit.timeit for several statements and provide '
                 'comparison results.',
     long_description=long_description,
```

### Comparing `timeit_compare-1.0.0/timeit_compare.py` & `timeit_compare-1.1.0/timeit_compare.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,99 @@
 """
 A method based on timeit that can help you to call timeit.timeit for several
 statements and provide comparison results.
 
-Function 'compare' only.
+In-Script usage:
+    from timeit_compare import compare
+
+    compare(*stmts[, setup][, globals][, number][, repeat][, sort_by]
+        [, reverse][, decimal])
+
+See parameters in the function compare.
+
+Command line usage:
+    python -m timeit_compare.py [-s] [-n] [-r] [--sort-by] [--reverse] [-d]
+        [-h] [--] [statements]
+
+See options in the function main.
+
+Note that if an error occurs during the operation of a statement, the
+program will stop timing this statement, display the error type in the
+error cell of the final results, and then continue to time other statements
+without errors.
+
+If you actively terminate the program, all statements immediately stop
+timing and output the results obtained before the program terminates.
+
+To ensure a good user experience, the output terminal should utilize a font
+that has a fixed width and supports unicode characters. Additionally, it
+should refrain from automatically wrapping text to a new line when it
+becomes excessively long. The default output terminal in PyCharm is a good
+example.
 """
 
-from timeit import Timer, default_timer
-from typing import Callable, Union
+from time import perf_counter
+from timeit import Timer
+from typing import Sequence, Callable, Union
 
 __all__ = ['compare']
 
 
 class _TimerTask:
     """Internal class."""
 
-    def __init__(self, index, stmt, setup, number):
+    def __init__(self, index, stmt, setup, globals):
         self.index = index
         self.stmt = stmt
-        self.number = number
 
         try:
-            timer = Timer(stmt, setup)
+            timer = Timer(stmt, setup, perf_counter, globals)
         except Exception as e:
             timer = None
             error = type(e)
         else:
             error = None
         self.timer = timer
         self.error = error
 
         self.time = []
         self.repeat = 0
 
-    def timeit(self):
+    def autorange_timeit(self, number):
+        if self.error is None:
+            try:
+                time = self.timer.timeit(number)
+            except Exception as e:
+                self.error = type(e)
+            else:
+                return time
+
+    def autorange_interrupt(self, e):
+        if self.error is None:
+            self.error = type(e)
+
+    def timeit(self, number):
         if self.error is None:
             try:
-                time = self.timer.timeit(self.number)
+                time = self.timer.timeit(number)
             except Exception as e:
                 self.error = type(e)
                 return True
             else:
-                self.time.append(time)
+                self.time.append(time / number)
                 self.repeat += 1
         return False
 
+    def interrupt(self, e, repeat):
+        if self.error is None:
+            if self.repeat < repeat:
+                self.error = type(e)
+                return True
+        return False
+
     def analyse(self):
         if self.time:
             mean = sum(self.time) / self.repeat
 
             sorted_time = sorted(self.time)
 
             i = self.repeat // 2
@@ -77,147 +123,199 @@
         else:
             mean_percent = median_percent = None
 
         self.mean_percent = mean_percent
         self.median_percent = median_percent
 
     _null = '--'
+    _units = (('s', 1.0), ('ms', 1e-3), ('μs', 1e-6), ('ns', 1e-9))
 
-    def get_line(self, decimal):
+    def get_line(self, decimal, repeat):
         index = f'{self.index}'
 
         if isinstance(self.stmt, str):
             stmt = repr(self.stmt)
             if len(stmt) > 25:
                 stmt = f"{stmt[:25]} ...'"
         elif callable(self.stmt):
             stmt = getattr(self.stmt, '__name__', self._null)
             if len(stmt) > 25:
                 stmt = f'{stmt[:25]} ...'
         else:
             stmt = self._null
 
-        repeat = f'{self.repeat}'
-
         if self.time:
-            mean = f'{self.mean:.{decimal}f}s'
+            for unit, scale in self._units:
+                if self.min >= scale:
+                    break
+
+            def format_time(second):
+                return f'{second / scale:.{decimal}f}'
+
+            mean = format_time(self.mean)
             mean_percent = f'{self.mean_percent:.2%}'
             mean_process = _get_process(self.mean_percent, 8)
 
-            median = f'{self.median:.{decimal}f}s'
+            median = format_time(self.median)
             median_percent = f'{self.median_percent:.2%}'
             median_process = _get_process(self.median_percent, 8)
 
-            min_ = f'{self.min:.{decimal}f}s'
-            max_ = f'{self.max:.{decimal}f}s'
-            std = f'{self.std:.{decimal}f}'
+            min_ = format_time(self.min)
+            max_ = format_time(self.max)
+            std = format_time(self.std)
 
         else:
-            mean = mean_percent = mean_process = \
+            unit = mean = mean_percent = mean_process = \
                 median = median_percent = median_process = \
                 min_ = max_ = std = self._null
 
         if self.error is not None:
             error = self.error.__name__
+            if self.repeat < repeat:
+                error = f'{error}(r={self.repeat})'
         else:
             error = self._null
 
         return [
-            index, stmt, repeat,
+            index, stmt, unit,
             mean, mean_percent, mean_process,
             median, median_percent, median_process,
             min_, max_, std,
             error
         ]
 
 
 def compare(
-        *stmts: Union[str, Callable],
-        setup: str = 'pass',
-        number: int = 100_000,
-        repeat: int = 10,
+        *stmts: Union[Sequence, str, Callable],
+        setup: Union[str, Callable] = 'pass',
+        globals: dict = None,
+        number: int = 0,
+        repeat: int = 5,
         sort_by: str = 'mean',
         reverse: bool = False,
-        decimal: int = 4
+        decimal: int = 3
 ) -> None:
     """
     Call timeit.timeit for several statements and provide comparison results.
 
-    :param stmts: several statements to be compared,
-    :param setup: setup statement,
-    :param number: number of times per repetition,
-    :param repeat: number of repetitions,
+    :param stmts: (statement, setup, globals) or a single statement to be
+        compared.
+    :param setup: default setup for each statement (default 'pass').
+    :param globals: default globals for each statement (default globals()).
+    :param number: number of loops per repetition (default: see below).
+    :param repeat: number of repetitions (default 5).
     :param sort_by: the basis for sorting the results, which can be 'index',
-        'mean'(default), 'median', 'min', 'max' or 'std',
-    :param reverse: set True to sort the results in descending order,
-    :param: decimal: number of decimal places reserved for results,
-    :returns: None.
-
-    Note that if an error occurs during the operation of a statement, the
-    program will stop timing this statement, display the error type in the
-    error cell of the final results, and then continue to time other statements
-    without errors.
-
-    If you actively terminate the program, all statements immediately stop
-    timing and output the results obtained before the program terminates.
-
-    To ensure a good user experience, the output terminal should utilize a font
-    that has a fixed width and supports unicode characters. Additionally, it
-    should refrain from automatically wrapping text to a new line when it
-    becomes excessively long. The default output terminal in PyCharm is a good
-    example.
+        'mean', 'median', 'min', 'max' or 'std' (default 'mean').
+    :param reverse: set True to sort the results in descending order (default
+        False).
+    :param decimal: number of decimal places reserved for results (default 3).
+    :returns: None
+
+    If number is not given or is less than or equal to 0, it defaults to a
+    value that makes the total running time not too long. You can intentionally
+    set it to a higher value to make the results more accurate.
     """
 
-    start = default_timer()
+    start = perf_counter()
+
+    timer_args = []
+
+    for stmt in stmts:
+        if isinstance(stmt, Sequence) and not isinstance(stmt, str):
+            if len(stmt) > 3:
+                raise ValueError(f'stmt expected at most 3 argument, '
+                                 f'got {len(stmt)}')
+            args = ['pass', setup, globals]
+            for i, j in enumerate(stmt):
+                if j is not None:
+                    args[i] = j
+        else:
+            args = stmt, setup, globals
+
+        timer_args.append(args)
+
+    if not isinstance(number, int):
+        raise TypeError(f'number must be a integer, not {type(number)}')
+    if number < 0:
+        number = 0
 
     if not isinstance(repeat, int):
         raise TypeError(f'repeat must be a integer, not {type(repeat)}')
+    if repeat <= 0:
+        repeat = 1
 
     if not isinstance(sort_by, str):
         raise TypeError(f'sort_by must be a string, not {type(sort_by)}')
-
     sort_by = sort_by.lower()
-
     if sort_by not in {'index', 'mean', 'median', 'min', 'max', 'std'}:
         raise ValueError(
             f'sort_by must be index, mean, median, min, max or '
             f'std, not {sort_by}')
 
+    try:
+        reverse = bool(reverse)
+    except:
+        raise TypeError(f'reverse must be a boolean, not {type(reverse)}')
+
     if not isinstance(decimal, int):
         raise TypeError(f'decimal must be a integer, not {type(decimal)}')
-
     if decimal < 0:
-        raise ValueError(f'decimal must be greater than 0')
+        decimal = 0
+
+    # ________________________________________________________________________
+
+    task = [_TimerTask(index, *args) for index, args in enumerate(timer_args)]
+
+    print('timing now...')
+
+    if number == 0:
+        def autorange():
+            i = 1
+            while True:
+                for j in 1, 2, 5:
+                    number = i * j
+                    time_taken = 0.0
+                    all_error = True
+                    for item in task:
+                        time = item.autorange_timeit(number)
+                        if time is not None:
+                            time_taken += time
+                            all_error = False
+                    if all_error:
+                        return 0
+                    if time_taken > 0.2:
+                        return number
+                i *= 10
+
+        try:
+            number = autorange()
+        except (KeyboardInterrupt, SystemExit) as e:
+            for item in task:
+                item.autorange_interrupt(e)
 
-    task = [_TimerTask(index, stmt, setup, number) for index, stmt in
-            enumerate(stmts)]
     task_num = len(task)
     total_repeat = task_num * repeat
     complete = 0
     error = sum(item.error is not None for item in task)
-
-    print('timing now...')
     _update_process(complete, total_repeat, error, task_num)
 
     try:
         for _ in range(repeat):
             for item in task:
-                e = item.timeit()
-                if e:
+                turn_error = item.timeit(number)
+                if turn_error:
                     error += 1
                 complete += 1
                 _update_process(complete, total_repeat, error, task_num)
 
     except (KeyboardInterrupt, SystemExit) as e:
-        error_type = type(e)
         for item in task:
-            if item.error is None:
-                if item.repeat < repeat:
-                    item.error = error_type
-                    error += 1
+            turn_error = item.interrupt(e, repeat)
+            if turn_error:
+                error += 1
         complete = total_repeat
         _update_process(complete, total_repeat, error, task_num)
 
     print()
 
     result = []
     max_mean = 0.0
@@ -235,17 +333,19 @@
 
     for item in task:
         item.set_percent(max_mean, max_median)
 
     result.sort(key=lambda item: getattr(item, sort_by), reverse=reverse)
     result.extend(item for item in task if not item.time)
 
+    # ________________________________________________________________________
+
     # make table
     title = 'Comparison Results'
-    header = ['Index', 'Stmt', 'Repeat', 'Mean', 'Median', 'Min-Max', 'Std',
+    header = ['Index', 'Stmt', 'Unit', 'Mean', 'Median', 'Min-Max', 'Std',
               'Error']
     sort_by_tip = '(SortBy)'
     if sort_by == 'index':
         header[0] += sort_by_tip
     elif sort_by == 'mean':
         header[3] += sort_by_tip
     elif sort_by == 'median':
@@ -253,19 +353,20 @@
     elif sort_by == 'min':
         header[5] = f'Min{sort_by_tip}-Max'
     elif sort_by == 'max':
         header[5] = f'Min-Max{sort_by_tip}'
     else:  # sort_by == 'std'
         header[6] += sort_by_tip
     header_cols = [1, 1, 1, 3, 3, 2, 1, 1]
-    body = [task.get_line(decimal) for task in result]
-    note = f'{number:_} loops per repetition'
+    body = [task.get_line(decimal, repeat) for task in result]
+    note = (f"{repeat} repetition{'s' if repeat != 1 else ''}, "
+            f"{number:_} loop{'s' if number != 1 else ''} each.")
     _print_table(1, title, header, header_cols, body, note)
 
-    end = default_timer()
+    end = perf_counter()
     print(f'finish at {end - start:.4f}s')
 
 
 BLOCK = ' ▏▎▍▌▋▊▉█'
 
 
 def _get_process(process, length):
@@ -351,30 +452,23 @@
     title_line = f'{{:^{total_width}}}'
     header_line = f"{dl}│{'│'.join(f'{{:^{hw}}}' for hw in header_width)}│{dr}"
     body_line = f"{dl}│{'│'.join(f'{{:^{bw}}}' for bw in body_width)}│{dr}"
     note_line = f'{{:<{total_width}}}'
 
     top_border = f"{dl}╭{'┬'.join('─' * hw for hw in header_width)}╮{dr}"
     bottom_border = f"{dl}╰{'┴'.join('─' * bw for bw in body_width)}╯{dr}"
-
     split_border = []
-    i = 0
+    bw = iter(body_width)
     for col in header_cols:
         if col == 1:
-            bw = body_width[i]
-            split_border.append('─' * bw)
-            split_border.append('┼')
+            border = '─' * next(bw)
         else:
-            for bw in body_width[i: i + col]:
-                split_border.append('─' * bw)
-                split_border.append('┬')
-            split_border[-1] = '┼'
-        i += col
-    split_border.pop()
-    split_border = f"{dl}├{''.join(split_border)}┤{dr}"
+            border = '┬'.join('─' * next(bw) for _ in range(col))
+        split_border.append(border)
+    split_border = f"{dl}├{'┼'.join(split_border)}┤{dr}"
 
     lines = [title_line, top_border, header_line, split_border]
     lines.extend([body_line] * len(body))
     lines.append(bottom_border)
     lines.append(note_line)
     table_template = '\n'.join(lines)
 
@@ -385,25 +479,84 @@
     all_data.append(note)
 
     table_string = table_template.format(*all_data)
 
     print('\n', table_string, '\n', sep='')
 
 
-if __name__ == '__main__':
-    # Compare the running time of initialization methods
-    # for several built-in data types
+def main() -> None:
+    """
+Usage:
+  python timeit_compare.py [-s] [-n] [-r] [--sort-by] [--reverse] [-d] [-h] [--] [statements ...]
+
+Options:
+  -s, --setup       default setup for each statement (default 'pass').
+  -n, --number      number of loops per repetition (default: see below).
+  -r, --repeat      number of repetitions (default 5).
+  --sort-by         the basis for sorting the results, which can be 'index', 'mean', 'median', 'min', 'max' or 'std' (default 'mean').
+  --reverse         set to sort the results in descending order (default False).
+  -d, --decimal     number of decimal places reserved for results (default 3).
+  -h, --help        print this usage message and exit.
+  --                separate options from statement, use when statement starts with -.
+  statements        'statement#setup' or a single statement to be compared.
+
+If -n is not given or is less than or equal to 0, it defaults to a value that makes the total running time not too long. You can intentionally set it to a higher value to make the results more accurate.
+    """
+    import sys
+    args = sys.argv[1:]
+
+    import getopt
+    try:
+        opts, args = getopt.getopt(
+            args, 's:n:r:d:h',
+            ['setup=', 'number=', 'repeat=', 'sort-by=', 'reverse',
+             'decimal=', 'help'])
+    except getopt.error as e:
+        error = str(e)
+    else:
+        error = None
+    if error is not None:
+        raise getopt.error(f'{error}\nuse -h/--help for command line help')
+
+    stmts = [a.split('#', 1) for a in args]
+    setup = []
+    globals = None
+    number = 0
+    repeat = 5
+    sort_by = 'mean'
+    reverse = False
+    decimal = 3
+    for k, v in opts:
+        if k in ('-s', '--setup'):
+            setup.append(v)
+        elif k in ('-n', '--number'):
+            number = int(v)
+        elif k in ('-r', '--repeat'):
+            repeat = int(v)
+        elif k == '--sort-by':
+            sort_by = v
+        elif k == '--reverse':
+            reverse = True
+        elif k in ('-d', '--decimal'):
+            decimal = int(v)
+        elif k in ('-h', '--help'):
+            print(main.__doc__)
+            return
+    setup = '\n'.join(setup) if setup else 'pass'
+
+    import os
+    sys.path.insert(0, os.curdir)
+
     compare(
-        bool,
-        bytearray,
-        bytes,
-        complex,
-        dict,
-        float,
-        frozenset,
-        int,
-        list,
-        set,
-        str,
-        tuple,
-        number=1_000_000
+        *stmts,
+        setup=setup,
+        globals=globals,
+        number=number,
+        repeat=repeat,
+        sort_by=sort_by,
+        reverse=reverse,
+        decimal=decimal
     )
+
+
+if __name__ == '__main__':
+    main()
```

