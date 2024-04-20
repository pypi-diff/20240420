# Comparing `tmp/trm_woodburn-0.0.9.tar.gz` & `tmp/trm_woodburn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.9.tar", last modified: Tue Apr 16 04:09:40 2024, max compression
+gzip compressed data, was "trm_woodburn-0.1.0.tar", last modified: Sat Apr 20 01:05:26 2024, max compression
```

## Comparing `trm_woodburn-0.0.9.tar` & `trm_woodburn-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.066722 trm_woodburn-0.0.9/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.9/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 04:09:40.066673 trm_woodburn-0.0.9/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5975 2024-04-16 03:26:34.000000 trm_woodburn-0.0.9/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.9/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-16 04:09:40.066938 trm_woodburn-0.0.9/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.065062 trm_woodburn-0.0.9/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.065747 trm_woodburn-0.0.9/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.9/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    20770 2024-04-16 04:09:06.000000 trm_woodburn-0.0.9/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 04:09:40.066492 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6454 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-16 04:09:40.000000 trm_woodburn-0.0.9/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 01:05:26.771224 trm_woodburn-0.1.0/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.1.0/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-20 01:05:26.771173 trm_woodburn-0.1.0/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6392 2024-04-20 01:04:40.000000 trm_woodburn-0.1.0/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.1.0/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-20 01:05:26.771449 trm_woodburn-0.1.0/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 01:05:26.769370 trm_woodburn-0.1.0/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 01:05:26.770212 trm_woodburn-0.1.0/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.1.0/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    23937 2024-04-20 01:00:22.000000 trm_woodburn-0.1.0/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 01:05:26.770980 trm_woodburn-0.1.0/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-20 01:05:26.000000 trm_woodburn-0.1.0/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-20 01:05:26.000000 trm_woodburn-0.1.0/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-20 01:05:26.000000 trm_woodburn-0.1.0/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-20 01:05:26.000000 trm_woodburn-0.1.0/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-20 01:05:26.000000 trm_woodburn-0.1.0/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.9/LICENSE.txt` & `trm_woodburn-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.9/PKG-INFO` & `trm_woodburn-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.9
+Version: 0.1.0
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,16 +29,16 @@
     another window.
 -   The entire python program and the terminal is locked up after any
     `plt.show()` command until you close all figure windows.
 -   Unless you save the figures to individual files, there is no buffer to show
     plots from past runs.
 
 These are all excuses to use this library. But, the biggest reason to use this
-library is that the terminal is cool, and the more you can do you work in the
-terminal the better.
+library is that the terminal is cool, and the more you can do your work in the
+terminal the better!
 
 ## Plots
 
 ```python
 trm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
 ```
 
@@ -67,41 +67,44 @@
 The `rows` and `cols` parameters let you specify the number of terminal text
 rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
 to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
-default to `20` rows and `60` columns.
+default to `20` rows and `60` columns. These defaults can be redefined by
+changing `trm.config.rows` and `trm.config.cols`.
 
 By default, this library will use Unicode symbols (specifically braille) for
-plotting. A good font to use for this is JuliaMono. However, if your font does
-not support the necessary Unicode symbols, you can tell the library to not use
-them by setting `trm.config.uni` to `False` before calling the `trm.plot`
-function.
+plotting. A good font to use is JuliaMono. However, if your font does not
+support the necessary Unicode symbols, you can tell the library to not use them
+by setting `trm.config.uni` to `False` before calling the `trm.plot` function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
-plotted, color will be used. The color map is blue, green, yellow, red, and
+plotted, color will be used. The color map is blue, green, yellow, orange, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
-would you do that?), then the colors will recyle.
+would you do that?), then the colors will recycle.
 
 If you want equal axis scaling, set `equal` to `1`. However, since terminal
-fonts are not always the same aspect ratio, you can adjust this value to tune.
+fonts are not always the same aspect ratio and because the line spacing in your
+terminal might be adjustable, you can adjust this value to tune.
 
 ## Bars
 
 ```python
-trm.bars(x, labels=None, width=COLS, show_zero=True)
+trm.bars(x, labels=None, cols=1, fat=False)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
 values. The `labels` input is a list of strings corresponding to the labels to
-print before the bar of each value in `x`. The `width` input is the total width
-of characters including the labels.
+print before the bar of each value in `x`. If the `cols` input is greater than
+1, it is the total width of characters including the labels. If it is less than
+or equal to 1, it is the portion of the terminal window width which will be used
+for the graph. If the `fat` input is set to `True`, the bars will be thick.
 
 ```
  apples |=========                                         |
 oranges |=========================================         |
 bananas |==================================================|
   pears |====================                              |
  grapes |============================                      |
