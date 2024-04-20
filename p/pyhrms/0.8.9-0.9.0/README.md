# Comparing `tmp/pyhrms-0.8.9.zip` & `tmp/pyhrms-0.9.0.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 101898 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-14 23:13 pyhrms-0.8.9/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms/
--rw-r--r--  2.0 unx    30087 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/PKG-INFO
--rwx------  2.0 unx      927 b- defN 24-Apr-14 23:08 pyhrms-0.8.9/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/setup.cfg
--rwx------  2.0 unx    25541 b- defN 24-Apr-14 23:12 pyhrms-0.8.9/README.rst
--rw-r--r--  2.0 unx    30087 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms.egg-info/requires.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-14 23:13 pyhrms-0.8.9/pyhrms.egg-info/dependency_links.txt
--rwx------  2.0 unx   308332 b- defN 24-Apr-14 23:07 pyhrms-0.8.9/pyhrms/pyhrms.py
--rwx------  2.0 unx     2199 b- defN 24-Apr-14 23:07 pyhrms-0.8.9/pyhrms/__init__.py
-14 files, 397604 bytes uncompressed, 99976 bytes compressed:  74.9%
+Zip file size: 101775 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-20 23:30 pyhrms-0.9.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms/
+-rw-r--r--  2.0 unx    29957 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/PKG-INFO
+-rwx------  2.0 unx      927 b- defN 24-Apr-20 23:18 pyhrms-0.9.0/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/setup.cfg
+-rwx------  2.0 unx    25411 b- defN 24-Apr-20 23:29 pyhrms-0.9.0/README.rst
+-rw-r--r--  2.0 unx    29957 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms.egg-info/requires.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-20 23:30 pyhrms-0.9.0/pyhrms.egg-info/dependency_links.txt
+-rwx------  2.0 unx   308434 b- defN 24-Apr-20 23:17 pyhrms-0.9.0/pyhrms/pyhrms.py
+-rwx------  2.0 unx     2199 b- defN 24-Apr-20 23:18 pyhrms-0.9.0/pyhrms/__init__.py
+14 files, 397316 bytes uncompressed, 99853 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: pyhrms-0.8.9/
+Filename: pyhrms-0.9.0/
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms.egg-info/
+Filename: pyhrms-0.9.0/pyhrms.egg-info/
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms/
+Filename: pyhrms-0.9.0/pyhrms/
 Comment: 
 
-Filename: pyhrms-0.8.9/PKG-INFO
+Filename: pyhrms-0.9.0/PKG-INFO
 Comment: 
 
-Filename: pyhrms-0.8.9/setup.py
+Filename: pyhrms-0.9.0/setup.py
 Comment: 
 
-Filename: pyhrms-0.8.9/setup.cfg
+Filename: pyhrms-0.9.0/setup.cfg
 Comment: 
 
-Filename: pyhrms-0.8.9/README.rst
+Filename: pyhrms-0.9.0/README.rst
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms.egg-info/PKG-INFO
+Filename: pyhrms-0.9.0/pyhrms.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms.egg-info/SOURCES.txt
+Filename: pyhrms-0.9.0/pyhrms.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms.egg-info/requires.txt
+Filename: pyhrms-0.9.0/pyhrms.egg-info/requires.txt
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms.egg-info/top_level.txt
+Filename: pyhrms-0.9.0/pyhrms.egg-info/top_level.txt
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms.egg-info/dependency_links.txt
+Filename: pyhrms-0.9.0/pyhrms.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms/pyhrms.py
+Filename: pyhrms-0.9.0/pyhrms/pyhrms.py
 Comment: 
 
-Filename: pyhrms-0.8.9/pyhrms/__init__.py
+Filename: pyhrms-0.9.0/pyhrms/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pyhrms-0.8.9/PKG-INFO` & `pyhrms-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyhrms
-Version: 0.8.9
+Version: 0.9.0
 Summary: A powerful GC/LC-HRMS data analysis tool
 Home-page: https://github.com/WangRui5/PyHRMS.git
 Author: Wang Rui
 Author-email: wtrt7009@gmail.com
 License: UNKNOWN
 Description: PyHRMS: Tools For working with High Resolution Mass Spectrometry (HRMS) data in Environmental Science
         =====================================================================================================
@@ -15,23 +15,23 @@
         
         Contributer: Rui Wang
         ======================
         First release date: Nov.15.2021
         
         Update
         ======
