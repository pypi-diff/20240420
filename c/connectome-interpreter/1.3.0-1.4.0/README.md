# Comparing `tmp/connectome_interpreter-1.3.0.tar.gz` & `tmp/connectome_interpreter-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.3.0.tar", last modified: Mon Apr 15 08:32:36 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.4.0.tar", last modified: Sat Apr 20 14:48:55 2024, max compression
```

## Comparing `connectome_interpreter-1.3.0.tar` & `connectome_interpreter-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:36.054204 connectome_interpreter-1.3.0/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      938 2024-04-15 08:32:36.054204 connectome_interpreter-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:36.024979 connectome_interpreter-1.3.0/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.3.0/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.3.0/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    18200 2024-04-10 13:11:37.000000 connectome_interpreter-1.3.0/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16261 2024-04-14 17:16:24.000000 connectome_interpreter-1.3.0/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    26902 2024-04-14 22:22:33.000000 connectome_interpreter-1.3.0/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:36.051269 connectome_interpreter-1.3.0/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0      938 2024-04-15 08:32:35.000000 connectome_interpreter-1.3.0/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-04-15 08:32:35.000000 connectome_interpreter-1.3.0/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:32:35.000000 connectome_interpreter-1.3.0/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-15 08:32:35.000000 connectome_interpreter-1.3.0/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-15 08:32:35.000000 connectome_interpreter-1.3.0/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 08:32:36.055198 connectome_interpreter-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1532 2024-04-15 08:30:37.000000 connectome_interpreter-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:36.052208 connectome_interpreter-1.3.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.3.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:48:55.239209 connectome_interpreter-1.4.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      938 2024-04-20 14:48:55.237943 connectome_interpreter-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 14:48:55.166052 connectome_interpreter-1.4.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.4.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.4.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    18727 2024-04-18 22:37:14.000000 connectome_interpreter-1.4.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16261 2024-04-14 17:16:24.000000 connectome_interpreter-1.4.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    30606 2024-04-20 14:33:04.000000 connectome_interpreter-1.4.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:48:55.234953 connectome_interpreter-1.4.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0      938 2024-04-20 14:48:54.000000 connectome_interpreter-1.4.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-04-20 14:48:55.000000 connectome_interpreter-1.4.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 14:48:54.000000 connectome_interpreter-1.4.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-20 14:48:54.000000 connectome_interpreter-1.4.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-20 14:48:54.000000 connectome_interpreter-1.4.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 14:48:55.239209 connectome_interpreter-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1557 2024-04-20 14:47:52.000000 connectome_interpreter-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:48:55.236946 connectome_interpreter-1.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.4.0/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.3.0/LICENSE` & `connectome_interpreter-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.3.0/PKG-INFO` & `connectome_interpreter-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.3.0
+Version: 1.4.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
```

### Comparing `connectome_interpreter-1.3.0/README.md` & `connectome_interpreter-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.3.0/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.4.0/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.3.0/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.4.0/connectome_interpreter/compress_paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     sum_matrix = matrices[0].copy()
     for i in range(1, n):
         sum_matrix += matrices[i]
 
     return sum_matrix
 
 
-def result_summary(stepsn, inidx, outidx, inidx_map=None, outidx_map=None, display_output=True, sort_by_column=None):
+def result_summary(stepsn, inidx, outidx, inidx_map=None, outidx_map=None, display_output=True, sort_by_column=None, pre_in_column=False, display_threshold=0):
     """
     Generates a summary of connections between different types of neurons, 
     represented by their input and output indexes. The function calculates 
     the total synaptic input from presynaptic neuron groups to an average neuron in each 
     postsynaptic neuron group.
 
     Args:
@@ -222,14 +222,16 @@
         inidx (numpy.ndarray): Array of indices representing the input (presynaptic) neurons, used to subset stepsn. nan values are removed.
         outidx (numpy.ndarray): Array of indices representing the output (postsynaptic) neurons.
         inidx_map (dict, optional): Mapping from indices to neuron groups for the input neurons. Defaults to None, in which case neurons are not grouped. 
         outidx_map (dict, optional): Mapping from indices to neuron groups for the output neurons.
             Defaults to None, in which case it is set to be the same as inidx_map.
         display_output (bool, optional): Whether to display the output in a coloured dataframe. Defaults to True.
         sort_by_column (str or list, optional): the column name(s) to sort the result by. If none is provided, then sort by the first column. 
+        pre_in_column (bool, optional): Whether to have the presynaptic neuron groups as columns. Defaults to False (pre in rows, post in columns).
+        display_threshold (float, optional): The threshold for displaying the output. Defaults to 0.
 
     Returns:
         pd.DataFrame: A dataframe representing the summed synaptic input from presynaptic neuron groups 
             to an average neuron in each postsynaptic neuron group. This dataframe is always returned, regardless of the
             value of display_output.
 
     Displays:
@@ -260,14 +262,21 @@
     summed_df = df.groupby(df.index).sum()
 
     # Average across columns and transpose back
     # averaging across columns of the same type:
     # on average, a neuron of that type receives x% input from a presynaptic type
     result_df = summed_df.T.groupby(level=0).mean().T
 
+    if pre_in_column:
+        result_df = result_df.T
+
+    if display_threshold > 0:
+        # only display rows where any value >= display_threshold
+        result_df = result_df[(result_df >= display_threshold).any(axis=1)]
+
     if sort_by_column is None:
         # sort result_df by the values in the first column, in descending order
         result_df = result_df.sort_values(
             by=result_df.columns[0], ascending=False)
     elif isinstance(sort_by_column, str):
         sort_by_column = [sort_by_column]
```

### Comparing `connectome_interpreter-1.3.0/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.4.0/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.3.0/connectome_interpreter/utils.py` & `connectome_interpreter-1.4.0/connectome_interpreter/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import random
+import warnings
 
 import torch
 import pandas as pd
 import numpy as np
 from scipy.sparse import coo_matrix, csr_matrix, issparse
 import matplotlib.colors as mcl
 import matplotlib.pyplot as plt
@@ -192,58 +193,138 @@
 
     Returns:
       coo_matrix or csr_matrix: The updated sparse matrix, in the same format as the input.
     """
     if not issparse(sparse_matrix):
         raise TypeError("The provided matrix is not a sparse matrix.")
 