@@ -147,24 +150,25 @@
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
 ## Progress bars
 
 ```python
-trm.progress(k, K, tic=None, width=None)
+trm.progress(k, K, t_init=None, cols=1, fat=False)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
 seem to be extremely over-complicated. TQDM, for example, includes over 20
 source files. This library's implementation of a progress bar is a single,
 one-page function. The `k` input is the counter of whatever for loop the
 progress bar is reporting on. The `K` input is one greater than the largest
-possible value of `k`, as in `for k in range(K):`. If `tic` is provided, the
+possible value of `k`, as in `for k in range(K):`. If `t_init` is provided, the
 estimated time remaining to complete the process based on the initial time
-stored in `tic` will be displayed. When the process is completed, the total
-elapsed time since `tic` will be displayed. If `width` is not provided, the full
-width of the current terminal window will be used.
+stored in `t_init` will be displayed. When the process is completed, the total
+elapsed time since `t_init` will be displayed. If `cols` is not provided, the
+full width of the current terminal window will be used. If the `fat` input is
+set to `True`, the bars will be thick.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
```

### Comparing `trm_woodburn-0.0.9/README.md` & `trm_woodburn-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     another window.
 -   The entire python program and the terminal is locked up after any
     `plt.show()` command until you close all figure windows.
 -   Unless you save the figures to individual files, there is no buffer to show
     plots from past runs.
 
 These are all excuses to use this library. But, the biggest reason to use this
-library is that the terminal is cool, and the more you can do you work in the
-terminal the better.
+library is that the terminal is cool, and the more you can do your work in the
+terminal the better!
 
 ## Plots
 
 ```python
 trm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
 ```
 
@@ -52,41 +52,44 @@
 The `rows` and `cols` parameters let you specify the number of terminal text
 rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
 to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
-default to `20` rows and `60` columns.
+default to `20` rows and `60` columns. These defaults can be redefined by
+changing `trm.config.rows` and `trm.config.cols`.
 
 By default, this library will use Unicode symbols (specifically braille) for
-plotting. A good font to use for this is JuliaMono. However, if your font does
-not support the necessary Unicode symbols, you can tell the library to not use
-them by setting `trm.config.uni` to `False` before calling the `trm.plot`
-function.
+plotting. A good font to use is JuliaMono. However, if your font does not
+support the necessary Unicode symbols, you can tell the library to not use them
+by setting `trm.config.uni` to `False` before calling the `trm.plot` function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
-plotted, color will be used. The color map is blue, green, yellow, red, and
+plotted, color will be used. The color map is blue, green, yellow, orange, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
-would you do that?), then the colors will recyle.
+would you do that?), then the colors will recycle.
 
 If you want equal axis scaling, set `equal` to `1`. However, since terminal
-fonts are not always the same aspect ratio, you can adjust this value to tune.
+fonts are not always the same aspect ratio and because the line spacing in your
+terminal might be adjustable, you can adjust this value to tune.
 
 ## Bars
 
 ```python
-trm.bars(x, labels=None, width=COLS, show_zero=True)
+trm.bars(x, labels=None, cols=1, fat=False)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
 values. The `labels` input is a list of strings corresponding to the labels to
-print before the bar of each value in `x`. The `width` input is the total width
-of characters including the labels.
+print before the bar of each value in `x`. If the `cols` input is greater than
+1, it is the total width of characters including the labels. If it is less than
+or equal to 1, it is the portion of the terminal window width which will be used
+for the graph. If the `fat` input is set to `True`, the bars will be thick.
 
 ```
  apples |=========                                         |
 oranges |=========================================         |
 bananas |==================================================|
   pears |====================                              |
  grapes |============================                      |
@@ -132,24 +135,25 @@
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
 ## Progress bars
 
 ```python
-trm.progress(k, K, tic=None, width=None)
+trm.progress(k, K, t_init=None, cols=1, fat=False)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
 seem to be extremely over-complicated. TQDM, for example, includes over 20
 source files. This library's implementation of a progress bar is a single,
 one-page function. The `k` input is the counter of whatever for loop the
 progress bar is reporting on. The `K` input is one greater than the largest
-possible value of `k`, as in `for k in range(K):`. If `tic` is provided, the
+possible value of `k`, as in `for k in range(K):`. If `t_init` is provided, the
 estimated time remaining to complete the process based on the initial time
-stored in `tic` will be displayed. When the process is completed, the total
-elapsed time since `tic` will be displayed. If `width` is not provided, the full
-width of the current terminal window will be used.
+stored in `t_init` will be displayed. When the process is completed, the total
+elapsed time since `t_init` will be displayed. If `cols` is not provided, the
+full width of the current terminal window will be used. If the `fat` input is
+set to `True`, the bars will be thick.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
```