-        Apr.14.2024: pyhrms 0.8.9 new features:
+        Apr.20.2024: pyhrms 0.9.0 new features:
         
-            * Corrected issues in rt_matching and ms2_matching to prevent errors;
+            * Modified evaluate_ms to retain five decimal places;
         
-            * Updated gen_DDA_ms2_df to include isotope information
+            * Fixed issue where peak_checking_area returned zeros;
         
-            * Improved the peak_checking_area_precursor_frag_swath function with various bug fixes.
+            * Updated gen_DDA_ms2_df;
         
-            * Enhanced the swath_process function with new features to mark isotopes and adducts
+            * Resolved issues in post_filter.
         
         pyhrms can be installed and import as following:
         
         .. code-block:: python
         
             pip install pyhrms
```

## Comparing `pyhrms-0.8.9/setup.py` & `pyhrms-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme_file():
     with open('README.rst') as rf:
         return rf.read()
 
 setuptools.setup(
     name = 'pyhrms',
-    version = '0.8.9',
+    version = '0.9.0',
     author = 'Wang Rui',
     author_email = 'wtrt7009@gmail.com',
     url = 'https://github.com/WangRui5/PyHRMS.git',
     description = 'A powerful GC/LC-HRMS data analysis tool',
     long_description = readme_file(),
     packages = setuptools.find_packages(),
     install_requires = ['numpy>=1.19.2','pandas>=1.3.3'
```

## Comparing `pyhrms-0.8.9/README.rst` & `pyhrms-0.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 Contributer: Rui Wang
 ======================
 First release date: Nov.15.2021
 
 Update
 ======
-Apr.14.2024: pyhrms 0.8.9 new features:
+Apr.20.2024: pyhrms 0.9.0 new features:
 
-    * Corrected issues in rt_matching and ms2_matching to prevent errors;
+    * Modified evaluate_ms to retain five decimal places;
 
-    * Updated gen_DDA_ms2_df to include isotope information
+    * Fixed issue where peak_checking_area returned zeros;
 
-    * Improved the peak_checking_area_precursor_frag_swath function with various bug fixes.
+    * Updated gen_DDA_ms2_df;
 
-    * Enhanced the swath_process function with new features to mark isotopes and adducts
+    * Resolved issues in post_filter.
 
 pyhrms can be installed and import as following:
 
 .. code-block:: python
 
     pip install pyhrms
```

## Comparing `pyhrms-0.8.9/pyhrms.egg-info/PKG-INFO` & `pyhrms-0.9.0/pyhrms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyhrms
-Version: 0.8.9
+Version: 0.9.0
 Summary: A powerful GC/LC-HRMS data analysis tool
 Home-page: https://github.com/WangRui5/PyHRMS.git
 Author: Wang Rui
 Author-email: wtrt7009@gmail.com
 License: UNKNOWN
 Description: PyHRMS: Tools For working with High Resolution Mass Spectrometry (HRMS) data in Environmental Science
         =====================================================================================================
@@ -15,23 +15,23 @@
         
         Contributer: Rui Wang
         ======================
         First release date: Nov.15.2021
         
         Update
         ======
-        Apr.14.2024: pyhrms 0.8.9 new features:
+        Apr.20.2024: pyhrms 0.9.0 new features:
         
-            * Corrected issues in rt_matching and ms2_matching to prevent errors;
+            * Modified evaluate_ms to retain five decimal places;
         
-            * Updated gen_DDA_ms2_df to include isotope information
+            * Fixed issue where peak_checking_area returned zeros;
         
-            * Improved the peak_checking_area_precursor_frag_swath function with various bug fixes.
+            * Updated gen_DDA_ms2_df;
         
-            * Enhanced the swath_process function with new features to mark isotopes and adducts
+            * Resolved issues in post_filter.
         
         pyhrms can be installed and import as following:
         
         .. code-block:: python
         
             pip install pyhrms
```

## Comparing `pyhrms-0.8.9/pyhrms/pyhrms.py` & `pyhrms-0.9.0/pyhrms/pyhrms.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,15 +859,15 @@
         iso_info_s1 = (iso_info_s / iso_info_s.values.max()).sort_index().round(3)
         iso_info_s2 = iso_info_s1[iso_info_s1 > 0.015].to_dict()
         return iso_info_s2
 
 
 def isotope_score(iso_info, formula, mode='pos', i_threshold=2, error=0.015):
     """
-    Calculate the isotope matching score based on the observed isotope distribution and 
+    Calculate the isotope matching score based on the observed isotope distribution and
     the theoretical distribution for a given molecular formula.
 
     Args:
         iso_info (dict): The observed isotope distribution.
         formula (str): The molecular formula.
         mode (str): Analysis mode - 'pos' for positive, 'neg' for negative. Defaults to 'pos'.
         i_threshold (float): The intensity threshold for theoretical isotope distribution. Defaults to 2.
@@ -955,20 +955,20 @@
 
             target_list = x[intersect_index]
 
             half_mz_left = target_list[np.argwhere(target_list < mz_obs)[-1]][0]
             half_mz_right = target_list[np.argwhere(target_list > mz_obs)[0]][0]
 
             resolution = int(mz_obs / (half_mz_right - half_mz_left))
-            mz_opt = round(half_mz_left + (half_mz_right - half_mz_left) / 2, 4)
+            mz_opt = round(half_mz_left + (half_mz_right - half_mz_left) / 2, 5)
             error1 = round((mz_obs - mz_exp) / mz_exp * 1000000, 1)
             error2 = round((mz_opt - mz_exp) / mz_exp * 1000000, 1)
         except:
             mz_obs, error1, mz_opt, error2, resolution = mz_exp, 0, 0, 0, 0
-    return round(mz_obs, 4), error1, mz_opt, error2, resolution
+    return round(mz_obs, 5), error1, mz_opt, error2, resolution
 
 
 def target_spec(spec, target_mz, width=0.04):
     """
     Narrow the spec to a certain mass range centered around a target mz.
 
     Args:
@@ -1081,19 +1081,19 @@
 
     if profile is True:
         peaks_index = [[i, scipy.signal.find_peaks(ms1[i].i.copy())[0]]
                        for i in tqdm(range(len(ms1)), desc=f'{message}Loading Data', leave=False, colour='Green')]
         raw_info_centroid = {
             round(ms1[i].scan_time[0], 3): pd.Series(
                 data=ms1[i].i[peaks],
-                index=ms1[i].mz[peaks].round(4),
+                index=ms1[i].mz[peaks].round(5),
                 name=round(ms1[i].scan_time[0], 3)) for i, peaks in
             tqdm(peaks_index, desc=f'{message}Convert to Centroid', leave=False, colour='Green')}
         raw_info_profile = {round(ms1[i].scan_time[0], 3):
-                                pd.Series(data=ms1[i].i, index=ms1[i].mz.round(4), name=round(ms1[i].scan_time[0], 3))
+                                pd.Series(data=ms1[i].i, index=ms1[i].mz.round(5), name=round(ms1[i].scan_time[0], 3))
                             for i in tqdm(range(len(ms1)), desc=f'{message}Recording raw profile info', leave=False,
                                           colour='Green')}
         if orbi is True:
             data = []
             for k, v in tqdm(raw_info_centroid.items(), desc=f'{message}Checking orbitrap data', leave=False,
                              colour='Green'):
                 df = v.to_frame().reset_index()
@@ -1104,15 +1104,15 @@
                 data.append(s)
         else:
             data = [pd.Series(data=v.values, index=v.index.values.round(3), name=v.name) for k, v in
                     tqdm(raw_info_centroid.items(), leave=False, desc=f'{message}Appending centroid data',
                          colour='Green')]
     else:
         raw_info_centroid = {round(ms1[i].scan_time[0], 3): pd.Series(
-            data=ms1[i].i, index=ms1[i].mz.round(4), name=round(ms1[i].scan_time[0], 3)) for i in
+            data=ms1[i].i, index=ms1[i].mz.round(5), name=round(ms1[i].scan_time[0], 3)) for i in
             tqdm(range(len(ms1)), desc=f'{message}Loading Data', leave=False, colour='Green')}
         if orbi is True:
             data = []
             for k, v in tqdm(raw_info_centroid.items(), desc=f'{message}Checking orbitrap data', leave=False,
                              colour='Green'):
                 df = v.to_frame().reset_index()
                 df = df.sort_values(['index', k])
@@ -1883,28 +1883,28 @@
         centroid_data = pd.Series(name=profile_data.name, dtype='float64')
 
     return centroid_data
 
 
 def gen_DDA_ms2_df(ms1, ms2, i_threshold=0, profile=True, opt=False, more_info=False, message=''):
     """
-    Generates a DataFrame from DDA MS2 data with detailed information on retention times, 
+    Generates a DataFrame from DDA MS2 data with detailed information on retention times,
     precursors, fragments, and additional metrics depending on specified options.
 
     Args:
         ms1 (list): List of MS1 scans.
         ms2 (list): List of MS2 scans.
         i_threshold (float): Minimum intensity threshold for peak consideration. Defaults to 0.
         profile (bool): Indicates if data is in profile mode (True) or centroid mode (False). Defaults to True.
         opt (bool): If True, performs optimization on mass data. Defaults to False.
         more_info (bool): If True, additional information from MS1 is appended to the DataFrame. Defaults to False.
         message (str): Message to display during extended information gathering. Defaults to an empty string.
 
     Returns:
-        pandas.DataFrame: Contains columns for retention time (rt), precursor m/z, fragments (frag), 
+        pandas.DataFrame: Contains columns for retention time (rt), precursor m/z, fragments (frag),
                           intensity, collision energy, mode of ionization, scan index, MS2 spectra,
                           isotope distribution, and optionally optimized fragment m/z and MS1 data.
 
     Note:
         The function supports dynamic generation of data based on the `profile`, `opt`, and `more_info` flags,
         adapting the output DataFrame accordingly. The function requires tqdm and pandas libraries for execution.
     """
@@ -1964,15 +1964,15 @@
         frags.append(frag)
         intensities.append(list(s.values))
 
     # Create a DataFrame with precursor, rt, fragment, intensity, collision energy, mode, and scan index data
     DDA_df = pd.DataFrame(
         [precursors, rts, collision_energies, frags, intensities, modes, scan_indices, s_all, iso_info],
         index=['precursor', 'rt', 'collision energy', 'frag',
-               'intensity', 'mode', 'scan_index', 'MS2_spectra', 'iso_distribution']).T
+               'ms2_intensities', 'mode', 'scan_index', 'MS2_spectra', 'iso_distribution']).T
 
     # Optimize mass if required
     if profile and opt:
         mz_opt_all = []
         for i in tqdm(range(len(DDA_df)), desc='Optimizing mass'):
             frag = DDA_df.loc[i].frag
             x = DDA_df.loc[i].scan_index
