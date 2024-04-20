# Comparing `tmp/sdeper-1.0.3.tar.gz` & `tmp/sdeper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeper-1.0.3.tar", last modified: Mon Apr  1 03:37:52 2024, max compression
+gzip compressed data, was "sdeper-1.1.0.tar", last modified: Sat Apr 20 13:07:25 2024, max compression
```

## Comparing `sdeper-1.0.3.tar` & `sdeper-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:37:52.203644 sdeper-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 03:37:44.000000 sdeper-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 03:37:44.000000 sdeper-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-01 03:37:52.203644 sdeper-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-01 03:37:44.000000 sdeper-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 03:37:44.000000 sdeper-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-01 03:37:44.000000 sdeper-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 03:37:52.203644 sdeper-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-01 03:37:44.000000 sdeper-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:37:52.199643 sdeper-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17158 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/admm_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36041 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/cvae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/cvaeglrm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26876 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/hyper_parameter_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/imputation.py
--rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/local_fit_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)    19410 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    37191 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/parse_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/run_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:37:52.203644 sdeper-1.0.3/src/sdeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-01 03:37:52.000000 sdeper-1.0.3/src/sdeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-01 03:37:52.000000 sdeper-1.0.3/src/sdeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 03:37:52.000000 sdeper-1.0.3/src/sdeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 03:37:52.000000 sdeper-1.0.3/src/sdeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 03:37:52.000000 sdeper-1.0.3/src/sdeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-01 03:37:52.000000 sdeper-1.0.3/src/sdeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 03:37:44.000000 sdeper-1.0.3/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:25.875962 sdeper-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 13:07:17.000000 sdeper-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 13:07:17.000000 sdeper-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-20 13:07:25.875962 sdeper-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-20 13:07:17.000000 sdeper-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-20 13:07:17.000000 sdeper-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 13:07:17.000000 sdeper-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:07:25.875962 sdeper-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-20 13:07:17.000000 sdeper-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:25.871962 sdeper-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/admm_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37931 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/cvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/cvaeglrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27000 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/hyper_parameter_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/local_fit_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50641 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/parse_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/run_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:25.875962 sdeper-1.1.0/src/sdeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23099 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/version.py
```

### Comparing `sdeper-1.0.3/LICENSE` & `sdeper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdeper-1.0.3/PKG-INFO` & `sdeper-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.0.3
+Version: 1.1.0
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
@@ -18,22 +18,22 @@
 Requires-Dist: scipy==1.8.1
 Requires-Dist: pandas==1.4.3
 Requires-Dist: networkx==2.8.4
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: scikit-learn==1.1.1
 Requires-Dist: numba==0.55.2
 Requires-Dist: openpyxl==3.0.10
-Requires-Dist: tensorflow==2.9.1
+Requires-Dist: tensorflow-cpu==2.9.1
 Requires-Dist: scanpy==1.9.1
 Requires-Dist: scikit-misc==0.1.4
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: umap-learn==0.5.3
 Requires-Dist: distinctipy==1.2.2
-Requires-Dist: reportlab==3.6.12
-Requires-Dist: opencv-python==4.8.0.74
+Requires-Dist: reportlab==4.1.0
+Requires-Dist: opencv-python==4.6.0.66
 
 # SDePER
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
```

### Comparing `sdeper-1.0.3/README.md` & `sdeper-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdeper-1.0.3/setup.py` & `sdeper-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.0.3/src/admm_fit.py` & `sdeper-1.1.0/src/admm_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,24 @@
     """
     perform a whole ADMM iterations once as one fitting procedure in GLRM
     
     Note: the output of the fit result is 3-Dimensional. The dimension transform will be performed outside this function if needed
     
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.
     L : scipy sparse matrix (spots * spots)
         Laplacian matrix
     theta : 3-D numpy array (spots * celltypes * 1)
         initial guess of theta (celltype proportion).
     e_alpha : 1-D numpy array
         initial guess of e_alpha (spot-specific effect).
     gamma_g : 1-D numpy array
@@ -112,19 +113,19 @@
     use_cache : bool, optional
         if True, use the cached dict of calculated negative log-likelihood values.
 
     Returns
     -------
     Dict
         estimated model coefficients, including:
-            theta : celltype proportions (#spots * #celltypes * 1)
-            e_alpha : spot-specific effect (1-D array with length #spot)
-            sigma2 : variance paramter of the lognormal distribution (float)
-            gamma_g : gene-specific platform effect for all genes (1-D array with length #gene)
-            theta_tilde : celltype proportions for Adaptive Lasso (#spots * #celltypes * 1)
+            theta : celltype proportions (#spots * #celltypes * 1)\n
+            e_alpha : spot-specific effect (1-D array with length #spot)\n
+            sigma2 : variance paramter of the lognormal distribution (float)\n
+            gamma_g : gene-specific platform effect for all genes (1-D array with length #gene)\n
+            theta_tilde : celltype proportions for Adaptive Lasso (#spots * #celltypes * 1)\n
             theta_hat : celltype proportions for Graph Laplacian constrain (#spots * #celltypes * 1)
     """
     
     n_celltype = data['X'].shape[0]
     n_spot = data['Y'].shape[0]
     one_theta_shape = (n_celltype, 1)
```

### Comparing `sdeper-1.0.3/src/config.py` & `sdeper-1.1.0/src/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 theta_eps = 1e-8
 sigma2_eps = 1e-8
 
 
 
 """
 configuration for reproducible results in keras + TensorFlow
-skipped here, we configure the environment later
+skipped here, we configure the environment in main function
 """
 # Seed value
 #seed_value = 1154
 
 # 1. Set 'PYTHONHASHSEED' environment variable at a fixed value (it must be set before Python running)
 #import os
 #os.environ['PYTHONHASHSEED'] = str(seed_value)
```

### Comparing `sdeper-1.0.3/src/cvae.py` & `sdeper-1.1.0/src/cvae.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 # dealing with the keras symbolic tensor error
 from tensorflow.python.framework.ops import disable_eager_execution
 disable_eager_execution()
 
 
 
-def build_CVAE(spatial_df, scRNA_df, scRNA_celltype, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, diagnosis, rerun_DE=True):
+def build_CVAE(spatial_df, scRNA_df, scRNA_celltype, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, rerun_DE=True, filter_gene=True):
     '''
     build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
     
     input gene expression in datasets only included genes needed for downstream analysis and already been normalized by sequencing depth
 
     Parameters
     ----------
@@ -57,18 +57,33 @@
         maximum value of cells in pseudo-spot
     seq_depth_scaler : int
         a scaler of scRNA-seq sequencing depth
     cvae_input_scaler : int
         maximum value of the scaled input for CVAE
     cvae_init_lr : float
         initial learning rate for training CVAE
+    use_fdr : bool
+        whether to use FDR adjusted p value for filtering and sorting
+    p_val_cutoff : float
+        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering
+    fc_cutoff : float
+        threshold of fold change (without log transform!) in marker genes filtering
+    pct1_cutoff : float
+        threshold of pct.1 in marker genes filtering
+    pct2_cutoff : float
+        threshold of pct.2 in marker genes filtering
+    sortby_fc : bool
+        whether to sort marker genes by fold change
     diagnosis : bool
         if True save more information to files for diagnosis CVAE and hyper-parameter selection
     rerun_DE : bool, optional
         whether to rerun DE on the CVAE transformed scRNA-seq data, since the DE genes might be different with before CVAE transforming.
+    filter_gene : bool
+        whether to filter genes before DE.
+    
 
     Returns
     -------
     spatial_transformed_df : dataframe
         CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes)
     scRNA_decode_df : dataframe
         CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes)
@@ -291,14 +306,15 @@
     
     
     # early stopping based on validation loss
     early_stop = EarlyStopping(monitor='val_loss', min_delta=0, patience=50, restore_best_weights=True, verbose=False)
     
     
     # change tensorflow seed value, set the same seed value for sampling samples from latent space to decoder before training
+    # still has unknown randomness source even set seed here...
     set_random_seed(1154)
     
     # Train CVAE
     print('\nStart training...\n')
     history_callback = cvae.fit([data, labels], data,
                                 validation_data=([valid_data, valid_labels], valid_data),
                                 epochs=1000,
@@ -312,15 +328,15 @@
     
     if n_epoch < 1000:
         print(f'\ntraining finished in {n_epoch} epochs (early stop), transform data to adjust the platform effect...\n')
     else:
         print(f'\ntraining finished in {n_epoch} epochs (reach max pre-specified epoches), transform data to adjust the platform effect...\n')
 
     
-    # proprecess the trained models
+    # postprocess the trained models
     # Subset the encoder
     encoder = Model([cvae.get_layer('encoder_input').input, cvae.get_layer('cond_input').input],
                     [cvae.get_layer('z_mean').output, cvae.get_layer('z_log_var').output],
                     name='encoder')
     
     # Subset the decoder (build another new decoder and re-store weights)
     def build_new_decoder(p, p_cond, latent_dim):
@@ -365,15 +381,15 @@
                                    columns=scRNA_df.columns,
                                    index=scRNA_df.index)
     
     # whether to rerun DE
     if rerun_DE:
         print('\nre-run DE on CVAE transformed scRNA-seq data!')
         from utils import rerun_DE
-        new_markers = rerun_DE(scRNA_decode_df, scRNA_celltype, n_marker_per_cmp, diagnosis)
+        new_markers = rerun_DE(scRNA_decode_df, scRNA_celltype, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_gene)
     else:
         new_markers = None
     
     # take average for all genes
     scRNA_decode_df['celltype'] = scRNA_celltype.celltype
     scRNA_decode_df = scRNA_decode_df.groupby(['celltype']).mean()
     
@@ -569,15 +585,15 @@
     
     #print(f'before CVAE building function return RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
     
     return spatial_transformed_df, scRNA_decode_df, new_markers
 
 
 
-def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, diagnosis):
+def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene):
     '''
     read related CSV files, build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
@@ -599,34 +615,50 @@
         a scaler of scRNA-seq sequencing depth
     cvae_input_scaler : int
         maximum value of the scaled input for CVAE
     cvae_init_lr : float
         initial learning rate for training CVAE
     redo_de : bool
         whether to redo DE after CVAE transformation
+    use_fdr : bool
+        whether to use FDR adjusted p value for filtering and sorting
+    p_val_cutoff : float
+        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering
+    fc_cutoff : float
+        threshold of fold change (without log transform!) in marker genes filtering
+    pct1_cutoff : float
+        threshold of pct.1 in marker genes filtering
+    pct2_cutoff : float
+        threshold of pct.2 in marker genes filtering
+    sortby_fc : bool
+        whether to sort marker genes by fold change
     diagnosis : bool
         if True save more information to files for diagnosis CVAE and hyper-parameter selection