### Comparing `trm_woodburn-0.0.9/setup.cfg` & `trm_woodburn-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.9
+version = 0.1.0
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.9/src/trm/trm.py` & `trm_woodburn-0.1.0/src/trm/trm.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,32 +17,40 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2024-04-15"
+__date__ = "2024-04-19"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import os
+import sys
 import time
 import math
 import numpy as np
 
 
 class config:
-    uni = True # flag to use unicode characters
+    uni = True # flag to use Unicode characters
     cols = 60 # default column width
     rows = 20 # default row height
     ar = 2.1 # aspect ratio of characters
 
 
+class persistent:
+    t_last = None
+
+# ------------------
+# Plotting functions
+# ------------------
+
 def plot(x, y=None, label='', rows=1, cols=1, equal=0):
     """
     Create a text-based plot of the path defined by (`x`, `y`) using characters.
     If the size of the terminal can be found, that will be used for sizing the
     plot. Otherwise, the default dimensions (config.cols, config.rows) will be
     used. Note that this function does not plot connecting lines, only the
     points specified by the (`x`, `y`) pairs.
@@ -57,31 +65,31 @@
         be an array of indices.
     label : str, default ''
         Text to place at top of the plot, centered in the border.
     rows : int, default 1
         Desired number of rows if greater than 1 or fraction of existing rows if
         less than 1.
     cols : int, default 1
-        Desired number of columns if greater than 1 or fraction of existing
+        Desired number of columns if greater than 1 or fraction of window
         columns if less than 1.
     equal : float, default 0
         Axis scaling, `y` to `x`. A value of 0 leaves the scaling alone. A value
         of 1 would approximate equal axis scaling. However, because the aspect
         ratio of characters in the terminal is not exactly 2 to 1, this value
         can be adjusted to compensate.
     """
 
     # Get the terminal window size.
     try: # Try to get the true size.
         term_cols, term_rows = os.get_terminal_size()
-        use_color = True
+        colorize = True
     except: # If getting terminal size fails, use default values.
         term_cols = config.cols
         term_rows = config.rows
-        use_color = False
+        colorize = False
     term_rows -= 1 # Account for the prompt line.
 
     # Convert a fractional canvas size to columns and rows.
     if cols <= 1:
         cols = max(round(term_cols * cols), 3)
     if rows <= 1:
         rows = max(round(term_rows * rows), 3)
@@ -198,15 +206,15 @@
     # Map locations to a large matrix.
     M = np.zeros((subrows*rows, subcols*cols), dtype=int)
     X = np.round(X_jk).astype(int)
     Y = np.round(Y_jk).astype(int)
     M[Y, X] = 1 # Puts a 1 wherever the curve coordinates are.
 
     # Scale the data to dots.
-    if (J > 1) and (use_color):
+    if (J > 1) and (colorize):
         color_list = [39, 40, 220, 208, 201]
         u = X//subcols
         v = Y//subrows
         F = np.zeros((rows, cols), dtype=int)
         for j in range(J):
             F[v[j], u[j]] = color_list[j % 5]
     else:
@@ -215,150 +223,66 @@
     # Convert the large matrix to a smaller matrix of character values.
     C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
 
     # Draw the plot.
     draw_graph(C, ranges, label, F, row_zero)
 
 
-def draw_graph(C, left=None, right=None, F=None, row_zero=-1):
+def bars(x, labels=None, cols=1, fat=False):
     """
+    Create a bar graph of the data in `x` using the `labels` for each element
+    of `x`.
+
     Parameters
     ----------
-    C : (I, J) int np.ndarray
-        Matrix of character values.
-    left : string, default None
-        String to place on the left of the box.
-    right : string, default None
-        String to place on the right of the box.
-    F : (I, J) int np.ndarray, default None
-        Matrix of foreground 8-bit color values.
+    x : float array like
+        Set of values to plot as a bar graph.
+    labels : string list, default None
+        List of strings. This should be the same length as `x`.
+    cols : int, default 1
+        Desired number of columns if greater than 1 or fraction of window
+        columns if less than 1.
+    fat : bool, default False
+        Use thicker characters for the progress bar.
     """
 