@@ -1991,22 +1991,22 @@
                 if (ms1[j].scan_time[0] >= rt) & (j > 1):
                     spec = pd.Series(data=ms1[j - 1].i, index=ms1[j - 1].mz)
                     if profile is True:
                         spec1 = target_spec(spec, precursor, width=0.2)
 
                         intensity = spec1.max()
                         mz_obs, error1, mz_opt, error2, resolution = evaluate_ms(spec1, precursor)
-                        DDA_df.loc[i, 'ms1_intensity'] = intensity
+                        DDA_df.loc[i, 'intensity'] = intensity
                         DDA_df.loc[i, 'ms1_obs'] = mz_obs
 
                     else:
                         spec1 = target_spec(spec, precursor, width=0.2)
                         intensity = spec1.max()
                         ms1_obs = spec1.index[np.argmin(abs(spec1.index - precursor))]
-                        DDA_df.loc[i, 'ms1_intensity'] = intensity
+                        DDA_df.loc[i, 'intensity'] = intensity
                         DDA_df.loc[i, 'ms1_obs'] = ms1_obs
 
                     break
 
     return DDA_df
 
 
@@ -2471,15 +2471,18 @@
         p_values_columns = [i for i in df.columns if 'p_value' in i]
 
         for fold_change1 in fold_change_columns:
             df = df[df[fold_change1] > fold_change]
         for p_value1 in p_values_columns:
             df = df[df[p_value1] < p_value].reset_index(drop=True)
         # other parameters