-    # Ensure we're working with CSR for efficiency, remember original format
+    # Convert sparse matrix to COO format for direct edge manipulation
     original_format = sparse_matrix.getformat()
-    csr = sparse_matrix.tocsr() if original_format == 'coo' else sparse_matrix
+    if original_format != 'coo':
+        sparse_matrix = sparse_matrix.tocoo()
+
+    # Extract edges as a DataFrame
+    edges = pd.DataFrame(
+        {'input_idx': sparse_matrix.row, 'output_idx': sparse_matrix.col, 'value': sparse_matrix.data})
 
-    updated_cols = set()  # Track columns that are updated or added
     print("Updating matrix...")
     if input_idx is not None and output_idx is not None and value is not None:
-        # Convert inputs to arrays and ensure compatibility
+        # Create updates DataFrame from provided indices and values
         input_idx = to_nparray(input_idx)
         output_idx = to_nparray(output_idx)
-        if np.isscalar(value) or (isinstance(value, np.ndarray) and value.size == 1):
+        if np.isscalar(value):
             value = np.full(len(input_idx) * len(output_idx), value)
-        elif len(value) == len(input_idx) * len(output_idx):
-            value = np.atleast_1d(value)
-        else:
+        elif len(value) != len(input_idx) * len(output_idx):
             raise ValueError(
-                "The length of 'value' is incorrect. It should either be a single value or match the length of 'input_idx' * 'output_idx'.")
+                "Length of 'value' must match the product of the lengths of 'input_idx' and 'output_idx', or be one single value.")
 
-        for (i, j, val) in tqdm(zip(np.repeat(input_idx, len(output_idx)),
-                                    np.tile(output_idx, len(input_idx)),
-                                    value)):
-            # Update the matrix, note the changes in indexing for csr
-            if csr[i, j] != 0:
-                csr[i, j] = val  # Efficient for CSR format
-                updated_cols.add(j)
+        updates_df = pd.DataFrame({
+            'input_idx': np.repeat(input_idx, len(output_idx)),
+            'output_idx': np.tile(output_idx, len(input_idx)),
+            'value': value
+        })
 
     elif updates_df is not None:
-        # Batch updates from a DataFrame
-        for _, row in tqdm(updates_df.iterrows()):
-            i, j, val = row['input_idx'], row['output_idx'], row['value']
-            if csr[i, j] != 0:
-                csr[i, j] = val  # Efficient for CSR format
-                updated_cols.add(j)
+        # check column names
+        if not all(col in updates_df.columns for col in ['input_idx', 'output_idx', 'value']):
+            raise ValueError(
+                "The DataFrame must contain columns ['input_idx', 'output_idx', 'value'].")
+
+    else:
+        raise ValueError(
+            "Either ['input_idx', 'output_idx', and 'value'], or 'updates_df' must be provided.")
 
-    if re_normalize and updated_cols:
+    # Concatenate edges and updates_df, ensuring that updates_df is last so its values take precedence
+    combined_edges = pd.concat([edges, updates_df])
+
+    # Remove duplicates, keeping the last occurrence (from updates_df)
+    # We specify the subset to be the columns 'input_idx' and 'output_idx'
+    edges = combined_edges.drop_duplicates(
+        subset=['input_idx', 'output_idx'], keep='last')
+
+    # Convert back to original sparse matrix format
+    updated_matrix = coo_matrix(
+        (edges['value'], (edges['input_idx'], edges['output_idx'])), shape=sparse_matrix.shape)
+
+    if re_normalize:
         print("Re-normalizing updated columns...")