-    # Define the box drawing characters.
-    if config.uni:
-        b = ["\u250C", "\u2500", "\u2510", "\u2502", "\u2502",
-                "\u251C", "\u2524", "\u2514", "\u2518"]
-    else:
-        b = [".", "-", ".", "|", "|", "+", "+", "'", "'"]
-
-    # Replace zeros with spaces.
-    C = np.where(C == 0, 0x20, C)
-
-    # Draw the top edge of the box.
-    rows, cols = C.shape
-    print(f"{b[0]}{b[1]*cols}{b[2]}")
-
-    # Draw the contents and two sides of the box.
-    if F is None:
-        for row in range(rows):
-            string = b[3] if row != row_zero else b[5]
-            string += ''.join(list(map(chr, C[row])))
-            string += b[4] if row != row_zero else b[6]
-            print(string)
-    else:
-        # For each row of the matrix, draw.
-        for row in range(rows):
-            # Get this row of data.
-            F_row = F[row]
-            C_row = C[row]
-
-            # Draw this row.
-            chars = ''.join(list(map(chr, C_row)))
-            string = b[3] if row != row_zero else b[5]
-            f = 0
-            for col in range(cols):
-                if f != F_row[col]:
-                    f = F_row[col]
-                    if f == 0:
-                        string += "\x1b[0m"
-                    else:
-                        string += f"\x1b[38;5;{f}m"
-                string += chars[col]
-            if f != 0:
-                string += "\x1b[0m"
-            string += b[4] if row != row_zero else b[6]
-            print(string)
-
-    # Draw the bottom of the box and the left and right strings.
-    mid_dashes = cols - 2 - len(left) - 2 - len(right) - 2*(right != '')
-    if mid_dashes >= 0:
-        right = f" {right} " if right != '' else ''
-        print(f"{b[7]}{b[1]} {left} {b[1]*mid_dashes}{right}{b[1]}{b[8]}")
-    else:
-        print(f"{b[7]}{b[1]*cols}{b[8]}")
-        print(left + (', ' + right)*(right != ''))
-
-
-def matrix_to_braille(M):
-    # Pad the matrix with zeros.
-    I, J = M.shape
-    II = math.ceil(I/4)*4
-    JJ = math.ceil(J/2)*2
-    MM = np.zeros((II, JJ), dtype=int)
-    MM[:I, :J] = M
-
-    # Convert the matrix of ones and zeros to braille characters.
-    C = (0x2800 + MM[::4, ::2] +   8*MM[::4, 1::2]
-            +  2*MM[1::4, ::2] +  16*MM[1::4, 1::2]
-            +  4*MM[2::4, ::2] +  32*MM[2::4, 1::2]
-            + 64*MM[3::4, ::2] + 128*MM[3::4, 1::2])
-    return C
-
-
-def matrix_to_ascii(M):
-    # Pad the matrix with zeros.
-    I, J = M.shape
-    II = math.ceil(I/3)*3
-    MM = np.zeros((II, J), dtype=int)
-    MM[:I, :J] = M
-
-    # Convert the matrix of ones and zeros to braille characters.
-    glyphs = np.array([ # " `-'.!:|"
-        0x20, 0x60, 0x2D, 0x27, 0x2E, 0x21, 0x3A, 0x7C])
-    C = glyphs[M[::3] + 2*M[1::3] + 4*M[2::3]]
-    return C
-
-
-def matrix_to_stars(M):
-    I, J = M.shape
-    C = 0x20*np.ones((I, 2*J + 1), dtype=int)
-    C[:, 1:-1:2] += 0xA*M
-    return C
+    # Get the terminal window size.
+    try: # Try to get the true size.
+        term_cols, _ = os.get_terminal_size()
+        term_cols -= 1
+        colorize = True
+    except: # If getting terminal size fails, use default values.
+        term_cols = config.cols
+        colorize = False
 
+    # Convert a fractional `cols` to columns.
+    if cols <= 1:
+        cols = max(round(term_cols * cols), 18)
 
-def bars(x, names=None, width=config.cols, show_zero=True):
-    # Get the name space.
-    name_space = 0
-    if names is not None:
-        lens = [len(s) for s in names]
-        name_space = max(lens)
-
-    # Adjust the total width to make room for names.
-    width -= name_space
-    if width < 4:
-        width = 4
-
-    # Get min and max.
-    if show_zero:
-        x_min = 0
-    else:
-        x_min = min(x)
-    x_max = max(x)
+    # Get the width of labels.
+    label_width = 0
+    if labels is not None:
+        label_width = max([len(l) for l in labels])
+
+    # Adjust the total width to make room for labels.
+    width = cols - label_width - 2
+    if width < 1:
+        width = 1
 
     # For each value of x, print the bar.