-        df = df[(df.intensity > i_threshold) & (df.area > area_threshold)].reset_index(drop=True)
+        if 'intensity' in df.columns:
+            df = df[(df.intensity > i_threshold)].reset_index(drop=True)
+        if 'area' in df.columns:
+            df = df[(df.area > area_threshold)].reset_index(drop=True)
 
         df.to_excel(files[i].replace('.xlsx', '_filter.xlsx'))
 
 
 def summarize_results(df, suspect_list=None, db_toxicity=None,
                       rt_matched_column='rt_match_result', matched_DDA_column='match_result_DDA',
                       matched_DIA_column='match_result_DIA', best_matched_DDA_column='best_results_DDA',
@@ -3030,15 +3033,15 @@
         df = pd.read_excel(file)
         df1 = remove_adducts(df, mode=mode)
         df1.to_excel(file.replace('.xlsx', '_removing_adducts.xlsx'))
 
 
 def DDA_to_DIA_result(path, company, profile):
     """
-  This function processes DDA (Data-Dependent Acquisition) data in mzML format 
+  This function processes DDA (Data-Dependent Acquisition) data in mzML format
   and integrates the results into existing Excel files containing unique company information.
 
   Args:
       path (str): Path to the directory containing mzML files and Excel files.
       company (str): Name of the company associated with the data.
       profile (str): Profile to be used for DDA data processing.
 
@@ -3067,44 +3070,44 @@
                     df_frag = df2[(df2['precursor'] >= mz - 0.015) & (df2['precursor'] <= mz + 0.015)
                                   & (df2['rt'] >= rt - 0.1) & (df2['rt'] <= rt + 0.1)]
                     if len(df_frag) == 0:
                         df1.loc[i, 'frag_DDA'] = str([])
                     else:
                         s_ms2_info = df_frag.iloc[np.argmin(abs(df_frag['rt'].values - rt))]
                         ms2_rt = df_frag['rt'].values[np.argmin(abs(df_frag['rt'].values - rt))]
-                        s_ms2 = pd.Series(data=s_ms2_info['intensity'], index=s_ms2_info['frag'], name=ms2_rt)
+                        s_ms2 = pd.Series(data=s_ms2_info['ms2_intensities'], index=s_ms2_info['frag'], name=ms2_rt)
                         df1.loc[i, 'frag_DDA'] = str(list(s_ms2.index))
                         df1.loc[i, 'MS2_spec_DDA'] = str(s_ms2.astype(int))
                 df1.to_excel(file_excel)
 
 
 """
 ========================================================================================================
 2. Swath data process
 ========================================================================================================
 """
 
 
 def swath_window_checking(file, precursor_ion_start_mass=99.5, mz_overlap=1):
     """
-    Analyzes the precursor ion windows in a given mzML file. This function separates MS1 and MS2 scans, 
-    determines unique precursor ions, and calculates the mass spectrum range for each precursor ion window 
+    Analyzes the precursor ion windows in a given mzML file. This function separates MS1 and MS2 scans,
+    determines unique precursor ions, and calculates the mass spectrum range for each precursor ion window
     based on the starting mass and overlap values.
 
     Parameters:
     - file (str): Path to the mzML file containing mass spectrometry data.
     - precursor_ion_start_mass (float, optional): Specifies the initial mass value for the sequential mass window in ion analysis.
       Defaults to 99.5.
     - mz_overlap (float, optional): Defines the amount of overlap between consecutive MS2 windows in mass units. Defaults to 1.
 
     Returns:
     - dict: A dictionary mapping each precursor ion to its corresponding mass spectrum range [start, end].
 
     Note:
-    The function first calculates the window size for the initial precursor ion manually and then iteratively for the remaining ions, 
+    The function first calculates the window size for the initial precursor ion manually and then iteratively for the remaining ions,
     considering the specified overlap.
     """
 
     ms1, ms2 = sep_scans(file, 'AB')  # 分离ms1和ms2
     # 1. 获得所有selected precursors
     all_precursors = []
     for scan in ms2:
@@ -3708,15 +3711,15 @@
         # revise 3. 映射到raw_index_info
         raw_index_info['peak area'] = raw_index_info['short_index'].map(peak_area['peak_area'])
         if sn_info is True:
             raw_index_info['peak_area_S/N'] = raw_index_info['short_index'].map(peak_area['peak_area_S/N'])
 
         # 解决nan的情况
         raw_index_info['peak_area_S/N'] = raw_index_info['peak_area_S/N'].fillna(0)
-        raw_index_info['peak area'] = raw_index_info['peak area'].fillna(0)
+        raw_index_info['peak area'] = raw_index_info['peak area'].fillna(1)
         peak_area_all.append(raw_index_info)
     return pd.concat(peak_area_all)
 
 
 def gen_ref_swath(files_excel, rt_error=0.1, ms1_error=0.01, ms2_error=0.015):
     """
     Generates a reference list from a set of data points considering the given rt, ms1, and ms2 error tolerances.
@@ -4251,43 +4254,43 @@
 4. FT-ICRMS data processing
 ========================================================================================================
 """
 
 
 def draw_Van_Krevelen_diagrams(result, name='', path=None, dpi=300):
     """
-    Draws Van Krevelen diagrams to visually classify and compare the elemental composition 
-    of organic compounds based on their hydrogen-to-carbon (H/C) and oxygen-to-carbon (O/C) ratios. 
-    This function differentiates between compounds containing only carbon, hydrogen, and oxygen (CHO), 
-    those also containing nitrogen (CHON), sulfur (CHOS), or both (CHONS), and plots them on the diagram 
-    with distinct markers. Additionally, it delineates stoichiometric regions associated with different 
+    Draws Van Krevelen diagrams to visually classify and compare the elemental composition
+    of organic compounds based on their hydrogen-to-carbon (H/C) and oxygen-to-carbon (O/C) ratios.
+    This function differentiates between compounds containing only carbon, hydrogen, and oxygen (CHO),
+    those also containing nitrogen (CHON), sulfur (CHOS), or both (CHONS), and plots them on the diagram
+    with distinct markers. Additionally, it delineates stoichiometric regions associated with different
     compound classes such as lipids, proteins, lignins, carbohydrates, etc., on the diagram.
 
     Parameters:
-        result (Pandas DataFrame): A DataFrame containing the columns 'C', 'H', 'O', 'N', and 'S' 
+        result (Pandas DataFrame): A DataFrame containing the columns 'C', 'H', 'O', 'N', and 'S'
                                    which represent the count of each element in the compounds. Must not
                                    contain NaN values in the 'C' column.
         name (str, optional): Title of the plot. Defaults to an empty string.
-        path (str, optional): File path where the plot image will be saved. If None, the plot is shown 
+        path (str, optional): File path where the plot image will be saved. If None, the plot is shown
                               using plt.show(). Defaults to None.
         dpi (int, optional): The resolution of the saved plot image in dots per inch. Defaults to 300.
 
     Returns:
         None. Displays the Van Krevelen diagram or saves it as a file, depending on the 'path' parameter.
 
     Raises:
         ValueError: If the 'result' DataFrame does not contain the required columns ('C', 'H', 'O', 'N', 'S').
 
     Example usage:
         draw_Van_Krevelen_diagrams(result_df, name='Sample Van Krevelen Diagram', path='diagram.png', dpi=300)
 
     Note:
-        - This function is specifically designed for analyzing and visualizing elemental compositions 
+        - This function is specifically designed for analyzing and visualizing elemental compositions
           in organic geochemistry and may not be applicable for other types of data.
-        - Ensure the 'result' DataFrame is preprocessed to remove NaN values in 'C' column and contains 
+        - Ensure the 'result' DataFrame is preprocessed to remove NaN values in 'C' column and contains
           the necessary elemental columns before calling this function.
     """
 
     # 数据处理
     result1 = result[~result['C'].isna()]
     CHO = result1[(result1['N'] == 0) & (result1['S'] == 0)]
     CHO_OC = CHO['O/C']
@@ -6293,24 +6296,24 @@
 
 def get_correction_factor_waters(file, lock_mass=556.2771):
     """
     Calculate the correction factor for Waters LC-TOF-MS data based on the lockmass value.
 
     Parameters:
     - file (str): Path to the mzML file containing the LC-TOF-MS data.
-    - lockmass (float, optional): The lockmass value used for correction. Default values are 
+    - lockmass (float, optional): The lockmass value used for correction. Default values are
       556.2771 for positive mode and 554.2615 for negative mode.
 
     Returns:
     tuple: A tuple containing two elements:
         - factor_median (float): The median of the calculated correction factors.
         - factor_mean (float): The mean of the calculated correction factors.
 
-    The function reads the provided mzML file, identifies the lockmass peaks, and calculates the 
-    correction factors for mass-to-charge (m/z) values. The median and mean of these factors are 
+    The function reads the provided mzML file, identifies the lockmass peaks, and calculates the
+    correction factors for mass-to-charge (m/z) values. The median and mean of these factors are
     then returned.
     """
     run = pymzml.run.Reader(file)
     function_nums = [scan.id_dict['function'] for scan in run]
     func_num_max = max(function_nums)
     lockspray = [scan for scan in run if scan.id_dict['function'] == func_num_max]
     mz_corr_factors = []
```

## Comparing `pyhrms-0.8.9/pyhrms/__init__.py` & `pyhrms-0.9.0/pyhrms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import pyhrms
 
-__version__ = "0.8.9"
+__version__ = "0.9.0"
 
 __all__ = [
     "sep_scans",
     "gen_df",
     "peak_picking",
     "split_peak_picking",
     "remove_unnamed_columns",
```

