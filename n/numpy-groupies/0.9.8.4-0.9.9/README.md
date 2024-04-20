# Comparing `tmp/numpy_groupies-0.9.8.4.tar.gz` & `tmp/numpy_groupies-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/numpy_groupies-0.9.8.4.tar", last modified: Mon Apr 23 16:50:45 2018, max compression
+gzip compressed data, was "dist/numpy_groupies-0.9.9.tar", last modified: Mon Jan 28 12:06:38 2019, max compression
```

## Comparing `numpy_groupies-0.9.8.4.tar` & `numpy_groupies-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/
--rw-rw-r--   0 michael   (1001) michael   (1001)    68611 2018-04-23 14:34:00.000000 numpy_groupies-0.9.8.4/versioneer.py
-drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/numpy_groupies/
--rw-rw-r--   0 michael   (1001) michael   (1001)     1484 2018-04-23 14:34:00.000000 numpy_groupies-0.9.8.4/numpy_groupies/__init__.py
--rw-rw-r--   0 michael   (1001) michael   (1001)    18456 2018-04-23 14:38:38.000000 numpy_groupies-0.9.8.4/numpy_groupies/_version.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     3702 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/aggregate_numpy_ufunc.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     8905 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/aggregate_weave.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     2330 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/aggregate_pandas.py
--rw-rw-r--   0 michael   (1001) michael   (1001)    11574 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/aggregate_numpy.py
--rw-rw-r--   0 michael   (1001) michael   (1001)    14587 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/aggregate_numba.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     4508 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/aggregate_purepy.py
--rw-rw-r--   0 michael   (1001) michael   (1001)    14354 2018-04-23 13:11:55.000000 numpy_groupies-0.9.8.4/numpy_groupies/utils_numpy.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     5635 2018-04-23 13:24:49.000000 numpy_groupies-0.9.8.4/numpy_groupies/utils.py
-drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/numpy_groupies.egg-info/
--rw-rw-r--   0 michael   (1001) michael   (1001)     1753 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/numpy_groupies.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1001) michael   (1001)        1 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/numpy_groupies.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1001) michael   (1001)       15 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/numpy_groupies.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1001) michael   (1001)      526 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/numpy_groupies.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1001) michael   (1001)     1753 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/PKG-INFO
--rw-rw-r--   0 michael   (1001) michael   (1001)      253 2018-04-23 16:50:45.000000 numpy_groupies-0.9.8.4/setup.cfg
--rw-rw-r--   0 michael   (1001) michael   (1001)     3467 2018-04-23 16:49:15.000000 numpy_groupies-0.9.8.4/setup.py
--rw-rw-r--   0 michael   (1001) michael   (1001)       60 2018-04-23 14:34:00.000000 numpy_groupies-0.9.8.4/MANIFEST.in
--rw-rw-r--   0 michael   (1001) michael   (1001)    15820 2018-04-23 16:16:41.000000 numpy_groupies-0.9.8.4/README.md
+drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/
+-rw-rw-r--   0 michael   (1001) michael   (1001)    68611 2018-04-23 14:34:00.000000 numpy_groupies-0.9.9/versioneer.py
+drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/numpy_groupies/
+-rw-rw-r--   0 michael   (1001) michael   (1001)     1484 2018-04-23 14:34:00.000000 numpy_groupies-0.9.9/numpy_groupies/__init__.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)    18456 2018-04-23 14:38:38.000000 numpy_groupies-0.9.9/numpy_groupies/_version.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)     3702 2018-04-23 13:24:49.000000 numpy_groupies-0.9.9/numpy_groupies/aggregate_numpy_ufunc.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)     8905 2018-04-23 13:24:49.000000 numpy_groupies-0.9.9/numpy_groupies/aggregate_weave.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)     2320 2018-10-14 15:35:08.000000 numpy_groupies-0.9.9/numpy_groupies/aggregate_pandas.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)    11574 2018-04-23 13:24:49.000000 numpy_groupies-0.9.9/numpy_groupies/aggregate_numpy.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)    14551 2018-10-14 15:33:11.000000 numpy_groupies-0.9.9/numpy_groupies/aggregate_numba.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)     4508 2018-04-23 13:24:49.000000 numpy_groupies-0.9.9/numpy_groupies/aggregate_purepy.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)    14354 2018-04-23 13:11:55.000000 numpy_groupies-0.9.9/numpy_groupies/utils_numpy.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)     5635 2018-04-23 13:24:49.000000 numpy_groupies-0.9.9/numpy_groupies/utils.py
+drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/numpy_groupies.egg-info/
+-rw-rw-r--   0 michael   (1001) michael   (1001)     1751 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/numpy_groupies.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1001) michael   (1001)        1 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/numpy_groupies.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1001) michael   (1001)       15 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/numpy_groupies.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1001) michael   (1001)      526 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/numpy_groupies.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1001) michael   (1001)     1751 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/PKG-INFO
+-rw-rw-r--   0 michael   (1001) michael   (1001)      253 2019-01-28 12:06:38.000000 numpy_groupies-0.9.9/setup.cfg
+-rw-rw-r--   0 michael   (1001) michael   (1001)     3467 2018-04-23 16:49:15.000000 numpy_groupies-0.9.9/setup.py
+-rw-rw-r--   0 michael   (1001) michael   (1001)       60 2018-04-23 14:34:00.000000 numpy_groupies-0.9.9/MANIFEST.in
+-rw-rw-r--   0 michael   (1001) michael   (1001)    15494 2018-10-14 15:51:38.000000 numpy_groupies-0.9.9/README.md
```

### Comparing `numpy_groupies-0.9.8.4/versioneer.py` & `numpy_groupies-0.9.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/__init__.py` & `numpy_groupies-0.9.9/numpy_groupies/__init__.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/_version.py` & `numpy_groupies-0.9.9/numpy_groupies/_version.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/aggregate_numpy_ufunc.py` & `numpy_groupies-0.9.9/numpy_groupies/aggregate_numpy_ufunc.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/aggregate_weave.py` & `numpy_groupies-0.9.9/numpy_groupies/aggregate_weave.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/aggregate_pandas.py` & `numpy_groupies-0.9.9/numpy_groupies/aggregate_pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     if func == "sort":
         grouped = df.groupby('group_idx', sort=True)
     else:
         grouped = df.groupby('group_idx', sort=False).aggregate(func, **kwargs)
 
     dtype = check_dtype(dtype, getattr(func, '__name__', funcname), a, size)
     if funcname.startswith('cum'):