-    k = (width - 3)/(x_max - x_min)
+    span = max(x) - 0
     for n in range(len(x)):
-        blen = round((x[n] - x_min) * k)
-        bstr = "=" * blen
-        estr = ' ' * (width - 3 - blen)
-        if names is None:
-            print(f" |{bstr}{estr}|")
+        if labels is None:
+            print(" |", end='')
         else:
-            sstr = " " * (name_space - len(names[n]))
-            print(f"{sstr}{names[n]} |{bstr}{estr}|")
+            sstr = " " * (label_width - len(labels[n]))
+            print(f"{sstr}{labels[n]} |", end='')
+        ratio = x[n]/span
+        draw_bar(width*ratio, width, colorize, fat)
+        print("", flush=True)
 
 
 def heat(matrix):
     """
     Create a surface plot using the input `matrix`. The rows are printed in
     reverse order.
     """
@@ -370,25 +294,25 @@
     rows, cols = M.shape
 
     # Print the matrix.
     if config.uni:
         for row in range(0, (rows - rows%2), 2):
             for col in range(cols):
                 print("\x1b[38;5;%dm\x1b[48;5;%dm\u2580" %
-                        (M[row, col], M[row + 1, col]), end="")
-            print("\x1b[39m\x1b[49m")
+                        (M[row, col], M[row + 1, col]), end='', flush=True)
+            print("\x1b[0m", flush=True)
         if rows % 2 == 1:
             for col in range(cols):
-                print("\x1b[38;5;%dm\u2580" % (M[-1, col]), end="")
-            print("\x1b[39m")
+                print("\x1b[38;5;%dm\u2580" % (M[-1, col]), end='', flush=True)
+            print("\x1b[0m", flush=True)
     else:
         for row in range(rows):
             for col in range(cols):
-                print("\x1b[48;5;%dm  " % (M[row, col]), end="")
-            print("\x1b[49m")
+                print("\x1b[48;5;%dm  " % (M[row, col]), end='')
+            print("\x1b[0m")
 
 
 def table(matrix, head=None, left=None, width=10, sep='  '):
     """
     Print a table to the terminal.
 
     Parameters
@@ -423,35 +347,35 @@
         if not is_2d:
             matrix = [matrix]
     elif isinstance(matrix, np.ndarray):
         matrix = matrix.tolist()
         if not isinstance(matrix[0], list):
             matrix = [matrix]
     else:
-        raise Exception('print_table: matrix must be a list!')
+        raise Exception('heat: matrix must be a list!')
 
     # Check the type of head.
     if head is None:
         head = []
     elif isinstance(head, (str, float, int)):
         head = [head]
     elif isinstance(head, np.ndarray):
         head = head.tolist()
     elif not isinstance(head, list):
-        raise Exception('print_table: head must be a list!')
+        raise Exception('heat: head must be a list!')
 
     # Check the type of left.
     if left is None:
         left = []
     elif isinstance(left, (str, float, int)):
         left = [left]
     elif isinstance(left, np.ndarray):
         left = left.tolist()
     elif not isinstance(left, list):
-        raise Exception('print_table: left must be a list!')
+        raise Exception('heat: left must be a list!')
 
     # Check that width is within 3 to 30.
     if width < 6:
         width = 6
     elif width > 30:
         width = 30
 
@@ -471,15 +395,15 @@
             width = -width
             skip_padding = True
         else:
             skip_padding = False
         if width < 6:
             width = 6
 
-        # Make num non-negative by remember the minus.
+        # Make num non-negative but remember the minus.
         if num < 0:
             sw = 1
             s = "-"
             num = -num
             ei = int(np.floor(np.log10(num))) # integer exponent
         elif num > 0:
             sw = 0
@@ -584,68 +508,258 @@
     # Create the shape string.
     shape_str = f"{matrix.shape[0]}x{matrix.shape[1]}"
 
     # Draw the plot.
     draw_graph(C, shape_str, label)
 
 
-def time_str(t_seconds):
-    """ Convert time in seconds to a clock string of the form
-    `HH:MM:SS.S`. """
-    t_seconds = abs(t_seconds)
-    hours = int(t_seconds/3600)
-    minutes = int((t_seconds - hours*3600)//60)
-    seconds = (t_seconds % 60)
-    clock_str = "%02d:%02d:%04.1f" % (hours, minutes, seconds)
-    return clock_str
-
-
-def progress(k, K, tic=None, width=None):
+def progress(k, K, t_init=None, cols=1, fat=False):
     """
     Output a simple progress bar with percent complete to the terminal. When `k`
     equals `K - 1`, the progress bar will complete and start a new line.
 
     Parameters
     ----------
     k : int
         Index which should grow monotonically from 0 to K - 1.
     K : int
         Final index value of `k` plus 1.