-        # Normalize updated columns
-        for col in updated_cols:
-            col_sum = csr[:, col].sum()
-            if col_sum != 0:
-                csr[:, col] /= col_sum
-    # remove 0 entries
-    csr.eliminate_zeros()
-    return csr.asformat(original_format)
+        # Convert updated_matrix back to CSR format for efficient column operations
+        updated_matrix = updated_matrix.tocsr()
+
+        # Identify the unique columns to re-normalize based on the updates_df
+        unique_cols = updates_df.reset_index()['output_idx'].unique()
+
+        # Compute sum of each column that has been updated
+        col_sums = np.array(
+            updated_matrix[:, unique_cols].sum(axis=0)).flatten()
+
+        # Avoid division by zero by replacing zeros with one (or any non-zero number to prevent change)
+        # This step ensures no values are divided by zero, maintaining original values in such cases
+        col_sums[col_sums == 0] = 1
+
+        for idx, col in enumerate(unique_cols):
+            updated_matrix[:, col] /= col_sums[idx]
+
+    if issubclass(updated_matrix.dtype.type, np.integer):
+        warnings.warn(
+            "Matrix data is of integer type instead of float32. Is the sparse matrix normalised connectivity?",
+            UserWarning
+        )
+    return updated_matrix.asformat(original_format)
+
+    # if not issparse(sparse_matrix):
+    #     raise TypeError("The provided matrix is not a sparse matrix.")
+
+    # # Ensure we're working with CSR for efficiency, remember original format
+    # original_format = sparse_matrix.getformat()
+    # csr = sparse_matrix.tocsr() if original_format == 'coo' else sparse_matrix
+
+    # updated_cols = set()  # Track columns that are updated or added
+    # print("Updating matrix...")
+    # if input_idx is not None and output_idx is not None and value is not None:
+    #     # Convert inputs to arrays and ensure compatibility
+    #     input_idx = to_nparray(input_idx)
+    #     output_idx = to_nparray(output_idx)
+    #     if np.isscalar(value) or (isinstance(value, np.ndarray) and value.size == 1):
+    #         value = np.full(len(input_idx) * len(output_idx), value)
+    #     elif len(value) == len(input_idx) * len(output_idx):
+    #         value = np.atleast_1d(value)
+    #     else:
+    #         raise ValueError(
+    #             "The length of 'value' is incorrect. It should either be a single value or match the length of 'input_idx' * 'output_idx'.")
+
+    #     for (i, j, val) in tqdm(zip(np.repeat(input_idx, len(output_idx)),
+    #                                 np.tile(output_idx, len(input_idx)),
+    #                                 value)):
+    #         # Update the matrix, note the changes in indexing for csr
+    #         if csr[i, j] != 0:
+    #             csr[i, j] = val  # Efficient for CSR format
+    #             updated_cols.add(j)
+
+    # elif updates_df is not None:
+    #     # Batch updates from a DataFrame
+    #     for _, row in tqdm(updates_df.iterrows()):
+    #         i, j, val = row['input_idx'], row['output_idx'], row['value']
+    #         if csr[i, j] != 0:
+    #             csr[i, j] = val  # Efficient for CSR format
+    #             updated_cols.add(j)
+
+    # else:
+    #     raise ValueError("Either ['input_idx', 'output_idx', and 'value'], or 'updates_df' must be provided.")
+
+    # if re_normalize and updated_cols:
+    #     print("Re-normalizing updated columns...")
+    #     # Normalize updated columns
+    #     for col in updated_cols:
+    #         col_sum = csr[:, col].sum()
+    #         if col_sum != 0:
+    #             csr[:, col] /= col_sum
+    # # remove 0 entries
+    # csr.eliminate_zeros()
+    # return csr.asformat(original_format)
 
 
 def to_nparray(input_data):
     """
     Converts the input data into a numpy array, filtering out any NaN values and duplicates. 
     The input can be a single number, a list, a set, a numpy array, or a pandas Series.
```

### Comparing `connectome_interpreter-1.3.0/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.4.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.3.0
+Version: 1.4.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
```

### Comparing `connectome_interpreter-1.3.0/setup.py` & `connectome_interpreter-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.3.0',
+    version='1.4.0',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
         'torch',
@@ -28,10 +28,11 @@
     description='A tool for connectomics data interpretation',
     keywords=['connectomics', 'neural network',
               'mechanistic interpretability'],
     project_urls={
         'Documentation': 'https://connectome-interpreter.readthedocs.io/en/latest/',
         'Larva connectome example': 'https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing',
         'Adult connectome example (FAFB)': 'https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing',
-    }
-    # url='https://connectome-interpreter.readthedocs.io/en/latest/',  # Project home page
+    },
+    # url='https://connectome-interpreter.readthedocs.io/en/latest/',
+    test_suite='tests'  # Project home page
 )
```