+    filter_cell : bool
+        whether to filter cells before DE
+    filter_gene : bool
+        whether to filter genes before DE
 
     Returns
     -------
     spatial_transformed_df : dataframe
         CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes)
     scRNA_decode_df : dataframe
         CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes)
     new_markers : list or None
         marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE.
     '''
     
     start_time = time()
     
     # read spatial data
-    spatial_spot_obj = read_spatial_data(spatial_file)
+    spatial_spot_obj = read_spatial_data(spatial_file, filter_gene)
     
     # read scRNA-seq data
-    scrna_obj = read_scRNA_data(ref_file, ref_anno_file)
+    scrna_obj = read_scRNA_data(ref_file, ref_anno_file, filter_cell, filter_gene)
     
     # Overlap of genes between scRNA cell-level and spatial spot-level data
     overlap_genes = list(set(spatial_spot_obj.var_names).intersection(set(scrna_obj.var_names)))
     print(f'total {len(overlap_genes)} overlapped genes')
     # if len(overlap_genes) < spatial_spot_obj.n_vars:
     #     print(f'{spatial_spot_obj.n_vars-len(overlap_genes)} genes in spatial data but not found in scRNA-seq data: {", ".join(set(spatial_spot_obj.var_names).difference(set(overlap_genes)))}\n')
     
@@ -668,15 +700,15 @@
             print(f'from user specified marker gene expression use {len(marker_genes)} marker genes overlapped with spatial + scRNA-seq data')
             # if len(marker_genes) < len(overlap_genes):
             #     print(f'{len(overlap_genes)-len(marker_genes)} genes in overlapped gene list between spatial and scRNA-seq data but not found in user provided marker gene expression: {", ".join(set(overlap_genes).difference(set(marker_genes)))}\n')
             
         else:
             # perform DE, return the marker gene expression
             print('no marker gene profile provided. Perform DE to get cell-type marker genes on scRNA-seq data...\n')
-            marker_genes = run_DE(scrna_obj, n_marker_per_cmp, diagnosis, 'DE celltype markers.csv')
+            marker_genes = run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, 'DE celltype markers.csv')
         
         # final gene list for downstream analysis
         final_gene_list = sorted(list(set(scrna_hv_genes).union(set(marker_genes))))
         print(f'\nuse union of highly variable gene list and cell-type marker gene list derived from scRNA-seq data, finally get {len(final_gene_list)} genes for downstream analysis')
     
     
     print('\nstart CVAE building...\n')
@@ -684,12 +716,14 @@
     scrna_celltype['celltype'] = scrna_celltype['celltype'].astype(str)
     
     # build CVAE
     spatial_df, scrna_avg_df, new_markers = build_CVAE(sc.get.obs_df(spatial_spot_obj, keys=final_gene_list),
                                           sc.get.obs_df(scrna_obj, keys=final_gene_list),
                                           scrna_celltype,
                                           n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler,
-                                          cvae_input_scaler, cvae_init_lr, diagnosis, rerun_DE=redo_de)
+                                          cvae_input_scaler, cvae_init_lr,
+                                          use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc,
+                                          diagnosis, rerun_DE=redo_de, filter_gene=filter_gene)
     
     print(f'\nplatform effect adjustment by CVAE finished. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n\n')
     
     return spatial_df, scrna_avg_df, new_markers
```

### Comparing `sdeper-1.0.3/src/cvaeglrm.py` & `sdeper-1.1.0/src/cvaeglrm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue May 10 03:15:36 2022
 
 @author: hill103
 
-this script is the main function of the whole GLRM pipeline
+this script is the main function of the whole CVAE-GLRM pipeline
 
 pipeline steps:
     
-    1. receive and parse the command line parameters and then pass the parameters to GLRM model
-    2. pre-process (include building CVAE)
-    3. model fitting
-    4. post-process and save the results
+    1. receive and parse the command line parameters and then pass the parameters to CVAE-GLRM model
+    2. pre-process
+    3. building CVAE (if available)
+    4. GLRM model fitting
+    5. post-process and save the results
 """
 
 
 
 def main():
+    '''
+    main function
+    
+    Parameters
+    ----------
+    None.
+
+    Returns
+    -------
+    None.
+
+    '''
 
     from config import print, cur_version, output_path
     import os
     os.environ['PYTHONHASHSEED'] = '0'
     os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
     import warnings
     warnings.filterwarnings("ignore")
@@ -48,15 +61,15 @@
     tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
     session_conf = tf.compat.v1.ConfigProto(intra_op_parallelism_threads=paramdict['n_cores'], inter_op_parallelism_threads=paramdict['n_cores'])
     sess = tf.compat.v1.Session(graph=tf.compat.v1.get_default_graph(), config=session_conf)
     tf.compat.v1.keras.backend.set_session(sess)
     
     
     print('\n\n######### Preprocessing... #########\n')
-    data = preprocess(paramdict['spatial_file'], paramdict['ref_file'], paramdict['ref_celltype_file'], paramdict['marker_file'], paramdict['A_file'], paramdict['use_cvae'], paramdict['n_hv_gene'], paramdict['n_marker_per_cmp'], paramdict['pseudo_spot_min_cell'], paramdict['pseudo_spot_max_cell'], paramdict['seq_depth_scaler'], paramdict['cvae_input_scaler'], paramdict['cvae_init_lr'], paramdict['redo_de'], paramdict['diagnosis'])
+    data = preprocess(paramdict['spatial_file'], paramdict['ref_file'], paramdict['ref_celltype_file'], paramdict['marker_file'], paramdict['A_file'], paramdict['use_cvae'], paramdict['n_hv_gene'], paramdict['n_marker_per_cmp'], paramdict['pseudo_spot_min_cell'], paramdict['pseudo_spot_max_cell'], paramdict['seq_depth_scaler'], paramdict['cvae_input_scaler'], paramdict['cvae_init_lr'], paramdict['redo_de'], paramdict['use_fdr'], paramdict['p_val_cutoff'], paramdict['fc_cutoff'], paramdict['pct1_cutoff'], paramdict['pct2_cutoff'], paramdict['sortby_fc'], paramdict['filter_cell'], paramdict['filter_gene'], paramdict['diagnosis'])
     
     
     # whether to estimate gamma_g, if CVAE is used then disable gamma_g estimation
     if paramdict['use_cvae']:
         estimate_gamma_g = False
     else:
         estimate_gamma_g = True
```

### Comparing `sdeper-1.0.3/src/hyper_parameter_optimization.py` & `sdeper-1.1.0/src/hyper_parameter_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,23 +127,24 @@
 
 def cv_find_lambda_r(data, mle_theta, mle_e_alpha, gamma_g, sigma2, lasso_weight, candidate_list, hybrid_version=True, opt_method='L-BFGS-B', hv_x=None, hv_log_p=None, use_admm=False, use_likelihood=True, k=5, use_cache=True, diagnosis=False):
     '''
     find optimal value for hyper-parameter lambda_r by k fold cross-validation
     
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.\n
     mle_theta : 3-D numpy array (spots * celltypes * 1)
         estimated theta (celltype proportion) by MLE.
     mle_e_alpha : 1-D numpy array
         estimated e_alpha (spot-specific effect) by MLE.
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     sigma2 : float
@@ -336,23 +337,24 @@
     
 def cv_find_lambda_g(data, G, theta_mask, gamma_g, sigma2, candidate_list, hybrid_version=True, opt_method='L-BFGS-B', hv_x=None, hv_log_p=None, use_admm=True, use_likelihood=True, k=5, use_cache=True, diagnosis=False):
     '''
     find optimal value for hyper-parameter lambda_g by k fold cross-validation
     
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.\n
     theta_mask : 3-D numpy array (spots * celltypes * 1)
         mask for cell-type proportions (1: present, 0: not present). Only used for stage 2 theta optmization.
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     sigma2 : float
         variance paramter of the lognormal distribution of ln(lambda). All gene share the same variance.
     candidate_list : list
```

### Comparing `sdeper-1.0.3/src/imputation.py` & `sdeper-1.1.0/src/imputation.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.0.3/src/local_fit_numba.py` & `sdeper-1.1.0/src/local_fit_numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,57 @@
 import math
 from config import min_val, min_theta, min_sigma2, N_z, gamma, print, mu_digits, sigma2_digits, theta_eps, sigma2_eps
 
 
 
 ################################# code related to global optimization #################################
 class RandomDisplacementBounds(object):
-    """
-    A custom step-function (https://stackoverflow.com/questions/47055970/how-can-i-write-bounds-of-parameters-by-using-basinhopping)
-    random displacement with bounds:  see: https://stackoverflow.com/a/21967888/2320035
-        Modified! (dropped acceptance-rejection sampling for a more specialized approach)
+    """A class to perform random displacement with bounds on parameters during optimization.
+
+    This step function is designed to modify the basinhopping algorithm's step-taking behavior by 
+    ensuring that new positions remain within specified bounds. This implementation uses a direct 
+    calculation to determine the minimum and maximum allowable steps rather than using
+    acceptance-rejection sampling, which can be found in the more general approach discussed on 
+    StackOverflow (https://stackoverflow.com/a/21967888/2320035). The approach has been modified 
+    for enhanced performance with specific bounds.
+    
+    ref: https://stackoverflow.com/questions/47055970/how-can-i-write-bounds-of-parameters-by-using-basinhopping
+
+    Attributes:
+        xmin (np.ndarray or list): The lower bounds of the parameters. None indicates unbounded.
+        xmax (np.ndarray or list): The upper bounds of the parameters. None indicates unbounded.
+        stepsize (float): The maximum step size to take in any parameter direction.
+
     """
     def __init__(self, xmin, xmax, stepsize=0.5):
+        """
+        Initializes the RandomDisplacementBounds with specified bounds and step size.
+
+        Args:
+            xmin (np.ndarray or list): The lower bounds of the parameters.
+            xmax (np.ndarray or list): The upper bounds of the parameters.
+            stepsize (float, optional): The maximum step size to take in any parameter direction. Defaults to 0.5.
+        """
         self.xmin = xmin
         self.xmax = xmax
         self.stepsize = stepsize
 
     def __call__(self, x):
-        """take a random step but ensure the new position is within the bounds """
+        """
+        Calculates a new position for the optimization algorithm by taking a random step
+        within the defined bounds.
+
+        This method ensures that the new position does not violate the specified bounds.
+
+        Args:
+            x (np.ndarray): The current position of the parameters in the optimization algorithm.
+
+        Returns:
+            np.ndarray: The new position after taking a random step within the bounds.
+        """
         # define a custom function to consider None in bound
         def calcMinStep(xmin, x, stepsize):
             if xmin is None:
                 return -stepsize
             else:
                 return np.maximum(xmin - x, -stepsize)
             
@@ -343,16 +374,20 @@
 
 def hv_comb(w_vec, y_vec, mu, gamma_g, sigma2, hv_x, hv_log_p, N, use_cache):
     '''
     a function to calculate the negative likelihood value given the distribution parameters considering heavy-tail plus corresponding gradient vector
     
     this function will be used as target function for optimization
     
-    we assume y ~ Poisson(N*lambda)
-              ln(lambda) follow epsilon's distribution ~ N(mu, sigma2)
+    we assume:
+        
+        y ~ Poisson(N*lambda)
+
+        ln(lambda) follow epsilon's distribution ~ N(mu, sigma2)
+        
     then ln(N*lambda) ~ N(mu+ln(N), sigma2)
     
     N is sequencing depth for this spot
     mu is alpha + log(theta*marker gene) + gamma
     
     Now we also consider the heavy-tail instead of just normal distribution
     
@@ -522,16 +557,20 @@
 
 def hv_wrapper(w_vec, y_vec, mu, gamma_g, sigma2, hv_x, hv_log_p, N, use_cache):
     '''
     a wrapper to calculate the negative log-likelihood value given the distribution parameters considering heavy-tail
     
     this wrapper will be used as target function for optimization
     
-    we assume y ~ Poisson(N*lambda)
-              ln(lambda) follow epsilon's distribution ~ N(mu, sigma2)
+    we assume:
+        
+        y ~ Poisson(N*lambda)
+    
+        ln(lambda) follow epsilon's distribution ~ N(mu, sigma2)
+    
     then ln(N*lambda) ~ N(mu+ln(N), sigma2)
     
     N is sequencing depth for this spot
     mu is alpha + log(theta*marker gene) + gamma
     
     Now we also consider the heavy-tail instead of just normal distribution
     
@@ -581,26 +620,27 @@
     
     the loss function contains three parts (defined for each spot separately)
     
     1. negative log-likelihood of the base model given observed data and initial parameter value. It sums across all genes
     
     2. a loss of ADMM to make theta equals theta_hat (used for regularization/penalty; optional, controlled by nu_vec and rho)
                     
-                        1/(2*rho) (||w/sum(w) - theta_hat + u||_2)^2
-                        u is the scaled dual variables to make theta = theta_hat    
-                        and nu = theta_hat - u
+        1/(2*rho) (||w/sum(w) - theta_hat + u||_2)^2
+    
+    u is the scaled dual variables to make theta = theta_hat and nu = theta_hat - u
+    
     and we did re-parametrization w = e^alpha * theta, so theta = w / sum(w)
     
     3. a loss of Adaptive Lasso to shrink theta (optional, controlled by lambda_r and lasso_weight_vec)
     
-                        lambda_r * (inner product(w/sum(w), lasso_weight))
+        lambda_r * (inner product(w/sum(w), lasso_weight))
                         
     4. a loss of L2 penalty to shrink theta (optional, controlled by lambda_l2)
     
-                        lambda_l2 * (sum(squared(w/sum(w))))
+        lambda_l2 * (sum(squared(w/sum(w))))
     
     Parameters
     ----------
     w_vec : 1-D numpy array
         e_alpha (spot-specific effect) * theta (celltype proportion) of one spot.
     y_vec : 1-D numpy array
         observed gene counts of one spot.
@@ -718,42 +758,47 @@
 
 
 
 def update_theta(data, warm_start_theta, warm_start_e_alpha, gamma_g, sigma2, nu=None, rho=None, lambda_r=None, lasso_weight=None, lambda_l2=None, global_optimize=False, hybrid_version=True, opt_method='L-BFGS-B', hv_x=None, hv_log_p=None, theta_mask=None, verbose=False, use_cache=True):
     '''
     update theta (celltype proportion) and e_alpha (spot-specific effect) given sigma2 (variance paramter of the log-normal distribution) and gamma_g (gene-specific platform effect) by MLE
     