-    tic : float, default None
-        Starting time (s). If provided, an estimated time remaining will be
-        displayed. If left as None, no time will be shown. When the progress bar
-        completes, the total duration will be shown.
-    width : int, default None
-        Width of the full string, including the percent complete, the bar, and
-        the clock. If not given, the width of the terminal window will be used.
+    t_init : float, default None
+        Initial process time (s). If provided, an estimated time remaining will
+        be displayed. If left as None, no time will be shown. When the progress
+        bar completes, the total duration will be shown.
+    cols : int, default 1
+        Desired width of the full string, including the percent complete, the
+        bar, and the clock if greater than 1 or fraction of window columns if
+        less than 1.
+    fat : bool, default False
+        Use thicker characters for the progress bar.
     """
 
-    # Default the width to the terminal width or config.cols.
-    if width is None:
-        try: # Try to get the true size.
-            width, _ = os.get_terminal_size()
-        except: # If getting terminal size fails, use default values.
-            width = config.cols
+    # Skip this call if the bar is not done but not enough time has passed.
+    t_now = time.perf_counter()
+    if (k + 1 < K) and (persistent.t_last is not None) and \
+            (t_now - persistent.t_last < 0.1):
+        return
+    persistent.t_last = t_now
+
+    # Get the terminal window size.
+    try: # Try to get the true size.
+        term_cols, _ = os.get_terminal_size()
+        term_cols -= 1
+        colorize = True
+    except: # If getting terminal size fails, use default values.
+        term_cols = config.cols
+        colorize = False
+
+    # Convert a fractional `cols` to columns.
+    if cols <= 1:
+        cols = max(round(term_cols * cols), 18)
 
     # Get the ratio.
-    ratio = (k + 1)/K
+    ratio = (k + 1)/K if k < K - 1 else 1
 
     # Get the clock string.
-    if tic is not None:
-        t_elapsed = time.perf_counter() - tic
+    if t_init is not None:
+        t_diff = t_now - t_init
         if k + 1 == K:
-            clk_str = "  " + time_str(t_elapsed)
+            clk_str = "  " + time_str(t_diff)
         else:
-            t_remaining = t_elapsed*(1.0 - ratio)/ratio
-            clk_str = " -" + time_str(t_remaining)
+            t_left = 0.0 if ratio <= 0 else t_diff*(1 - ratio)/ratio
+            clk_str = " -" + time_str(t_left)
     else:
         clk_str = ""
 
+    # Maximum length of bar
+    N = cols - 5 - len(clk_str)
+
     # Build the progress bar.
-    N = width - 8 - len(clk_str) # maximum length of bar within the brackets
-    if k + 1 == K:
-        print(f"\r100% [{'/'*N}]{clk_str}", flush=True)
-    elif (K < N) or (k % int(K/N) == 0):
-        bar_len = int(N*ratio)
-        print(f"\r{int(100*ratio):3d}% "
-            + f"[{'/'*bar_len}{'-'*(N - bar_len)}]{clk_str}",
-            end="", flush=True)
+    print(f"\r{int(100*ratio):3d}% ", end='')
+    draw_bar(N*ratio, N, colorize, fat)
+    if k + 1 >= K:
+        print(f"{clk_str}", flush=True)
+    else:
+        print(f"{clk_str}", end='', flush=True)
+
+# -----------------
+# Support functions
+# -----------------
+
+def time_str(t_seconds):
+    """ Convert time in seconds to a clock string of the form
+    `HH:MM:SS.S`. """
+    t_seconds = abs(t_seconds)
+    hours = int(t_seconds/3600)
+    minutes = int((t_seconds - hours*3600)//60)
+    seconds = (t_seconds % 60)
+    clock_str = "%02d:%02d:%04.1f" % (hours, minutes, seconds)
+    return clock_str
+
+
+def matrix_to_braille(M):
+    # Pad the matrix with zeros.
+    I, J = M.shape
+    II = math.ceil(I/4)*4
+    JJ = math.ceil(J/2)*2
+    MM = np.zeros((II, JJ), dtype=int)
+    MM[:I, :J] = M
+
+    # Convert the matrix of ones and zeros to braille characters.
+    C = (0x2800 + MM[::4, ::2] +   8*MM[::4, 1::2]
+            +  2*MM[1::4, ::2] +  16*MM[1::4, 1::2]
+            +  4*MM[2::4, ::2] +  32*MM[2::4, 1::2]
+            + 64*MM[3::4, ::2] + 128*MM[3::4, 1::2])
+    return C
+
+
+def matrix_to_ascii(M):
+    # Pad the matrix with zeros.
+    I, J = M.shape
+    II = math.ceil(I/3)*3
+    MM = np.zeros((II, J), dtype=int)
+    MM[:I, :J] = M
+
+    # Convert the matrix of ones and zeros to braille characters.
+    glyphs = np.array([ # " `-'.!:|"
+        0x20, 0x60, 0x2D, 0x27, 0x2E, 0x21, 0x3A, 0x7C])
+    C = glyphs[M[::3] + 2*M[1::3] + 4*M[2::3]]
+    return C
+
+
+def matrix_to_stars(M):
+    I, J = M.shape
+    C = 0x20*np.ones((I, 2*J + 1), dtype=int)
+    C[:, 1:-1:2] += 0xA*M
+    return C
+
+
+def draw_graph(C, left=None, right=None, F=None, row_zero=-1):
+    """
+    Parameters
+    ----------
+    C : (I, J) int np.ndarray
+        Matrix of character values.
+    left : string, default None
+        String to place on the left of the box.
+    right : string, default None
+        String to place on the right of the box.
+    F : (I, J) int np.ndarray, default None
+        Matrix of foreground 8-bit color values.
+    """
+
+    # Define the box drawing characters.
+    if config.uni:
+        b = ["\u250C", "\u2500", "\u2510", "\u2502", "\u2502",
+                "\u251C", "\u2524", "\u2514", "\u2518"]
+    else:
+        b = [".", "-", ".", "|", "|", "+", "+", "'", "'"]
+
+    # Replace zeros with spaces.
+    C = np.where(C == 0, 0x20, C)
+
+    # Draw the top edge of the box.
+    rows, cols = C.shape
+    print(b[0], end='')
+    for col in range(cols):
+        print(b[1], end='', flush=True)
+    print(b[2])
+
+    # Draw the contents and two sides of the box.
+    if F is None:
+        for row in range(rows):
+            if row != row_zero:
+                l = b[3]
+                r = b[4]
+            else:
+                l = b[5]
+                r = b[6]
+            C_row = C[row]
+            print(l, end='', flush=True)
+            for col in range(cols):
+                print(chr(C_row[col]), end='', flush=True)
+            print(r, flush=True)
+    else:
+        # For each row of the matrix, draw.
+        for row in range(rows):
+            if row != row_zero:
+                l = b[3]
+                r = b[4]
+            else:
+                l = b[5]
+                r = b[6]
+
+            # Get this row of data.
+            F_row = F[row]
+            C_row = C[row]
+
+            # Draw this row.
+            print(l, end='', flush=True)
+            f = 0
+            for col in range(cols):
+                if f != F_row[col]:
+                    f = F_row[col]
+                    if f == 0:
+                        print("\x1b[0m", end='')
+                    else:
+                        print(f"\x1b[38;5;{f}m", end='')
+                print(chr(C_row[col]), end='', flush=True)
+            if f != 0:
+                print("\x1b[0m", end='')
+            print(r, flush=True)
+
+    # Draw the bottom of the box and the left and right strings.
+    mid_dashes = cols - 2 - len(left) - 2 - len(right) - 2*(right != '')
+    if mid_dashes >= 0:
+        right = f" {right} " if right != '' else ''
+        print(f"{b[7]}{b[1]} {left} ", end='', flush=True)
+        for col in range(mid_dashes):
+            print(b[1], end='', flush=True)
+        print(f"{right}{b[1]}{b[8]}", flush=True)
+    else:
+        print(f"{b[7]}{b[1]*cols}{b[8]}")
+        print(left + (', ' + right)*(right != ''), flush=True)
+
+
+def draw_bar(n, N, colorize, fat):
+    # Define the left, center, and right characters and color commands.
+    if colorize:
+        grey = '\x1b[100m' if config.uni and fat else '\x1b[90m'
+    else:
+        grey = ''
+    if config.uni:
+        if fat:
+            l = chr(0x2588)
+            frac = int(n*8) % 8 # 0 to 7
+            c = ' ' if frac == 0 else chr(0x2588 + 8 - frac)
+            c = grey + c
+            r = ' '
+        else:
+            l = chr(0x2501)
+            if (n) % 1 < 0.5:
+                c = grey + chr(0x257A) if colorize else ' '
+            else:
+                c = chr(0x2578) + grey
+            r = chr(0x2501) if colorize else ' '
+    else:
+        if fat:
+            l = '/'
+            c = grey + '-' if (n % 1 < 0.5) else '/' + grey
+            r = '-'
+        else:
+            l = '='
+            c = grey + '-' if (n % 1 < 0.5) else '=' + grey
+            r = '-'
+
+    # Build the progress bar.
+    if n >= N:
+        for j in range(N):
+            print(l, end='', flush=True)
+    else:
+        bar_len = int(n)
+        spc_len = N - 1 - bar_len
+        for j in range(bar_len):
+            print(l, end='', flush=True)
+        print(c, end='', flush=True)
+        for j in range(spc_len):
+            print(r, end='', flush=True)
+        if colorize:
+            print('\x1b[0m', end='', flush=True)
```

### Comparing `trm_woodburn-0.0.9/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.1.0/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.9
+Version: 0.1.0
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,16 +29,16 @@
     another window.
 -   The entire python program and the terminal is locked up after any
     `plt.show()` command until you close all figure windows.
 -   Unless you save the figures to individual files, there is no buffer to show
     plots from past runs.
 
 These are all excuses to use this library. But, the biggest reason to use this
-library is that the terminal is cool, and the more you can do you work in the
-terminal the better.
+library is that the terminal is cool, and the more you can do your work in the
+terminal the better!
 
 ## Plots
 
 ```python
 trm.plot(x, y=None, label='', rows=1, cols=1, equal=0)
 ```
 
@@ -67,41 +67,44 @@
 The `rows` and `cols` parameters let you specify the number of terminal text
 rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
 to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
-default to `20` rows and `60` columns.
+default to `20` rows and `60` columns. These defaults can be redefined by
+changing `trm.config.rows` and `trm.config.cols`.
 
 By default, this library will use Unicode symbols (specifically braille) for
-plotting. A good font to use for this is JuliaMono. However, if your font does
-not support the necessary Unicode symbols, you can tell the library to not use
-them by setting `trm.config.uni` to `False` before calling the `trm.plot`
-function.
+plotting. A good font to use is JuliaMono. However, if your font does not
+support the necessary Unicode symbols, you can tell the library to not use them
+by setting `trm.config.uni` to `False` before calling the `trm.plot` function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
-plotted, color will be used. The color map is blue, green, yellow, red, and
+plotted, color will be used. The color map is blue, green, yellow, orange, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
-would you do that?), then the colors will recyle.
+would you do that?), then the colors will recycle.
 
 If you want equal axis scaling, set `equal` to `1`. However, since terminal
-fonts are not always the same aspect ratio, you can adjust this value to tune.
+fonts are not always the same aspect ratio and because the line spacing in your
+terminal might be adjustable, you can adjust this value to tune.
 
 ## Bars
 
 ```python
-trm.bars(x, labels=None, width=COLS, show_zero=True)
+trm.bars(x, labels=None, cols=1, fat=False)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
 values. The `labels` input is a list of strings corresponding to the labels to
-print before the bar of each value in `x`. The `width` input is the total width
-of characters including the labels.
+print before the bar of each value in `x`. If the `cols` input is greater than
+1, it is the total width of characters including the labels. If it is less than
+or equal to 1, it is the portion of the terminal window width which will be used
+for the graph. If the `fat` input is set to `True`, the bars will be thick.
 
 ```
  apples |=========                                         |
 oranges |=========================================         |
 bananas |==================================================|
   pears |====================                              |
  grapes |============================                      |
@@ -147,24 +150,25 @@
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
 ## Progress bars
 
 ```python
-trm.progress(k, K, tic=None, width=None)
+trm.progress(k, K, t_init=None, cols=1, fat=False)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
 seem to be extremely over-complicated. TQDM, for example, includes over 20
 source files. This library's implementation of a progress bar is a single,
 one-page function. The `k` input is the counter of whatever for loop the
 progress bar is reporting on. The `K` input is one greater than the largest
-possible value of `k`, as in `for k in range(K):`. If `tic` is provided, the
+possible value of `k`, as in `for k in range(K):`. If `t_init` is provided, the
 estimated time remaining to complete the process based on the initial time
-stored in `tic` will be displayed. When the process is completed, the total
-elapsed time since `tic` will be displayed. If `width` is not provided, the full
-width of the current terminal window will be used.
+stored in `t_init` will be displayed. When the process is completed, the total
+elapsed time since `t_init` will be displayed. If `cols` is not provided, the
+full width of the current terminal window will be used. If the `fat` input is
+set to `True`, the bars will be thick.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
```