-        ret = grouped.as_matrix()[:, 0]
+        ret = grouped.values[:, 0]
     else:
         ret = np.full(size, fill_value, dtype=dtype)
-        ret[grouped.index] = grouped.as_matrix()[:, 0]
+        ret[grouped.index] = grouped.values[:, 0]
     return ret
 
 
 _supported_funcs = 'sum prod all any min max mean var std first last cumsum cumprod cummax cummin'.split()
 _impl_dict = {fn: partial(_wrapper, func=fn) for fn in _supported_funcs}
 _impl_dict.update(('nan' + fn, partial(_wrapper, func=fn))
                   for fn in _supported_funcs
```

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/aggregate_numpy.py` & `numpy_groupies-0.9.9/numpy_groupies/aggregate_numpy.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/aggregate_numba.py` & `numpy_groupies-0.9.9/numpy_groupies/aggregate_numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 if ri < 0:
                     raise ValueError("negative indices not supported")
                 if ri >= size:
                     raise ValueError("one or more indices in group_idx are too large")
                 val = valgetter(a, i)
                 inner(ri, val, ret, counter, mean)
                 outersetter(outer, i, ret[ri])
-        return nb.njit(_loop, nogil=True, cache=True)
+        return nb.njit(_loop, nogil=True)
 
     @staticmethod
     def _valgetter(a, i):
         return a[i]
 
     @staticmethod
     def _valgetter_scalar(a, i):
@@ -203,15 +203,15 @@
         # Deal with ndimensional indexing
         if ndim_idx > 1:
             ret = ret.reshape(size, order=order)
         return ret
 
     def callable(self, nans=False):
         """Compile a jitted function and loop it over the sorted data."""
-        jitfunc = nb.njit(self.func, nogil=True, cache=True)
+        jitfunc = nb.njit(self.func, nogil=True)
 
         def _loop(sortidx, group_idx, a, ret):
             size = len(ret)
             group_idx_srt = group_idx[sortidx]
             a_srt = a[sortidx]
 
             indices = step_indices(group_idx_srt)
@@ -219,15 +219,15 @@
                 start_idx, stop_idx =  indices[i], indices[i + 1]
                 ri = group_idx_srt[start_idx]
                 if ri < 0:
                     raise ValueError("negative indices not supported")
                 if ri >= size:
                     raise ValueError("one or more indices in group_idx are too large")
                 ret[ri] = jitfunc(a_srt[start_idx:stop_idx])
-        return nb.njit(_loop, nogil=True, cache=True)
+        return nb.njit(_loop, nogil=True)
 
 
 class Sum(AggregateOp):
     forced_fill_value = 0
 
     @staticmethod
     def _inner(ri, val, ret, counter, mean):
```

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/aggregate_purepy.py` & `numpy_groupies-0.9.9/numpy_groupies/aggregate_purepy.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/utils_numpy.py` & `numpy_groupies-0.9.9/numpy_groupies/utils_numpy.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies/utils.py` & `numpy_groupies-0.9.9/numpy_groupies/utils.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies.egg-info/PKG-INFO` & `numpy_groupies-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: numpy-groupies
-Version: 0.9.8.4
+Name: numpy_groupies
+Version: 0.9.9
 Summary: Optimised tools for group-indexing operations: aggregated sum and more.
 Home-page: https://github.com/ml31415/numpy-groupies
 Author: @ml31415 and @d1manson
 Author-email: npgroupies@occam.com.ua
 License: BSD
 Download-URL: https://github.com/ml31415/numpy-groupies/archive/master.zip
 Description-Content-Type: UNKNOWN
```

### Comparing `numpy_groupies-0.9.8.4/numpy_groupies.egg-info/SOURCES.txt` & `numpy_groupies-0.9.9/numpy_groupies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/PKG-INFO` & `numpy_groupies-0.9.9/numpy_groupies.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: numpy_groupies
-Version: 0.9.8.4
+Name: numpy-groupies
+Version: 0.9.9
 Summary: Optimised tools for group-indexing operations: aggregated sum and more.
 Home-page: https://github.com/ml31415/numpy-groupies
 Author: @ml31415 and @d1manson
 Author-email: npgroupies@occam.com.ua
 License: BSD
 Download-URL: https://github.com/ml31415/numpy-groupies/archive/master.zip
 Description-Content-Type: UNKNOWN
```

### Comparing `numpy_groupies-0.9.8.4/setup.py` & `numpy_groupies-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `numpy_groupies-0.9.8.4/README.md` & `numpy_groupies-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -186,49 +186,51 @@
 
 Below we are using `500,000` indices uniformly picked from `[0, 1000)`. The values of `a` are uniformly picked from 
 the interval `[0,1)`, with anything less than `0.2` then set to 0 (in order to serve as falsy values in boolean operations). 
 For `nan-` operations another 20% of the values are set to nan, leaving the remainder on the interval `[0.2,0.8)`.
 
 The benchmarking results are given in ms for an i7-7560U running at 2.40GHz:
 ```text
-function         ufunc         numpy         numba         weave        pandas
-------------------------------------------------------------------------------
-sum             29.939         1.452         0.912         1.186        16.274
-prod            30.729        30.353         0.909         1.188        16.016
-amin            29.871        29.899         0.969         1.179        16.470
-amax            30.023        29.806         1.018         1.257        15.815
-len             28.982         1.262         0.781         1.085        16.378
-all             33.745         3.421         0.987         1.250        93.688
-any             33.027         5.097         1.033         1.225        93.393
-anynan          29.499         2.473         0.989         1.195        84.557
-allnan          30.067         4.068         0.978         1.215        74.876
-mean              ----         2.110         0.983         1.205         9.522
-std               ----         4.709         1.038         1.219        43.495
-var               ----         3.546         1.026         1.224        43.093
-first             ----         1.529         0.997         0.987         8.602
-last              ----         1.267         0.692         0.879         9.038
-argmax            ----        29.894         0.906          ----       141.851
-argmin            ----        32.924         0.868          ----       138.898
-cumsum            ----       129.279         1.169          ----         7.830
-cumprod           ----          ----         1.268          ----         7.990
-cummax            ----          ----         1.198          ----         8.385
-cummin            ----          ----         1.147          ----         8.286
-nansum            ----         4.592         1.662         1.180         9.431
-nanprod           ----        27.126         1.701         1.184         9.256
-nanmin            ----        27.436         1.834         1.220         9.171
-nanmax            ----        27.510         1.891         1.263         9.264
-nanlen            ----         4.650         1.588         1.158        10.634
-nanall            ----         6.790         1.781         1.279        79.503
-nanany            ----         7.900         1.721         1.249        83.260
-nanmean           ----         5.163         1.689         1.316         9.286
-nanvar            ----         6.729         1.890         1.517        44.632
-nanstd            ----         7.091         1.882         1.484        44.752
-nanfirst          ----         4.844         1.884         1.098        11.124
-nanlast           ----         4.857         1.589         1.041        11.132
-Linux(x86_64), Python 2.7.12, Numpy 1.14.1, Numba 0.37.0, Pandas 0.22.0
+function         ufunc         numpy         numba         weave
+-----------------------------------------------------------------
+sum              29.738         1.454         0.901         1.176
+prod             29.552        29.575         0.905         1.162
+amin             29.944        29.850         0.979         1.169
+amax             29.943        29.956         1.009         1.201
+len              28.865         1.250         0.748         1.053
+all              34.013         3.962         0.995         1.195
+any              32.913         6.690         1.023         1.189
+anynan           28.956         2.551         0.961         1.210
+allnan           29.966         5.943         0.924         1.204
+mean               ----         2.302         0.843         1.030
+std                ----         5.587         1.015         1.210
+var                ----         5.635         1.004         1.205
+first              ----         1.586         0.977         0.994
+last               ----         1.335         0.665         0.887
+argmax             ----        29.734         0.903          ----
+argmin             ----        33.152         0.868          ----
+nansum             ----         4.576         1.633         1.176
+nanprod            ----        26.832         1.618         1.186
+nanmin             ----        27.198         1.852         1.211
+nanmax             ----        27.194         1.786         1.252
+nanlen             ----         4.602         1.611         1.948
+nanall             ----         8.512         1.706         1.237
+nanany             ----         9.492         1.719         1.245
+nanmean            ----         5.089         1.669         1.282
+nanvar             ----         8.783         1.815         1.485
+nanstd             ----         8.771         1.805         1.482
+nanfirst           ----         4.899         1.851         1.095
+nanlast            ----         4.834         1.625         1.051
+cumsum             ----       132.572         1.161          ----
+cumprod            ----          ----         1.179          ----
+cummax             ----          ----         1.146          ----
+cummin             ----          ----         1.114          ----
+arbitrary          ----       217.585        72.019          ----
+sort               ----       237.604          ----          ----
+Linux(x86_64), Python 2.7.12, Numpy 1.15.2, Numba 0.40.1
 
 ```
 
 
 ## Development
 This project was started by @ml31415 and the `numba` and `weave` implementations are by him. The pure 
 python and `numpy` implementations were written by @d1manson.
```