-    we assume ln(lambda) = alpha + gamma_g + ln(sum(theta*mu_X)) + epsilon
-              subject to sum(theta)=1, theta>=0
+    we assume 
+    
+        ln(lambda) = alpha + gamma_g + ln(sum(theta*mu_X)) + epsilon
+    
+        subject to sum(theta)=1, theta>=0
     
     mu_X is marker genes from data['X']
     
     then the mean parameter of the lognormal distribution of ln(lambda) is alpha + gamma_g + ln(sum(theta*mu_X))
     
     we did re-parametrization w = e^alpha * theta, then
     
-              ln(lambda) = gamma_g + ln(sum([e^alpha*theta]*mu_X)) + epsilon
-              subject to w>=0, it will imply sum(theta)=1 and theta>=0
+        ln(lambda) = gamma_g + ln(sum([e^alpha*theta]*mu_X)) + epsilon
+    
+        subject to w>=0, it will imply sum(theta)=1 and theta>=0
     
     the steps to update theta and e_alpha:
         1. dimension change of theta, theta_hat, u from 3-D (spots * celltypes * 1) to 1-D (celltypes), and do re-parametrization to get w
         2. solve w for each spot in parallel
         3. extract updated theta and e_alpha from w, and change the dimension of updated theta, theta_hat, u back
 
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.
     warm_start_theta : 3-D numpy array (spots * celltypes * 1)
         initial guess of theta (celltype proportion).
     warm_start_e_alpha : 1-D numpy array
         initial guess of e_alpha (spot-specific effect).
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     sigma2 : float
@@ -932,39 +977,44 @@
 
 ################################# code related to update sigma2 #################################
 
 def update_sigma2(data, theta, e_alpha, gamma_g, sigma2, opt_method='L-BFGS-B', global_optimize=False, hv_x=None, verbose=False, use_cache=True):
     '''
     update sigma2 (variance paramter of the lognormal distribution) given theta (celltype proportion), e_alpha (spot-specific effect) and gamma_g (gene-specific platform effect) by MLE
     
-    we assume ln(lambda) = alpha + gamma_g + ln(sum(theta*mu_X)) + epsilon
-              subject to sum(theta)=1, theta>=0
+    we assume
+    
+        ln(lambda) = alpha + gamma_g + ln(sum(theta*mu_X)) + epsilon
+        
+        subject to sum(theta)=1, theta>=0
     
     mu_X is marker genes from data['X']
     
     then the mean parameter of the log-normal distribution of ln(lambda) is alpha + gamma_g + ln(sum(theta*mu_X))
     
     we did re-parametrization w = e^alpha * theta, then
     
-              ln(lambda) = gamma_g + ln(sum([e^alpha*theta]*mu_X)) + epsilon
-              subject to w>=0, it will imply sum(theta)=1 and theta>=0
+        ln(lambda) = gamma_g + ln(sum([e^alpha*theta]*mu_X)) + epsilon
+        
+        subject to w>=0, it will imply sum(theta)=1 and theta>=0
               
     currently optimization of sigma2 DO NOT support parallel computing
 
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.
     theta : 3-D numpy array (spots * celltypes * 1)
         theta (celltype proportion).
     e_alpha : 1-D numpy array
         e_alpha (spot-specific effect).
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     sigma2 : float
@@ -1095,21 +1145,26 @@
 def adaptive_lasso(nu, rho, lambda_r=1.0, lasso_weight=None):
     '''
     update theta_tilde by Adaptive Lasso and ADMM loss
     
     theta_tilde = argmin lambda_r*lasso_weight*theta_tilde + 1/(2*rho) * (||theta_tilde-theta_hat+u_tilde||_2)^2
     
     that is
-            -if theta_tilde>=0, theta_tilde = theta_hat - u_tilde - lambda_r*rho*lasso_weight
-            -if theta_tilde<0, theta_tilde = theta_hat - u_tilde + lambda_r*rho*lasso_weight
+    
+        - if theta_tilde>=0, theta_tilde = theta_hat - u_tilde - lambda_r*rho*lasso_weight
+        
+        - if theta_tilde<0, theta_tilde = theta_hat - u_tilde + lambda_r*rho*lasso_weight
             
     change it to
-            -if theta_hat-u_tilde-lambda_r*rho*lasso_weight>=0, theta_tilde = theta_hat - u_tilde - lambda_r*rho*lasso_weight
-            -if theta_hat-u_tilde+lambda_r*rho*lasso_weight<=0, theta_tilde = theta_hat - u_tilde + lambda_r*rho*lasso_weight
-            -if theta_hat-u_tilde-lambda_r*rho*lasso_weight<0 or theta_hat-u_tilde+lambda_r*rho*lasso_weight>0, not defined, let theta_tilde = 0
+    
+        - if theta_hat-u_tilde-lambda_r*rho*lasso_weight>=0, theta_tilde = theta_hat - u_tilde - lambda_r*rho*lasso_weight
+        
+        - if theta_hat-u_tilde+lambda_r*rho*lasso_weight<=0, theta_tilde = theta_hat - u_tilde + lambda_r*rho*lasso_weight
+        
+        - if theta_hat-u_tilde-lambda_r*rho*lasso_weight<0 or theta_hat-u_tilde+lambda_r*rho*lasso_weight>0, not defined, let theta_tilde = 0
             
     and nu = theta_hat - u_tilde
     
     WANRING: negative theta tilde value observed, so also clip it to >= 0
 
     Parameters
     ----------
```

### Comparing `sdeper-1.0.3/src/model_fit.py` & `sdeper-1.1.0/src/model_fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,24 @@
     
     when fitting the base model, we will perform fitting iteratively until the sigma^2 change <= 0.001
     
     Note: the output of the fit result is 3-Dimensional. The dimension transform will be performed outside this function if needed
 
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes)
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes)
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.\n
+            celltype_names: a list of string of celltype names.
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     global_optimize : bool, optional
         if is True, use basin-hopping algorithm to find the global minimum. The default is False.
     hybrid_version : bool, optional
         if True, use the hybrid_version of GLRM, i.e. in ADMM local model loss function optimization for w but adaptive lasso constrain on theta. If False, local model loss function optimization and adaptive lasso will on the same w. The default is True.
     opt_method : string, optional
@@ -56,17 +57,17 @@
         if True, print more information in program running.
     use_cache : bool, optional
         if True, use the cached dict of calculated negative log-likelihood values.
 
     Returns
     -------
     tuple
-        a tuple of estimated theta, e_alpha and sigma2
-            theta : celltype proportions (3-D numpy array (spots * celltypes * 1))
-            e_alpha : spot-specific effect (1-D array with length #spot)
+        a tuple of estimated theta, e_alpha and sigma2:
+            theta : celltype proportions (3-D numpy array (spots * celltypes * 1))\n
+            e_alpha : spot-specific effect (1-D array with length #spot)\n
             sigma2 : variance paramter of the lognormal distribution (float)
     '''
 
     start_time = time()
     
     n_celltype, n_gene = data['X'].shape
     n_spot = data['Y'].shape[0]
@@ -146,23 +147,24 @@
 
 def estimating_gamma_g(data, hybrid_version=True, opt_method='L-BFGS-B', verbose=False):
     """
     estimate platform effect gamma_g by fit model on pseudo-bulk measurement
 
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes)
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes)
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.\n
+            celltype_names: a list of string of celltype names.
     hybrid_version : bool, optional
         if True, use the hybrid_version of GLRM, i.e. in ADMM local model loss function optimization for w but adaptive lasso constrain on theta. If False, local model loss function optimization and adaptive lasso will on the same w. The default is True.
     opt_method : string, optional
         specify method used in scipy.optimize.minimize for local model fitting. The default is 'L-BFGS-B', a default method in scipy for optimization with bounds. Another choice would be 'SLSQP', a default method in scipy for optimization with constrains and bounds.
     verbose : bool, optional
         if True, print more information in program running
     
@@ -207,23 +209,24 @@
 
 def fit_model_two_stage(data, G, gamma_g=None, lambda_r=None, weight_threshold=1e-3, lambda_g=None, global_optimize=False, hybrid_version=True, opt_method='L-BFGS-B', verbose=False, use_cache=True, diagnosis=False):
     """
     fit Graph Laplacian Regularized Stratified Model (GLRM) in a two-stage way
     
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.
     G : built graph object from networks module
         used for constructing Laplacian Matrix
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     lambda_r : float
         strength for Adaptive Lasso penalty. If None, use cross-validation to determine optimal lambda_r
     weight_threshold : float, optional
@@ -243,19 +246,19 @@
     diagnosis : bool
         if True save more information to files for diagnosis CVAE and hyper-parameter selection
 
     Returns
     -------
     Dict
         estimated model coefficients, including:
-            theta : celltype proportions (#spots * #celltypes * 1)
-            e_alpha : spot-specific effect (1-D array with length #spot)
-            sigma2 : variance paramter of the lognormal distribution (float)
-            gamma_g : gene-specific platform effect for all genes (1-D array with length #gene)
-            theta_tilde : celltype proportions for Adaptive Lasso (#spots * #celltypes * 1)
+            theta : celltype proportions (#spots * #celltypes * 1)\n
+            e_alpha : spot-specific effect (1-D array with length #spot)\n
+            sigma2 : variance paramter of the lognormal distribution (float)\n
+            gamma_g : gene-specific platform effect for all genes (1-D array with length #gene)\n
+            theta_tilde : celltype proportions for Adaptive Lasso (#spots * #celltypes * 1)\n
             theta_hat : celltype proportions for Graph Laplacian constrain (#spots * #celltypes * 1)
     """
     
     print('\n\nStart GLRM fitting...\n')
     
     start_time = time()
```

### Comparing `sdeper-1.0.3/src/parse_opt.py` & `sdeper-1.1.0/src/parse_opt.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,27 @@
 
 
 from getopt import getopt
 import sys, os
 from config import print, input_path, cur_version
 import numpy as np
 import pandas as pd
+import copy
+
+
+
+# default value for options
+default_paramdict = {'spatial_file': None, 'ref_file': None, 'ref_celltype_file': None, 'marker_file': None, 'loc_file': None, 'A_file': None,
+                     'n_cores': 1, 'threshold': 0, 'use_cvae': True, 'use_imputation': False, 'diagnosis': False, 'verbose': True,
+                     'use_fdr': True, 'p_val_cutoff': 0.05, 'fc_cutoff': 1.2, 'pct1_cutoff': 0.3, 'pct2_cutoff': 0.1, 'sortby_fc': True, 'n_marker_per_cmp': 10, 'filter_cell': True, 'filter_gene': True,
+                     'n_hv_gene': 200,  'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.003, 'redo_de': True, 'seed': 383,
+                     'lambda_r': None, 'lambda_r_range_min': 0.1, 'lambda_r_range_max': 100, 'lambda_r_range_k': 8,
+                     'lambda_g': None, 'lambda_g_range_min': 0.1, 'lambda_g_range_max': 100, 'lambda_g_range_k': 8,
+                     'diameter': 200, 'impute_diameter': [160, 114, 80]
+                    }
 
 
 
 def usage():
     '''
     help information of the main function
     
@@ -28,49 +41,95 @@
     None.
     
     Returns
     -------
     None.
     '''
     
-    print('''
+    print(f'''
 runDeconvolution [option][value]...
+
     -h or --help            print this help messages.
-    -q or --query           input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes), with absolute or relative path. Rows as spots and columns as genes. Row header as spot barcodes and column header as gene symbols are required.
-    -r or --ref             input csv file of raw nUMI counts in scRNA-seq data (cells * genes), with absolute or relative path. Rows as cells and columns as genes. Row header as cell barcodes and column header as gene symbols are required.
-    -c or --ref_anno        input csv file of cell-type annotations for all cells in scRNA-seq data, with absolute or relative path. Rows as cells and only 1 column as cell-type annotation. Row header as cell barcodes and column header as cell-types are required.
-    -m or --marker          input csv file of already curated cell-type marker gene expression (cell-types * genes; already normalized to remove effect of sequencing depth), with absolute or relative path. Rows as cell-types and columns as genes. Row header as cell-type names and column header as gene symbols are required. If marker gene expression is provided, the built-in differential analysis will be skipped and genes from this csv file will be directly used for cell-type deconvolution, as well as CVAE building if needed. If not provided, Wilcoxon rank sum test will be performed to select cell-type marker genes.
-    -l or --loc             input csv file of row/column integer index (x,y) of spatial spots (spots * 2), with absolute or relative path. Rows as spots and columns are coordinates x (column index) and y (row index). Row header as spot barcodes and column header "x","y" are both required. NOTE 1) the column header must be either "x" or "y" (lower case), 2) x and y are integer index (1,2,3,...) not pixels. This spot location file is required for imputation.
-    -a or --adjacency       input csv file of Adjacency Matrix of spots in spatial transcriptomic data (spots * spots), with absolute or relative path. In the Adjacency Matrix, spots within neighborhood have a value 1, otherwises have a value 0, and diagonal entries are all 0. Row header and column header as spot barcodes are required. And the spot order should be consist with row order in spatial data. Default value is None.
-    -n or --n_cores         number of CPU cores used for parallel computing. Default value is 1, i.e. no parallel computing.
-    --lambda_r              hyper-parameter for Adaptive Lasso. Default value is None, i.e. use cross-validation to find the optimal value. The list of lambda_r candidates will has total lambda_r_range_k values, and candidate values will be evenly selected on a log scale (geometric progression) from range [lambda_r_range_min, lambda_r_range_max]. If lambda_r is specified as a valid value, then lambda_r_range_k, lambda_r_range_min and lambda_r_range_max will be ignored.
-    --lambda_r_range_min    minimum value of the range of lambda_r candidates used for hyper-parameter selection. Default value is 0.1.
-    --lambda_r_range_max    maximum value of the range of lambda_r candidates used for hyper-parameter selection. Default value is 100.
-    --lambda_r_range_k      number of lambda_r candidates used for hyper-parameter selection. Default value is 8 (including the values of lambda_r_range_min and lambda_r_range_max).
-    --lambda_g              hyper-parameter for Graph Laplacian Constrain, which equals the edge weights used in the Graph created from the Adjacency Matrix. Default value is None, i.e. use cross-validation to find the optimal value. The list of lambda_g candidates will has total lambda_g_range_k values, and candidate values will be evenly selected on a log scale (geometric progression) from range [lambda_g_range_min, lambda_g_range_max]. If lambda_g is specified as a valid value, then lambda_g_range_k, lambda_g_range_min and lambda_g_range_max will be ignored.
-    --lambda_g_range_min    minimum value of the range of lambda_g candidates used for hyper-parameter selection. Default value is 0.1.
-    --lambda_g_range_max    maximum value of the range of lambda_g candidates used for hyper-parameter selection. Default value is 100.
-    --lambda_g_range_k      number of lambda_g candidates used for hyper-parameter selection. Default value is 8 (including the values of lambda_g_range_min and lambda_g_range_max).
-    --use_cvae              control whether to build Conditional Variational Autoencoder (CVAE) to adjust the platform effect between spatial transcriptomic and scRNA-seq (true/false). Default value is true. Building CVAE requires raw nUMI counts and corresponding cell-type annotation of scRNA-seq data specified.
-    --threshold             threshold for hard thresholding the estimated cell-type proportions, i.e. for one spot, estimated cell-type proportions smaller than this threshold value will be set to 0 , then re-normalize all proportions of this spot to sum as 1. Default value is 0, which means no hard thresholding.
-    --n_hv_gene             number of highly variable genes identified in scRNA-seq data and then used for building CVAE. Default number is 1,000. If the actual number of genes in scRNA-seq data is less than the specified value, all genes in scRNA-seq data will be used for CVAE.
-    --n_marker_per_cmp      number of selected TOP cell-type specified marker genes for each comparison of ONE cell-type against another ONE cell-type using Wilcoxon rank sum test. Default number is 30. For each comparison, genes with a FDR adjusted p value < 0.05 will be selected first, then these marker genes will be sorted by a combined rank of log fold change and pct.1/pct.2, and finally pick up specified number of gene with TOP ranks.
-    --pseudo_spot_min_cell  minimum value of cells in one pseudo-spot for building CVAE. Default value is 2.
-    --pseudo_spot_max_cell  maximum value of cells in one pseudo-spot for building CVAE. Default value is 8.
-    --seq_depth_scaler      a scaler of scRNA-seq sequencing depth to transform sequencing depth normalized gene expressions back to raw nUMI after CVAE transformation. Default value is 10,000 for all cells.
-    --cvae_input_scaler     maximum value of the scaled input for CVAE input layer. Default value is 10, i.e. scale all the sequencing depth normalized gene expressions to range [0, 10].
-    --cvae_init_lr          initial learning rate for training CVAE. Default value is 0.003. Althoug learning rate will decreasing automatically during training, large initial learning rate will cause training failure at the very beginning of training. If loss function value do NOT monotonically decrease, please try smaller initial learning rate.
-    --redo_de               control whether to redo Differential analysis on CVAE transformed scRNA-seq gene expression to get a new set of marker gene list for cell-types (true/false). Default value is true. It's recommended to redo Differential analysis since CVAE transformation may change the marker gene profile of cell-types.
-    --seed                  seed value for random in building CVAE. Default value is 383.
-    --diagnosis             if true, provide more outputs related to CVAE and hyper-parameter selection for diagnosis. Default value is false.
-    --verbose               control whether to print more info of ADMM during program running (true/false). Default value is true.
-    -v or --version         print version of CVAE-GLRM
-    --use_imputation        control whether to perform imputation (true/false). Default value is false. Imputation requires the spot diameter (µm) at higher resolution to be specified.
-    --diameter              the physical diameter (µm) of spatial spots. Default value is 200.
-    --impute_diameter       the target spot diameter (µm) during imputation. Either one number or an array of numbers separated by "," are supported. Default value is 160,114,80, corresponding to the low, medium, high resolution.
+    -v or --version         print version of SDePER
+    
+    
+    --------------- Input options -------------------
+    
+    -q or --query           input csv file of raw nUMI counts of spatial transcriptomic data (spots * genes), with absolute or relative path. Rows as spots and columns as genes. Row header as spot barcodes and column header as gene symbols are both required.
+    -r or --ref             input csv file of raw nUMI counts of scRNA-seq data (cells * genes), with absolute or relative path. Rows as cells and columns as genes. Row header as cell barcodes and column header as gene symbols are both required.
+    -c or --ref_anno        input csv file of cell-type annotations for all cells in scRNA-seq data, with absolute or relative path. Rows as cells and only 1 column as cell-type annotation. Row header as cell barcodes and column header with arbitrary name are both required.
+    -m or --marker          input csv file of already curated cell-type marker gene expression (cell-types * genes; already normalized by sequencing depth), with absolute or relative path. Rows as cell-types and columns as genes. Row header as cell-type names and column header as gene symbols are both required. If marker gene expression is provided, the built-in differential analysis will be skipped and genes from this csv file will be directly used for cell-type deconvolution, as well as CVAE building. If not provided, Wilcoxon rank sum test will be performed to select cell-type marker genes. Default value is {default_paramdict["marker_file"]}.
+    -l or --loc             input csv file of row/column integer index (x,y) of spatial spots (spots * 2), with absolute or relative path. Rows as spots and columns are coordinates x (column index) and y (row index). Row header as spot barcodes and column header "x","y" are both required. NOTE 1) the column header must be either "x" or "y" (lower case), 2) x and y are integer index (1,2,3,...) not pixels. This spot location file is required for imputation. Default value is {default_paramdict["loc_file"]}.
+    -a or --adjacency       input csv file of Adjacency Matrix of spots in spatial transcriptomic data (spots * spots), with absolute or relative path. In Adjacency Matrix, entry value 1 represents corresponding two spots are adjacent spots according to the definition of neighborhood, while value 0 for non-adjacent spots. All diagonal entries are set as 0. Row header and column header as spot barcodes are both required. And the spot order should be consist with row order in spatial data. Default value is {default_paramdict["A_file"]}.
+    
+    
+    --------------- Output options -------------------
+    
+    We do not provide options for renaming output files. All outputs are in the same folder as input files.
+    The cell-type deconvolution result file is named as "celltype_proportions.csv".
+    If imputation is enabled, for each specified spot diameter d µm, there will be three more output files: 1) imputed spot locations "impute_diameter_d_spot_loc.csv", 2) imputed spot cell-type proportions "impute_diameter_d_spot_celltype_prop.csv", 3) imputed spot gene expressions (already normalized by sequencing depth of spots) "impute_diameter_d_spot_gene_norm_exp.csv".
+    
+    
+    --------------- General options -------------------
+    
+    -n or --n_cores         number of CPU cores used for parallel computing. Default value is {default_paramdict["n_cores"]}, i.e. no parallel computing.
+    --threshold             threshold for hard thresholding the estimated cell-type proportions, i.e. for one spot, estimated cell-type proportions smaller than this threshold value will be set to 0, then re-normalize all proportions of this spot to sum as 1. Default value is {default_paramdict["threshold"]}, which means no hard thresholding.
+    --use_cvae              control whether to build Conditional Variational Autoencoder (CVAE) to remove the platform effect between spatial transcriptomic and scRNA-seq data (true/false). Default value is {default_paramdict["use_cvae"]}. Building CVAE requires raw nUMI counts and corresponding cell-type annotation of scRNA-seq data specified.
+    --use_imputation        control whether to perform imputation (true/false). Default value is {default_paramdict["use_imputation"]}. Imputation requires the spot diameter (µm) at higher resolution to be specified.
+    --diagnosis             if true, provide more output files related to CVAE building and hyper-parameter selection for diagnosis. Default value is {default_paramdict["diagnosis"]}.
+    --verbose               control whether to print more info such as output of each ADMM iteration step during program running (true/false). Default value is {default_paramdict["verbose"]}.
+    
+    
+    ----- Cell-type marker identification options ------
+    
+    Cell-type specific markers are identified by Differential analysis (DE) across cell-types in reference scRNA-seq data. We also perform cell and/or gene filtering before DE. Each time we ONLY compare the normalized gene expression (raw nUMI counts divided by sequencing depth) one cell-type (1st) vs another one cell-type (2nd) using Wilcoxon Rank Sum Test, then take the UNION of all identified markers for downstream analysis. We filter the marker genes with pre-set thresholds of p value (or FDR), fold change, pct.1 (percentage of cells expressed this marker in 1st cell-type) and pct.2 (percentage of cells expressed this marker in 2nd cell-type). Next we sort the marker genes by p value (or FDR) or fold change, and select the TOP ones. The options related to cell-type marker identification are listed as below:
+    
+    --use_fdr               whether to use FDR adjusted p value for filtering and sorting. Default value is {default_paramdict["use_fdr"]}, i.e. use FDR adjusted p value. If false orginal p value will be used instead.
+    --p_val_cutoff          threshold of p value (or FDR if `--use_fdr` is true) in marker genes filtering. Default value is {default_paramdict["p_val_cutoff"]}, and only genes with p value (or FDR if `--use_fdr` is true) <= {default_paramdict["p_val_cutoff"]} will be kept.
+    --fc_cutoff             threshold of fold change (without log transform!) in marker genes filtering. Default value is {default_paramdict["fc_cutoff"]}, and only genes with fold change >= {default_paramdict["fc_cutoff"]} will be kept.
+    --pct1_cutoff           threshold of pct.1 (percentage of cells expressed this marker in 1st cell-type) in marker genes filtering. Default value is {default_paramdict["pct1_cutoff"]}, and only genes with pct.1 >= {default_paramdict["pct1_cutoff"]} will be kept.
+    --pct2_cutoff           threshold of pct.2 (percentage of cells expressed this marker in 2nd cell-type) in marker genes filtering. Default value is {default_paramdict["pct2_cutoff"]}, and only genes with pct.2 <= {default_paramdict["pct2_cutoff"]} will be kept.
+    --sortby_fc             whether to sort marker genes by fold change. Default value is {default_paramdict["sortby_fc"]}, i.e. sort marker genes by fold change then select TOP ones. If false, p value (or FDR if `--use_fdr` is true) will be used to sort marker genes instead.
+    --n_marker_per_cmp      number of selected TOP marker genes for each comparison of ONE cell-type against another ONE cell-type using Wilcoxon Rank Sum Test. Default number is {default_paramdict["n_marker_per_cmp"]}. For each comparison, genes passing filtering will be selected first, then these marker genes will be sorted by fold change or p value (or FDR), and finally pick up specified number of genes with TOP ranks. If the number of available genes is less than the specified number, a WARNING will be shown in the program running log file.
+    --filter_cell           whether to filter cells with <200 genes for reference scRNA-seq data before differential analysis. Default value is {default_paramdict["filter_cell"]}, i.e. filter cells first.
+    --filter_gene           whether to filter genes presented in <10 cells for reference scRNA-seq data and <3 spots for spatial data before differential analysis. Default value is {default_paramdict["filter_gene"]}, i.e. filter genes first.
+    
+    
+    --------------- CVAE related options ---------------
+    
+    We build Conditional Variational Autoencoder (CVAE) to adjust the platform effect between spatial transcriptomic and scRNA-seq data. The input of CVAE includes scRNA-seq cells, pseudo-spots generated by aggregating randomly selected cells and real spatial spots. To successfully train a neural network model is non-trivial, and model Topology together with most related hyper-parameters have been pre-fixed based on our experiences on analysis of various spatial transcriptomic datasets. The options can be tuned by users are listed as below:
+    
+    --n_hv_gene             number of highly variable genes identified in reference scRNA-seq data, and these HV genes will be used together with identified cell-type marker genes for building CVAE. Default number is {default_paramdict["n_hv_gene"]}. If the actual number of genes in scRNA-seq data is less than the specified value, all available genes in scRNA-seq data will be used for building CVAE.
+    --pseudo_spot_min_cell  minimum value of cells in one pseudo-spot when combining cells into pseudo-spots. Default value is {default_paramdict["pseudo_spot_min_cell"]}.
+    --pseudo_spot_max_cell  maximum value of cells in one pseudo-spot when combining cells into pseudo-spots. Default value is {default_paramdict["pseudo_spot_max_cell"]}.
+    --seq_depth_scaler      a scaler of scRNA-seq sequencing depth to transform CVAE decoded values (sequencing depth normalized gene expressions) back to raw nUMI counts. Default value is {default_paramdict["seq_depth_scaler"]} for all cells.
+    --cvae_input_scaler     maximum value of the scaled input for CVAE input layer. Default value is {default_paramdict["cvae_input_scaler"]}, i.e. linearly scale all the sequencing depth normalized gene expressions to range [0, {default_paramdict["cvae_input_scaler"]}].
+    --cvae_init_lr          initial learning rate for training CVAE. Default value is {default_paramdict["cvae_init_lr"]}. Although learning rate will decreasing automatically during training, large initial learning rate will cause training failure at the very beginning of training. If loss function value do NOT monotonically decrease, please try smaller initial learning rate.
+    --redo_de               control whether to redo Differential analysis on CVAE transformed scRNA-seq gene expressions to get a new set of marker gene list of cell-types (true/false). Default value is {default_paramdict["redo_de"]}. It's recommended to redo Differential analysis since CVAE transformation may change the marker gene profile of cell-types.
+    --seed                  seed value of TensorFlow to control the randomness in building CVAE. Default value is {default_paramdict["seed"]}.
+    
+    
+    -------------- GLRM hyper-parameter related options ---------------
+    
+    We incorporate adaptive Lasso penalty and graph Laplacian penalty in GLRM, and use the hyper-parameters lambda_r and lambda_g to balance the strength of those two penalties respectively.
+    
+    --lambda_r              hyper-parameter for adaptive Lasso. Default value is {default_paramdict["lambda_r"]}, i.e. use cross-validation to find the optimal value. The list of lambda_r candidates will has total `lambda_r_range_k` values, and candidate values will be evenly selected on a log scale (geometric progression) from range [`lambda_r_range_min`, `lambda_r_range_max`]. If `lambda_r` is specified as a valid value, then `lambda_r_range_k`, `lambda_r_range_min` and `lambda_r_range_max` will be ignored.
+    --lambda_r_range_min    minimum value of the range of lambda_r candidates used for hyper-parameter selection. Default value is {default_paramdict["lambda_r_range_min"]}.
+    --lambda_r_range_max    maximum value of the range of lambda_r candidates used for hyper-parameter selection. Default value is {default_paramdict["lambda_r_range_max"]}.
+    --lambda_r_range_k      number of lambda_r candidates used for hyper-parameter selection. Default value is {default_paramdict["lambda_r_range_k"]} (including the values of `lambda_r_range_min` and `lambda_r_range_max`).
+    --lambda_g              hyper-parameter for graph Laplacian constrain, which depends on the edge weights used in the graph created from the Adjacency Matrix. Default value is {default_paramdict["lambda_g"]}, i.e. use cross-validation to find the optimal value. The list of lambda_g candidates will has total `lambda_g_range_k` values, and candidate values will be evenly selected on a log scale (geometric progression) from range [`lambda_g_range_min`, `lambda_g_range_max`]. If `lambda_g` is specified as a valid value, then `lambda_g_range_k`, `lambda_g_range_min` and `lambda_g_range_max` will be ignored.
+    --lambda_g_range_min    minimum value of the range of lambda_g candidates used for hyper-parameter selection. Default value is {default_paramdict["lambda_g_range_min"]}.
+    --lambda_g_range_max    maximum value of the range of lambda_g candidates used for hyper-parameter selection. Default value is {default_paramdict["lambda_g_range_max"]}.
+    --lambda_g_range_k      number of lambda_g candidates used for hyper-parameter selection. Default value is {default_paramdict["lambda_g_range_k"]} (including the values of `lambda_g_range_min` and `lambda_g_range_max`).
+    
+    
+    -------------- imputation related options ---------------
+    
+    --diameter              the physical diameter (µm) of spatial spots. Default value is {default_paramdict["diameter"]}.
+    --impute_diameter       the target spot diameter (µm) during imputation. Either one number or an array of numbers separated by "," are supported. Default value is {",".join([str(x) for x in default_paramdict["impute_diameter"]])}, corresponding to the low, medium, high resolution.
 ''')
 
 
 def parseOpt():
     '''
     parse the command line parameters and return them as a dict
     
@@ -78,67 +137,77 @@
     ----------
     None.
 
     Returns
     -------
     paramdict : Dict
         parsed command line parameters for model, including:
-            spatial_file : full file path of spatial transcriptomic data
-            ref_file : full file path of scRNA-seq data
-            ref_celltype_file : full file path of the corresponding cell-type annotation of scRNA-seq data
-            marker_file : full file path of user curated cell-type marker gene expression
-            loc_file : full file path of spot locations in spatial transcriptomic data
-            A_file : full file path Adjacency Matrix of spots in spatial transcriptomic data
-            n_cores : number of CPU cores used for parallel computing
-            lambda_r : hyper-parameter for Adaptive Lasso
-            lambda_g : hyper-parameter for graph weight, affecting the Laplacian Matrix
-            use_cvae : whether to build CVAE
-            threshold : threshold for hard thresholding estimated cell-type proportion theta
-            n_hv_gene : number of highly variable genes for CVAE
-            n_marker_per_cmp : number of TOP marker genes for each comparison in DE
-            pseudo_spot_min_cell : minimum value of cells in pseudo-spot
-            pseudo_spot_max_cell : maximum value of cells in pseudo-spot
-            seq_depth_scaler : a scaler of scRNA-seq sequencing depth
-            cvae_input_scaler : maximum value of the scaled input for CVAE
-            cvae_init_lr : initial learning rate for training CVAE
-            redo_de : whether to redo DE after CVAE transformation
-            seed : seed value for random in building CVAE
-            diagnosis : True or False, if True save more information to files for diagnosis CVAE and hyper-parameter selection
-            verbose : True or False, if True print more information during program running
-            use_imputation : whether to perform imputation
-            diameter : the physical diameter of spatial spots
+            spatial_file : full file path of spatial transcriptomic data\n
+            ref_file : full file path of scRNA-seq data\n
+            ref_celltype_file : full file path of the corresponding cell-type annotation of scRNA-seq data\n
+            marker_file : full file path of user curated cell-type marker gene expression\n
+            loc_file : full file path of spot locations in spatial transcriptomic data\n
+            A_file : full file path Adjacency Matrix of spots in spatial transcriptomic data\n
+            n_cores : number of CPU cores used for parallel computing\n
+            lambda_r : hyper-parameter for Adaptive Lasso\n
+            lambda_g : hyper-parameter for graph weight, affecting the Laplacian Matrix\n
+            use_cvae : whether to build CVAE\n
+            threshold : threshold for hard thresholding estimated cell-type proportion theta\n
+            n_hv_gene : number of highly variable genes for CVAE\n
+            n_marker_per_cmp : number of TOP marker genes for each comparison in DE\n
+            pseudo_spot_min_cell : minimum value of cells in pseudo-spot\n
+            pseudo_spot_max_cell : maximum value of cells in pseudo-spot\n
+            seq_depth_scaler : a scaler of scRNA-seq sequencing depth\n
+            cvae_input_scaler : maximum value of the scaled input for CVAE\n
+            cvae_init_lr : initial learning rate for training CVAE\n
+            redo_de : whether to redo DE after CVAE transformation\n
+            seed : seed value for random in building CVAE\n
+            diagnosis : True or False, if True save more information to files for diagnosis CVAE and hyper-parameter selection\n
+            verbose : True or False, if True print more information during program running\n
+            use_fdr : whether to use FDR adjusted p value for filtering and sorting\n
+            p_val_cutoff : threshold of p value (or FDR if --use_fdr is true) in marker genes filtering\n
+            fc_cutoff : threshold of fold change (without log transform!) in marker genes filtering\n
+            pct1_cutoff : threshold of pct.1 in marker genes filtering\n
+            pct2_cutoff : threshold of pct.2 in marker genes filtering\n
+            sortby_fc : whether to sort marker genes by fold change\n
+            filter_cell : whether to filter cells before DE\n
+            filter_gene : whether to filter genes before DE\n
+            use_imputation : whether to perform imputation\n
+            diameter : the physical diameter of spatial spots\n
             impute_diameter : target spot diameter for imputation
     '''
     
     # 如果没有任何参数，显示提示信息，并退出
     if len(sys.argv) == 1:
         print('No options exist!')
         print('Use -h or --help for detailed help!')
         sys.exit(1)
         
     # 定义命令行参数
     # 短选项名后的冒号(:)表示该选项必须有附加的参数
     # 长选项名后的等号(=)表示该选项必须有附加的参数
     shortargs = 'hq:r:c:m:l:a:o:n:v'
-    longargs = ['help', 'query=', 'ref=', 'ref_anno=', 'marker=', 'loc=', 'adjacency=', 'n_cores=', 'lambda_r=', 'lambda_r_range_min=', 'lambda_r_range_max=', 'lambda_r_range_k=', 'lambda_g=', 'lambda_g_range_min=', 'lambda_g_range_max=', 'lambda_g_range_k=', 'use_cvae=', 'threshold=', 'n_hv_gene=', 'n_marker_per_cmp=', 'pseudo_spot_min_cell=', 'pseudo_spot_max_cell=', 'seq_depth_scaler=', 'cvae_input_scaler=', 'cvae_init_lr=', 'redo_de=', 'seed=', 'diagnosis=', 'verbose=', 'use_imputation=', 'diameter=', 'impute_diameter=', 'version']
+    longargs = ['help', 'query=', 'ref=', 'ref_anno=', 'marker=', 'loc=', 'adjacency=', 'n_cores=', 'lambda_r=', 'lambda_r_range_min=', 'lambda_r_range_max=', 'lambda_r_range_k=', 'lambda_g=', 'lambda_g_range_min=', 'lambda_g_range_max=', 'lambda_g_range_k=', 'use_cvae=', 'threshold=', 'n_hv_gene=', 'n_marker_per_cmp=', 'pseudo_spot_min_cell=', 'pseudo_spot_max_cell=', 'seq_depth_scaler=', 'cvae_input_scaler=', 'cvae_init_lr=', 'redo_de=', 'seed=', 'diagnosis=', 'verbose=', 'use_fdr=', 'p_val_cutoff=', 'fc_cutoff=', 'pct1_cutoff=', 'pct2_cutoff=', 'sortby_fc=', 'filter_cell=', 'filter_gene=', 'use_imputation=', 'diameter=', 'impute_diameter=', 'version']
     
   
     # 解析命令行参数
     # sys.argv[0]为python脚本名，后续全为参数
     # opts为分析出的参数信息，args为不符合格式信息的剩余参数
     opts, args = getopt(sys.argv[1:], shortargs, longargs)
     
     # 如果存在不符合格式信息的剩余参数，显示提示信息，并退出
     if args:
         print('Invalid options exist!')
         print('Use -h or --help for detailed help')
         sys.exit(1)
         
     # 定义dict类型的参数集，使得程序更稳健
-    paramdict = {'spatial_file': None, 'ref_file': None, 'ref_celltype_file': None, 'marker_file': None, 'loc_file': None, 'A_file': None, 'n_cores': 1, 'lambda_r': None, 'lambda_r_range_min': 0.1, 'lambda_r_range_max': 100, 'lambda_r_range_k': 8, 'lambda_g': None, 'lambda_g_range_min': 0.1, 'lambda_g_range_max': 100, 'lambda_g_range_k': 8, 'use_cvae': True, 'threshold': 0, 'n_hv_gene': 1000, 'n_marker_per_cmp': 30, 'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.003, 'redo_de': True, 'seed': 383, 'diagnosis': False, 'verbose': True, 'use_imputation': False, 'diameter': 200, 'impute_diameter': [160, 114, 80]}
+    # a deep copy
+    paramdict = copy.deepcopy(default_paramdict)
+    
     
     for opt,val in opts:
         
         if opt in ('-h', '--help'):
             usage()
             sys.exit(0)  # exit with success
             
@@ -213,279 +282,367 @@
                 paramdict['n_cores'] = int(float(val))
                 
                 if paramdict['n_cores'] > os.cpu_count():
                     print(f'WARNING: user set using `{paramdict["n_cores"]}` CPU cores but system only has `{os.cpu_count()}` cores. Reset CPU cores to `{os.cpu_count()}`')
                     paramdict['n_cores'] = os.cpu_count()
                 
                 if paramdict['n_cores'] < 1:
-                    print(f'WARNING: invalid option value `{paramdict["n_cores"]}` for CPU cores! Please use integer which >= 1. Currently CPU cores is set to be default value `1`')
-                    paramdict['n_cores'] = 1
+                    print(f'WARNING: invalid option value `{paramdict["n_cores"]}` for CPU cores! Please use integer which >= 1. Currently CPU cores is set to be default value `{default_paramdict["n_cores"]}`')
+                    paramdict['n_cores'] = default_paramdict["n_cores"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for CPU cores! Please use numeric value. Currently CPU cores is set to be default value `1`!')
+                print(f'WARNING: unrecognized option value `{val}` for CPU cores! Please use numeric value. Currently CPU cores is set to be default value `{default_paramdict["n_cores"]}`!')
             continue
         
     
         if opt in ('--lambda_r'):
             if val.casefold() == 'none'.casefold():
                 paramdict['lambda_r'] = None
                 continue
             else:
                 try:
                     paramdict['lambda_r'] = float(val)
                     
                     if paramdict['lambda_r'] < 0:
-                        print(f'WARNING: negative option value `{paramdict["lambda_r"]}` for lambda_r! Please use non-negative value. Currently lambda_r is set to be default value `None`!')
-                        paramdict['lambda_r'] = None
+                        print(f'WARNING: negative option value `{paramdict["lambda_r"]}` for lambda_r! Please use non-negative value. Currently lambda_r is set to be default value `{default_paramdict["lambda_r"]}`!')
+                        paramdict['lambda_r'] = default_paramdict["lambda_r"]
                 except:
-                    print(f'WARNING: unrecognized option value `{val}` for lambda_r! Please use numeric value or `none`. Currently lambda_r is set to be default value `None`!')
+                    print(f'WARNING: unrecognized option value `{val}` for lambda_r! Please use numeric value or `none`. Currently lambda_r is set to be default value `{default_paramdict["lambda_r"]}`!')
                 continue
             
             
         if opt in ('--lambda_r_range_min'):
             try:
                 paramdict['lambda_r_range_min'] = float(val)
                 
-                if paramdict['lambda_r_range_min'] <= 0:
-                    print(f'WARNING: non-positive option value `{paramdict["lambda_r_range_min"]}` for lambda_r_range_min! Please use positve value. Currently lambda_r_range_min is set to be default value `0.1`!')
-                    paramdict['lambda_r_range_min'] = 0.1
+                if paramdict['lambda_r_range_min'] < 0:
+                    print(f'WARNING: negative option value `{paramdict["lambda_r_range_min"]}` for lambda_r_range_min! Please use non-negative value. Currently lambda_r_range_min is set to be value `0`!')
+                    paramdict['lambda_r_range_min'] = 0
             except:
-                print(f'WARNING: unrecognized option value `{val}` for lambda_r_range_min! Please use numeric value. Currently lambda_r_range_min is set to be default value `0.1`!')
+                print(f'WARNING: unrecognized option value `{val}` for lambda_r_range_min! Please use numeric value. Currently lambda_r_range_min is set to be default value `{default_paramdict["lambda_r_range_min"]}`!')
             continue
         
         
         if opt in ('--lambda_r_range_max'):
             try:
                 paramdict['lambda_r_range_max'] = float(val)
                 # checking max value in the final check
             except:
-                print(f'WARNING: unrecognized option value `{val}` for lambda_r_range_max! Please use numeric value. Currently lambda_r_range_max is set to be default value `100`!')
+                print(f'WARNING: unrecognized option value `{val}` for lambda_r_range_max! Please use numeric value. Currently lambda_r_range_max is set to be default value `{default_paramdict["lambda_r_range_max"]}`!')
             continue
         
         
         if opt in ('--lambda_r_range_k'):
             try:
                 paramdict['lambda_r_range_k'] = int(float(val))
                 
                 if paramdict['lambda_r_range_k'] < 1:
                     print(f'WARNING: option value `{paramdict["lambda_r_range_k"]}` for lambda_r_range_k < 1! Please use integer which >= 1. Currently lambda_r_range_k is set to be value `1`!')
                     paramdict['lambda_r_range_k'] = 1
             except:
-                print(f'WARNING: unrecognized option value `{val}` for lambda_r_range_k! Please use numeric value. Currently lambda_r_range_k is set to be default value `8`!')
+                print(f'WARNING: unrecognized option value `{val}` for lambda_r_range_k! Please use numeric value. Currently lambda_r_range_k is set to be default value `{default_paramdict["lambda_r_range_k"]}`!')
             continue
     
         
         if opt in ('--lambda_g'):
             if val.casefold() == 'none'.casefold():
                 paramdict['lambda_g'] = None
                 continue
             else:
                 try:
                     paramdict['lambda_g'] = float(val)
                     
                     if paramdict['lambda_g'] < 0:
-                        print(f'WARNING: negative option value `{paramdict["lambda_g"]}` for lambda_g! Please use non-negative value. Currently lambda_g is set to be default value `None`!')
-                        paramdict['lambda_g'] = None
+                        print(f'WARNING: negative option value `{paramdict["lambda_g"]}` for lambda_g! Please use non-negative value. Currently lambda_g is set to be default value `{default_paramdict["lambda_g"]}`!')
+                        paramdict['lambda_g'] = default_paramdict["lambda_g"]
                 except:
                     print(f'WARNING: unrecognized option value `{val}` for lambda_g! Please use numeric value or `none`. Currently lambda_g is set to be default value `None`!')
                 continue
         
         
         if opt in ('--lambda_g_range_min'):
             try:
                 paramdict['lambda_g_range_min'] = float(val)
                 
-                if paramdict['lambda_g_range_min'] <= 0:
-                    print(f'WARNING: non-positive option value `{paramdict["lambda_g_range_min"]}` for lambda_g_range_min! Please use positve value. Currently lambda_g_range_min is set to be default value `0.1`!')
-                    paramdict['lambda_g_range_min'] = 0.1
+                if paramdict['lambda_g_range_min'] < 0:
+                    print(f'WARNING: negative option value `{paramdict["lambda_g_range_min"]}` for lambda_g_range_min! Please use non-negative value. Currently lambda_g_range_min is set to be value `0`!')
+                    paramdict['lambda_g_range_min'] = 0
             except:
-                print(f'WARNING: unrecognized option value `{val}` for lambda_g_range_min! Please use numeric value. Currently lambda_g_range_min is set to be default value `0.1`!')
+                print(f'WARNING: unrecognized option value `{val}` for lambda_g_range_min! Please use numeric value. Currently lambda_g_range_min is set to be default value `{default_paramdict["lambda_g_range_min"]}`!')
             continue
         
         
         if opt in ('--lambda_g_range_max'):
             try:
                 paramdict['lambda_g_range_max'] = float(val)
                 # checking max value in the final check
             except:
-                print(f'WARNING: unrecognized option value `{val}` for lambda_g_range_max! Please use numeric value. Currently lambda_g_range_max is set to be default value `100`!')
+                print(f'WARNING: unrecognized option value `{val}` for lambda_g_range_max! Please use numeric value. Currently lambda_g_range_max is set to be default value `{default_paramdict["lambda_g_range_max"]}`!')
             continue
         
         
         if opt in ('--lambda_g_range_k'):
             try:
                 paramdict['lambda_g_range_k'] = int(float(val))
                 
                 if paramdict['lambda_g_range_k'] < 1:
                     print(f'WARNING: option value `{paramdict["lambda_g_range_k"]}` for lambda_g_range_k < 1! Please use integer which >= 1. Currently lambda_g_range_k is set to be value `1`!')
                     paramdict['lambda_g_range_k'] = 1
             except:
-                print(f'WARNING: unrecognized option value `{val}` for lambda_g_range_k! Please use numeric value. Currently lambda_g_range_k is set to be default value `8`!')
+                print(f'WARNING: unrecognized option value `{val}` for lambda_g_range_k! Please use numeric value. Currently lambda_g_range_k is set to be default value `{default_paramdict["lambda_g_range_k"]}`!')
             continue
         
         
         if opt in ('--use_cvae'):
             if val.casefold() == 'true'.casefold():
                 paramdict['use_cvae'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['use_cvae'] = False
             else:
-                print(f'WARNING: unrecognized option value `{val}` for use_cvae! Please use string of true or false. Currently use_cvae is set to be default value `True`!')
+                print(f'WARNING: unrecognized option value `{val}` for use_cvae! Please use string of true or false. Currently use_cvae is set to be default value `{default_paramdict["use_cvae"]}`!')
             continue
         
         
         if opt in ('--threshold'):
             try:
                 paramdict['threshold'] = float(val)
                 
                 if paramdict['threshold'] < 0:
                     print(f'WARNING: negative option value `{paramdict["threshold"]}` for thoreshold! Please use non-negative value. Currently threshold is set to be default value `0`!')
                     paramdict['threshold'] = 0
             except:
-                print(f'WARNING: unrecognized option value `{val}` for threshold! Please use numeric value. Currently threshold is set to be default value `0`!')
+                print(f'WARNING: unrecognized option value `{val}` for threshold! Please use numeric value. Currently threshold is set to be default value `{default_paramdict["threshold"]}`!')
             continue
         
         
         if opt in ('--n_hv_gene'):
             try:
                 paramdict['n_hv_gene'] = int(float(val))
                 
                 if paramdict['n_hv_gene'] < 0:
-                    print(f'WARNING: negative option value `{paramdict["n_hv_gene"]}` for n_hv_gene! Please use non-negative integer. Currently n_hv_gene is set to be default value `1,000`!')
-                    paramdict['n_hv_gene'] = 1000
+                    print(f'WARNING: negative option value `{paramdict["n_hv_gene"]}` for n_hv_gene! Please use non-negative integer. Currently n_hv_gene is set to be default value `{default_paramdict["n_hv_gene"]}`!')
+                    paramdict['n_hv_gene'] = default_paramdict["n_hv_gene"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for n_hv_gene! Please use numeric value. Currently n_hv_gene is set to be default value `1,000`!')
+                print(f'WARNING: unrecognized option value `{val}` for n_hv_gene! Please use numeric value. Currently n_hv_gene is set to be default value `{default_paramdict["n_hv_gene"]}`!')
             continue
         
         
         if opt in ('--n_marker_per_cmp'):
             try:
                 paramdict['n_marker_per_cmp'] = int(float(val))
                 
                 if paramdict['n_marker_per_cmp'] <= 0:
-                    print(f'WARNING: non-positive option value `{paramdict["n_marker_per_cmp"]}` for n_marker_per_cmp! Please use positve integer. Currently n_marker_per_cmp is set to be default value `30`!')
-                    paramdict['n_marker_per_cmp'] = 30
+                    print(f'WARNING: non-positive option value `{paramdict["n_marker_per_cmp"]}` for n_marker_per_cmp! Please use positve integer. Currently n_marker_per_cmp is set to be default value `{default_paramdict["n_marker_per_cmp"]}`!')
+                    paramdict['n_marker_per_cmp'] = default_paramdict["n_marker_per_cmp"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for n_marker_per_cmp! Please use numeric value. Currently n_marker_per_cmp is set to be default value `30`!')
+                print(f'WARNING: unrecognized option value `{val}` for n_marker_per_cmp! Please use numeric value. Currently n_marker_per_cmp is set to be default value `{default_paramdict["n_marker_per_cmp"]}`!')
             continue
         
         
         if opt in ('--pseudo_spot_min_cell'):
             try:
                 paramdict['pseudo_spot_min_cell'] = int(float(val))
                 
                 if paramdict['pseudo_spot_min_cell'] < 2:
-                    print(f'WARNING: invalid option value `{paramdict["pseudo_spot_min_cell"]}` for pseudo_spot_min_cell! Please use integer which >= 2. Currently pseudo_spot_min_cell is set to be default value `2`!')
+                    print(f'WARNING: invalid option value `{paramdict["pseudo_spot_min_cell"]}` for pseudo_spot_min_cell! Please use integer which >= 2. Currently pseudo_spot_min_cell is set to be value `2`!')
                     paramdict['pseudo_spot_min_cell'] = 2
             except:
-                print(f'WARNING: unrecognized option value `{val}` for pseudo_spot_min_cell! Please use numeric value. Currently pseudo_spot_min_cell is set to be default value `2`!')
+                print(f'WARNING: unrecognized option value `{val}` for pseudo_spot_min_cell! Please use numeric value. Currently pseudo_spot_min_cell is set to be default value `{default_paramdict["pseudo_spot_min_cell"]}`!')
             continue
         
         
         if opt in ('--pseudo_spot_max_cell'):
             try:
                 paramdict['pseudo_spot_max_cell'] = int(float(val))
                 # checking pseudo_spot_max_cell leaves to the final check
             except:
-                print(f'WARNING: unrecognized option value `{val}` for pseudo_spot_max_cell! Please use numeric value. Currently pseudo_spot_max_cell is set to be default value `8`!')
+                print(f'WARNING: unrecognized option value `{val}` for pseudo_spot_max_cell! Please use numeric value. Currently pseudo_spot_max_cell is set to be default value `{default_paramdict["pseudo_spot_max_cell"]}`!')
             continue
         
         
         if opt in ('--seq_depth_scaler'):
             try:
                 paramdict['seq_depth_scaler'] = int(float(val))
                 
                 if paramdict['seq_depth_scaler'] <= 0:
-                    print(f'WARNING: non-positive option value `{paramdict["seq_depth_scaler"]}` for seq_depth_scaler! Please use positve integer. Currently seq_depth_scaler is set to be default value `10,000`!')
-                    paramdict['seq_depth_scaler'] = 10000
+                    print(f'WARNING: non-positive option value `{paramdict["seq_depth_scaler"]}` for seq_depth_scaler! Please use positve integer. Currently seq_depth_scaler is set to be default value `{default_paramdict["seq_depth_scaler"]}`!')
+                    paramdict['seq_depth_scaler'] = default_paramdict["seq_depth_scaler"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for seq_depth_scaler! Please use numeric value. Currently seq_depth_scaler is set to be default value `10,000`!')
+                print(f'WARNING: unrecognized option value `{val}` for seq_depth_scaler! Please use numeric value. Currently seq_depth_scaler is set to be default value `{default_paramdict["seq_depth_scaler"]}`!')
             continue
         
         
         if opt in ('--cvae_input_scaler'):
             try:
                 paramdict['cvae_input_scaler'] = int(float(val))
                 
                 if paramdict['cvae_input_scaler'] <= 0:
-                    print(f'WARNING: non-positive option value `{paramdict["cvae_input_scaler"]}` for cvae_input_scaler! Please use positve integer. Currently cvae_input_scaler is set to be default value `10`!')
-                    paramdict['cvae_input_scaler'] = 10
+                    print(f'WARNING: non-positive option value `{paramdict["cvae_input_scaler"]}` for cvae_input_scaler! Please use positve integer. Currently cvae_input_scaler is set to be default value `{default_paramdict["cvae_input_scaler"]}`!')
+                    paramdict['cvae_input_scaler'] = default_paramdict["cvae_input_scaler"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for cvae_input_scaler! Please use numeric value. Currently cvae_input_scaler is set to be default value `10`!')
+                print(f'WARNING: unrecognized option value `{val}` for cvae_input_scaler! Please use numeric value. Currently cvae_input_scaler is set to be default value `{default_paramdict["cvae_input_scaler"]}`!')
             continue
         
         
         if opt in ('--cvae_init_lr'):
             try:
                 paramdict['cvae_init_lr'] = float(val)
                 
                 if paramdict['cvae_init_lr'] <= 0:
-                    print(f'WARNING: non-positive option value `{paramdict["cvae_init_lr"]}` for cvae_init_lr! Please use positve value. Currently cvae_init_lr is set to be default value `0.003`!')
-                    paramdict['cvae_init_lr'] = 0.003
+                    print(f'WARNING: non-positive option value `{paramdict["cvae_init_lr"]}` for cvae_init_lr! Please use positve value. Currently cvae_init_lr is set to be default value `{default_paramdict["cvae_init_lr"]}`!')
+                    paramdict['cvae_init_lr'] = default_paramdict["cvae_init_lr"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for cvae_init_lr! Please use numeric value. Currently cvae_init_lr is set to be default value `0.003`!')
+                print(f'WARNING: unrecognized option value `{val}` for cvae_init_lr! Please use numeric value. Currently cvae_init_lr is set to be default value `{default_paramdict["cvae_init_lr"]}`!')
             continue
         
         
         if opt in ('--redo_de'):
             if val.casefold() == 'true'.casefold():
                 paramdict['redo_de'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['redo_de'] = False
             else:
-                print(f'WARNING: unrecognized option value `{val}` for redo_de! Please use string of true or false. Currently redo_de is set to be default value `True`!')
+                print(f'WARNING: unrecognized option value `{val}` for redo_de! Please use string of true or false. Currently redo_de is set to be default value `{default_paramdict["redo_de"]}`!')
             continue
         
         
         if opt in ('--seed'):
             try:
                 paramdict['seed'] = int(float(val))
             except:
-                print(f'WARNING: unrecognized option value `{val}` for seed! Please use numeric value. Currently seed is set to be default value `383`!')
+                print(f'WARNING: unrecognized option value `{val}` for seed! Please use numeric value. Currently seed is set to be default value `{default_paramdict["seed"]}`!')
             continue
         
         
         if opt in ('--diagnosis'):
             if val.casefold() == 'true'.casefold():
                 paramdict['diagnosis'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['diagnosis'] = False
             else:
-                print(f'WARNING: unrecognized option value `{val}` for diagnosis! Please use string of true or false. Currently verbose is set to be default value `False`!')
+                print(f'WARNING: unrecognized option value `{val}` for diagnosis! Please use string of true or false. Currently verbose is set to be default value `{default_paramdict["diagnosis"]}`!')
             continue
         
         
         if opt in ('--verbose'):
             if val.casefold() == 'true'.casefold():
                 paramdict['verbose'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['verbose'] = False
             else:
-                print(f'WARNING: unrecognized option value `{val}` for verbose! Please use string of true or false. Currently verbose is set to be default value `True`!')
+                print(f'WARNING: unrecognized option value `{val}` for verbose! Please use string of true or false. Currently verbose is set to be default value `{default_paramdict["verbose"]}`!')
+            continue
+        
+        
+        if opt in ('--use_fdr'):
+            if val.casefold() == 'true'.casefold():
+                paramdict['use_fdr'] = True
+            elif val.casefold() == 'false'.casefold():
+                paramdict['use_fdr'] = False
+            else:
+                print(f'WARNING: unrecognized option value `{val}` for use_fdr! Please use string of true or false. Currently use_fdr is set to be default value `{default_paramdict["use_fdr"]}`!')
+            continue
+        
+        
+        if opt in ('--p_val_cutoff'):
+            try:
+                paramdict['p_val_cutoff'] = float(val)
+                
+                if paramdict['p_val_cutoff'] < 0:
+                    print(f'WARNING: negative option value `{paramdict["p_val_cutoff"]}` for p_val_cutoff! Please use non-negative value. Currently p_val_cutoff is set to be default value `{default_paramdict["p_val_cutoff"]}`!')
+                    paramdict['p_val_cutoff'] = default_paramdict["p_val_cutoff"]
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for p_val_cutoff! Please use numeric value. Currently p_val_cutoff is set to be default value `{default_paramdict["p_val_cutoff"]}`!')
+            continue
+        
+        
+        if opt in ('--fc_cutoff'):
+            try:
+                paramdict['fc_cutoff'] = float(val)
+                
+                if paramdict['fc_cutoff'] < 1:
+                    print(f'WARNING: option value `{paramdict["fc_cutoff"]}` for fc_cutoff < 1! Please use a value >= 1. Currently fc_cutoff is set to be value `1`!')
+                    paramdict['fc_cutoff'] = 1
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for fc_cutoff! Please use numeric value. Currently fc_cutoff is set to be default value `{default_paramdict["fc_cutoff"]}`!')
+            continue
+        
+        
+        if opt in ('--pct1_cutoff'):
+            try:
+                paramdict['pct1_cutoff'] = float(val)
+                
+                if paramdict['pct1_cutoff'] > 1:
+                    print(f'WARNING: option value `{paramdict["pct1_cutoff"]}` for pct1_cutoff > 1! Please use a value <= 1. Currently pct1_cutoff is set to be default value `{default_paramdict["pct1_cutoff"]}`!')
+                    paramdict['pct1_cutoff'] = default_paramdict["pct1_cutoff"]
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for pct1_cutoff! Please use numeric value. Currently pct1_cutoff is set to be default value `{default_paramdict["pct1_cutoff"]}`!')
+            continue
+        
+        
+        if opt in ('--pct2_cutoff'):
+            try:
+                paramdict['pct2_cutoff'] = float(val)
+                
+                if paramdict['pct2_cutoff'] < 0:
+                    print(f'WARNING: option value `{paramdict["pct2_cutoff"]}` for pct2_cutoff < 0! Please use a value >= 0. Currently pct2_cutoff is set to be default value `{default_paramdict["pct2_cutoff"]}`!')
+                    paramdict['pct2_cutoff'] = default_paramdict["pct2_cutoff"]
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for pct2_cutoff! Please use numeric value. Currently pct2_cutoff is set to be default value `{default_paramdict["pct2_cutoff"]}`!')
+            continue
+         
+        
+        if opt in ('--sortby_fc'):
+            if val.casefold() == 'true'.casefold():
+                paramdict['sortby_fc'] = True
+            elif val.casefold() == 'false'.casefold():
+                paramdict['sortby_fc'] = False
+            else:
+                print(f'WARNING: unrecognized option value `{val}` for sortby_fc! Please use string of true or false. Currently sortby_fc is set to be default value `{default_paramdict["sortby_fc"]}`!')
+            continue
+        
+        
+        if opt in ('--filter_cell'):
+            if val.casefold() == 'true'.casefold():
+                paramdict['filter_cell'] = True
+            elif val.casefold() == 'false'.casefold():
+                paramdict['filter_cell'] = False
+            else:
+                print(f'WARNING: unrecognized option value `{val}` for filter_cell! Please use string of true or false. Currently filter_cell is set to be default value `{default_paramdict["filter_cell"]}`!')
+            continue
+        
+        
+        if opt in ('--filter_gene'):
+            if val.casefold() == 'true'.casefold():
+                paramdict['filter_gene'] = True
+            elif val.casefold() == 'false'.casefold():
+                paramdict['filter_gene'] = False
+            else:
+                print(f'WARNING: unrecognized option value `{val}` for filter_gene! Please use string of true or false. Currently filter_gene is set to be default value `{default_paramdict["filter_gene"]}`!')
             continue
         
         
         if opt in ('--use_imputation'):
             if val.casefold() == 'true'.casefold():
                 paramdict['use_imputation'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['use_imputation'] = False
             else:
-                print(f'WARNING: unrecognized option value `{val}` for use_imputation! Please use string of true or false. Currently use_imputation is set to be default value `False`!')
+                print(f'WARNING: unrecognized option value `{val}` for use_imputation! Please use string of true or false. Currently use_imputation is set to be default value `{default_paramdict["use_imputation"]}`!')
             continue
         
         
         if opt in ('--diameter'):
             try:
                 paramdict['diameter'] = int(float(val))
                 
                 if paramdict['diameter'] <= 0:
-                    print(f'WARNING: option value `{paramdict["diameter"]}` for diameter <= 0! Please use integers > 0. Currently diameter is set to be default value `200`!')
-                    paramdict['diameter'] = 200
+                    print(f'WARNING: option value `{paramdict["diameter"]}` for diameter <= 0! Please use integers > 0. Currently diameter is set to be default value `{default_paramdict["diameter"]}`!')
+                    paramdict['diameter'] = default_paramdict["diameter"]
             except:
-                print(f'WARNING: unrecognized option value `{val}` for diameter! Please use numeric value. Currently diameter is set to be default value `200`!')
+                print(f'WARNING: unrecognized option value `{val}` for diameter! Please use numeric value. Currently diameter is set to be default value `{default_paramdict["diameter"]}`!')
             continue
         
         
         if opt in ('--impute_diameter'):
             
             ori_list = val.split(',')
             tmp_list = []
@@ -498,15 +655,15 @@
                         print(f'WARNING: option value `{tmp_val}` for imputate_diameter <= 0! Please use integers > 0. Currently this value will be ignored!')
                     else:
                         tmp_list.append(tmp_val)
                 except:
                     print(f'WARNING: unrecognized option value `{x.strip()}` for imputate_diameter! Please use numeric value. Currently this value will be ignored!')
                     
             if len(tmp_list) == 0:
-                print(f'WARNING: no valid value can be extracted from option value `{val}` for imputate_diameter! Please use one numeric value or an array of numeric values separated by ",". Currently impute_diameter is set to be default value `160,114,80`!')
+                print(f'WARNING: no valid value can be extracted from option value `{val}` for imputate_diameter! Please use one numeric value or an array of numeric values separated by ",". Currently impute_diameter is set to be default value `{",".join([str(x) for x in default_paramdict["impute_diameter"]])}`!')
             else:
                 paramdict['impute_diameter'] = tmp_list
         
             continue
     
     
     # 检查参数是否齐全
```

### Comparing `sdeper-1.0.3/src/preprocess.py` & `sdeper-1.1.0/src/preprocess.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,22 +18,23 @@
     4. filter genes and spots before GLRM modeling
     
     5. check datasets to avoid some mistakes
 """
 
 
 
+import numpy as np
 import pandas as pd
 from cvae import build_CVAE_whole
 from utils import run_DE_only
 from config import print
 
 
 
-def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, diagnosis):
+def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, filter_cell, filter_gene, diagnosis):
     '''
     preprocess files
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
@@ -59,56 +60,83 @@
         a scaler of scRNA-seq sequencing depth
     cvae_input_scaler : int
         maximum value of the scaled input for CVAE
     cvae_init_lr : float
         initial learning rate for training CVAE
     redo_de : bool
         whether to redo DE after CVAE transformation
+    use_fdr : bool
+        whether to use FDR adjusted p value for filtering and sorting
+    p_val_cutoff : float
+        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering
+    fc_cutoff : float
+        threshold of fold change (without log transform!) in marker genes filtering
+    pct1_cutoff : float
+        threshold of pct.1 in marker genes filtering
+    pct2_cutoff : float
+        threshold of pct.2 in marker genes filtering
+    sortby_fc : bool
+        whether to sort marker genes by fold change
     diagnosis : bool
         if True save more information to files for diagnosis CVAE and hyper-parameter selection
+    filter_cell : bool
+        whether to filter cells before DE
+    filter_gene : bool
+        whether to filter genes before DE
 
     Returns
     -------
     data : Dict
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.
-        celltype_names: a list of string of celltype names.
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.\n
+            celltype_names: a list of string of celltype names.
     '''
     
     # first determine whether to build CVAE
     if use_cvae:
         if ref_file is None or ref_anno_file is None:
             raise Exception('ERROR: building CVAE requires both reference scRNA-seq data and corresponding cell-type annotation specified! But at least one of them is not specified!')
             
-        print('######### First build CVAE... #########\n')
+        print('first build CVAE...\n')
         # build CVAE, and return the data dict including transformed spatial data and reference gene expression
-        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, diagnosis)
+        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
         
         # calculate squencing depth, sum also works on sparse dataframe
         N = spatial_df.sum(axis=1)
     
     else:
         
-        print('######### Building CVAE skipped... #########\n')
+        print('building CVAE skipped...\n')
         
         # to_dense has been depreated
         # read spatial dataframe into a sparse dataframe
         # the default mangle_dupe_cols=True will handle the duplicated columns
         spatial_df = pd.concat(chunk.astype('Sparse[int]') for chunk in pd.read_csv(spatial_file, index_col=0, chunksize=1e4))
         print(f'read spatial data from file {spatial_file}')
         print(f'total {spatial_df.shape[0]} spots; {spatial_df.shape[1]} genes\n')
         
         # check whether cell name are unique
         if len(set(spatial_df.index.to_list())) < spatial_df.shape[0]:
             raise Exception('spot barcodes in spatial data are not unique!')
+            
+        # filtering genes
+        if filter_gene:
+            # Remove genes present in <3 cells
+            pre_n_gene = spatial_df.shape[1]
+            spatial_df = spatial_df.loc[:, spatial_df.apply(lambda x: np.count_nonzero(x), axis=0) >= 3].copy()
+            if pre_n_gene > spatial_df.shape[1]:
+                print(f'filtering genes present in <3 spots: {pre_n_gene-spatial_df.shape[1]} genes removed\n')
+            else:
+                print('filtering genes present in <3 spots: No genes removed\n')
     
         # calculate squencing depth, sum also works on sparse dataframe
         N = spatial_df.sum(axis=1)
         
         new_markers = None
     
         
@@ -132,15 +160,15 @@
             print(f'from user specified marker gene expression use {len(marker_genes)} marker genes overlapped with spatial + scRNA-seq data')
             # if len(marker_genes) < spatial_df.shape[1]:
             #     print(f'{spatial_df.shape[1]-len(marker_genes)} genes in overlapped gene list between spatial and scRNA-seq data but not found in user provided marker gene expression: {", ".join(set(spatial_df.columns).difference(set(marker_genes)))}\n')
             
         else:
             # perform DE, return the marker gene expression. The identified markers but not in spatial data has already been removed
             print('no marker gene profile provided. Perform DE to get cell-type marker genes on scRNA-seq data...\n')
-            marker_df = run_DE_only(ref_file, ref_anno_file, spatial_df.columns.tolist(), n_marker_per_cmp, diagnosis)
+            marker_df = run_DE_only(ref_file, ref_anno_file, spatial_df.columns.tolist(), n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
             marker_genes = marker_df.columns
     
     else:
         
         print('use the marker genes derived from CVAE transformed scRNA-seq for downstream regression!')
         marker_genes = new_markers
```

### Comparing `sdeper-1.0.3/src/run_model.py` & `sdeper-1.1.0/src/run_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 
 def run_GLRM(data, lambda_r=None, weight_threshold=1e-3, lambda_g=None, estimate_gamma_g=True, n_jobs=1, threshold=0, diagnosis=False, verbose=False):
     """
     run GLRM, and fit coefficients
 
     Parameters
     ----------
-    data : a Dict contains all info need for modeling
-        X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).
-        Y: a 2-D numpy matrix of spatial gene expression (spots * genes).
-        A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.
-        N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.
-        non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.
-        spot_names: a list of string of spot barcodes. Only keep spots passed filtering.
-        gene_names: a list of string of gene symbols. Only keep actually used marker genes.
-        celltype_names: a list of string of celltype names.
+    data : Dict
+        a Dict contains all info need for modeling:
+            X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
+            Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
+            A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
+            N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
+            non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
+            spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
+            gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
+            celltype_names: a list of string of celltype names.
     lambda_r : float, optional
         strength for Adaptive Lasso penalty. The default is None, i.e. use cross-validation to determine optimal value
     weight_threshold : float, optional
         threshold for Adaptive Lasso weight. Theta values smaller than threshold value will be re-set. The default is 1e-3.
     lambda_g : float, optional
         edge weight for graph, and will affect the strength of Graph Laplacian constrain. The default is None, i.e. use cross-validation to determine optimal value
     estimate_gamma_g : bool, optional
@@ -51,19 +52,19 @@
     verbose : bool, optional
         if True, print variables in each ADMM loop. The default is True.
 
     Returns
     -------
     result : Dict
         estimated model coefficients, including (note theta dimension changed back to 2-D):
-            theta : celltype proportions (#spots * #celltypes)
-            e_alpha : spot-specific effect (1-D array with length #spot)
-            sigma2 : variance paramter of the lognormal distribution (float)
-            gamma_g : gene-specific platform effect for all genes (1-D array with length #gene)
-            theta_tilde : celltype proportions for Adaptive Lasso (#spots * #celltypes)
+            theta : celltype proportions (#spots * #celltypes)\n
+            e_alpha : spot-specific effect (1-D array with length #spot)\n
+            sigma2 : variance paramter of the lognormal distribution (float)\n
+            gamma_g : gene-specific platform effect for all genes (1-D array with length #gene)\n
+            theta_tilde : celltype proportions for Adaptive Lasso (#spots * #celltypes)\n
             theta_hat : celltype proportions for Graph Laplacian constrain (#spots * #celltypes)
     """
     
     assert(data['Y'].shape[1] == data['X'].shape[1])
     if data['A'] is not None:
         assert(data['A'].shape[0] == data['Y'].shape[0])
         assert(data['A'].shape[1] == data['Y'].shape[0])
```

### Comparing `sdeper-1.0.3/src/sdeper.egg-info/PKG-INFO` & `sdeper-1.1.0/src/sdeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.0.3
+Version: 1.1.0
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
@@ -18,22 +18,22 @@
 Requires-Dist: scipy==1.8.1
 Requires-Dist: pandas==1.4.3
 Requires-Dist: networkx==2.8.4
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: scikit-learn==1.1.1
 Requires-Dist: numba==0.55.2
 Requires-Dist: openpyxl==3.0.10
-Requires-Dist: tensorflow==2.9.1
+Requires-Dist: tensorflow-cpu==2.9.1
 Requires-Dist: scanpy==1.9.1
 Requires-Dist: scikit-misc==0.1.4
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: umap-learn==0.5.3
 Requires-Dist: distinctipy==1.2.2
-Requires-Dist: reportlab==3.6.12
-Requires-Dist: opencv-python==4.8.0.74
+Requires-Dist: reportlab==4.1.0
+Requires-Dist: opencv-python==4.6.0.66
 
 # SDePER
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
```

### Comparing `sdeper-1.0.3/src/sdeper.egg-info/SOURCES.txt` & `sdeper-1.1.0/src/sdeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

