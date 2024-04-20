# Comparing `tmp/necessaryconditionanalysis-0.1.0.tar.gz` & `tmp/necessaryconditionanalysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "necessaryconditionanalysis-0.1.0.tar", last modified: Sun Apr 14 21:12:59 2024, max compression
+gzip compressed data, was "necessaryconditionanalysis-0.1.1.tar", last modified: Sat Apr 20 13:50:13 2024, max compression
```

## Comparing `necessaryconditionanalysis-0.1.0.tar` & `necessaryconditionanalysis-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:59.800976 necessaryconditionanalysis-0.1.0/
--rw-rw-rw-   0        0        0     1098 2024-04-14 15:22:39.000000 necessaryconditionanalysis-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     1798 2024-04-14 21:12:59.795007 necessaryconditionanalysis-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1269 2024-04-14 15:13:43.000000 necessaryconditionanalysis-0.1.0/README.md
--rw-rw-rw-   0        0        0      504 2024-04-14 21:09:12.000000 necessaryconditionanalysis-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 21:12:59.800976 necessaryconditionanalysis-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:59.741708 necessaryconditionanalysis-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:59.762455 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis/
--rw-rw-rw-   0        0        0       33 2024-04-14 20:33:44.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis/__init__.py
--rw-rw-rw-   0        0        0    25935 2024-04-14 20:05:09.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:12:59.791003 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/
--rw-rw-rw-   0        0        0     1798 2024-04-14 21:12:59.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-04-14 21:12:59.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 21:12:59.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-14 21:12:59.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-14 21:12:59.000000 necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 13:50:13.363682 necessaryconditionanalysis-0.1.1/
+-rw-rw-rw-   0        0        0     1098 2024-04-14 15:22:39.000000 necessaryconditionanalysis-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     1798 2024-04-20 13:50:13.359691 necessaryconditionanalysis-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1269 2024-04-14 15:13:43.000000 necessaryconditionanalysis-0.1.1/README.md
+-rw-rw-rw-   0        0        0      504 2024-04-20 13:41:40.000000 necessaryconditionanalysis-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:50:13.364683 necessaryconditionanalysis-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 13:50:13.306721 necessaryconditionanalysis-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:50:13.329386 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis/
+-rw-rw-rw-   0        0        0       33 2024-04-14 20:33:44.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis/__init__.py
+-rw-rw-rw-   0        0        0    27461 2024-04-20 13:30:20.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:50:13.355302 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/
+-rw-rw-rw-   0        0        0     1798 2024-04-20 13:50:13.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-04-20 13:50:13.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:50:13.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-20 13:50:13.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-20 13:50:13.000000 necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/top_level.txt
```

### Comparing `necessaryconditionanalysis-0.1.0/LICENCE` & `necessaryconditionanalysis-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `necessaryconditionanalysis-0.1.0/PKG-INFO` & `necessaryconditionanalysis-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NecessaryConditionAnalysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: Necessary Condition Analysis in Python
 Author-email: Ricardo Chavelas Manzo <R.ChavelasManzo@tilburguniversity.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `necessaryconditionanalysis-0.1.0/README.md` & `necessaryconditionanalysis-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis/main.py` & `necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -325,37 +325,75 @@
     return(bb_table)
 
   # Calculate OLS model for all observations (a + b * x) returns (slope, intercept)
   @staticmethod
   def __OLS_params(data_array):
     return np.polyfit(data_array[:,0], data_array[:,1], deg=1)
 
+  # Define properties for non-public attributes  
+  ## effects_ property
+  @property
+  def effects_(self):
+    if not self.__fitted:
+      raise Exception("NCA has not been fitted, make sure to .fit() de model")
+    return pd.DataFrame(self._effects_)
+  ## accuracy_ property
+  @property
+  def accuracy_(self):
+    if not self.__fitted:
+      raise Exception("NCA has not been fitted, make sure to .fit() de model")
+    return pd.DataFrame(self._accuracy_)
+  ## condition_inefficiency_ property
+  @property
+  def condition_inefficiency_(self):
+    if not self.__fitted:
+      raise Exception("NCA has not been fitted, make sure to .fit() de model")
+    return pd.DataFrame(self._condition_inefficiency_)
+  ## condition_inefficiency_point_ property
+  @property
+  def condition_inefficiency_point_(self):
+    if not self.__fitted:
+      raise Exception("NCA has not been fitted, make sure to .fit() de model")
+    return pd.DataFrame(self._condition_inefficiency_point_)
+  ## outcome_inefficiency_ property
+  @property
+  def outcome_inefficiency_(self):
+    if not self.__fitted:
+      raise Exception("NCA has not been fitted, make sure to .fit() de model")
+    return pd.DataFrame(self._outcome_inefficiency_)
+  ## outcome_inefficiency_point_ property
+  @property
+  def outcome_inefficiency_point_(self):
+    if not self.__fitted:
+      raise Exception("NCA has not been fitted, make sure to .fit() de model")
+    return pd.DataFrame(self._outcome_inefficiency_point_)
+
   # Main methods of the NCA class
   ## fit() method, fits the data to the specified NCA ceilings
   def fit(self, X, y, data):
     '''
     X: Conditions / Cause / Independent variable(s)
     Y: Outcome / Effect / Dependent variable
     data: a dataframe like object
     '''
     # Create an attribute for the y and X variable names
     self.__y = y
     self.__X = X
-    # Create empty dict to hold effect sizes for all X for selected ceilings
-    self.effects_ = {}
+    ## Create empty dict to hold effect sizes for all X for selected ceilings
+    self._effects_ = {}   
     # Create empty dict to hold accuracy for all X for selected ceilings
-    self.accuracy_ = {}
+    self._accuracy_ = {}
     # Create emtpy dict to hold condition inefficiency for all X for selected ceilings
-    self.condition_inefficiency_ = {}
+    self._condition_inefficiency_ = {}
     # Create emtpy dict to hold outcome inefficiency for all X for selected ceilings
-    self.outcome_inefficiency_ = {}
+    self._outcome_inefficiency_ = {}
     # Create emtpy dict to hold condition inefficiency points for all x for selected ceilings
-    self.condition_inefficiency_point_ = {}
+    self._condition_inefficiency_point_ = {}
     # Create emtpy dict to hold outcome inefficiency points for all x for selected ceilings
-    self.outcome_inefficiency_point_ = {}
+    self._outcome_inefficiency_point_ = {}
 
     # Check that the data has the correct shape
     NCA.__check_data(X, y, data)
 
     # Calculate initial parameters
     self.__scope_limits = NCA.__define_scope_lims(data, X, y)
 
@@ -379,17 +417,17 @@
       # Calculate CE-FDH accuracy (by definition is always 1)
       self.__CE_FDH_accuracy_dict = {}
       for x_item in X:
         self.__CE_FDH_accuracy_dict[x_item] = 1
       # Append reports only in CE-FDH is in the required ceilings
       if "ce-fdh" in self.ceilings:
         ## Append CE-FDH effect sizes on effect sizes main dict
-        self.effects_["ce-fdh"] = self.__CE_FDH_effect_sizes_dict
+        self._effects_["ce-fdh"] = self.__CE_FDH_effect_sizes_dict
         ## Append CR-FDH accuarcy of accuracy main dict
-        self.accuracy_["ce-fdh"] = self.__CE_FDH_accuracy_dict
+        self._accuracy_["ce-fdh"] = self.__CE_FDH_accuracy_dict
 
     # Calculate CR-FDH if CR-FDH is in required ceilings
     if "cr-fdh" in self.ceilings:
       # Calculate CR-FDH OLS parameters
       self.__CR_FDH_OLS_params_dict = {}
       for x_item in X:
         self.__CR_FDH_OLS_params_dict[x_item] = NCA.__CR_FDH_OLS_params(self.__CE_FDH_upper_left_edges_dict[x_item])
@@ -401,43 +439,43 @@
                                                                 self.__CR_FDH_OLS_params_dict[x_item][1])
       # Calculate CR-FDH effect sizes
       self.__CR_FDH_effect_sizes_dict = {}
       for x_item in X:
         self.__CR_FDH_effect_sizes_dict[x_item] = NCA.__CR_FDH_effect_size(self.__scope_limits[x_item]["Scope"],
                                                         self.__CR_FDH_polygon_array_dict[x_item])
       ## Append CR-FDH effect sizes on effect sizes main dict
-      self.effects_["cr-fdh"] = self.__CR_FDH_effect_sizes_dict
+      self._effects_["cr-fdh"] = self.__CR_FDH_effect_sizes_dict
       # Calculate CR-FDH accuracy
       self.__CR_FDH_accuracy_dict = {}
       for x_item in X:
         self.__CR_FDH_accuracy_dict[x_item] = NCA.__accuracy_from_abline(self.__sorted_arrays[x_item],
                                                                            self.__CR_FDH_OLS_params_dict[x_item][0],
                                                                            self.__CR_FDH_OLS_params_dict[x_item][1])
       ## Append CR-FDH accuarcy of accuracy main dict
-      self.accuracy_["cr-fdh"] = self.__CR_FDH_accuracy_dict
+      self._accuracy_["cr-fdh"] = self.__CR_FDH_accuracy_dict
       # Calculate CR-FDH condition inefficiency
       self.__CR_FDH_condition_inefficiency_dict = {}
       self.__CR_FDH_condition_innefficiency_point_dict = {}
       for x_item in X:
         self.__CR_FDH_condition_inefficiency_dict[x_item], self.__CR_FDH_condition_innefficiency_point_dict[x_item] = NCA.__condition_inefficiency_from_abline(scope_lims=self.__scope_limits[x_item],
                                                                                                      slope_abline=self.__CR_FDH_OLS_params_dict[x_item][0],
                                                                                                      intercept_abline=self.__CR_FDH_OLS_params_dict[x_item][1])
       ## Append CR-FDH condition inefficiency  to main dict
-      self.condition_inefficiency_["cr-fdh"] = self.__CR_FDH_condition_inefficiency_dict
-      self.condition_inefficiency_point_["cr-fdh"] = self.__CR_FDH_condition_innefficiency_point_dict
+      self._condition_inefficiency_["cr-fdh"] = self.__CR_FDH_condition_inefficiency_dict
+      self._condition_inefficiency_point_["cr-fdh"] = self.__CR_FDH_condition_innefficiency_point_dict
       # Calculate CR-FDH outcome inefficiency
       self.__CR_FDH_outcome_inefficiency_dict = {}
       self.__CR_FDH_outcome_innefficiency_point_dict = {}
       for x_item in X:
         self.__CR_FDH_outcome_inefficiency_dict[x_item], self.__CR_FDH_outcome_innefficiency_point_dict[x_item] = NCA.__outcome_inefficiency_from_abline(scope_lims=self.__scope_limits[x_item],
                                                                                                  slope_abline=self.__CR_FDH_OLS_params_dict[x_item][0],
                                                                                                  intercept_abline=self.__CR_FDH_OLS_params_dict[x_item][1])
       ## Append CR-FDH outcome inefficiency to main dict
-      self.outcome_inefficiency_["cr-fdh"] = self.__CR_FDH_outcome_inefficiency_dict
-      self.outcome_inefficiency_point_["cr-fdh"] = self.__CR_FDH_outcome_innefficiency_point_dict
+      self._outcome_inefficiency_["cr-fdh"] = self.__CR_FDH_outcome_inefficiency_dict
+      self._outcome_inefficiency_point_["cr-fdh"] = self.__CR_FDH_outcome_innefficiency_point_dict
 
     # Calculate OLS model parameters for all observations (a + b*x)
     if "ols" in self.ceilings:
       # Calculate OLS parameters
       self.__OLS_params_dict = {}
       for x_item in X:
         self.__OLS_params_dict[x_item] = NCA.__OLS_params(self.__sorted_arrays[x_item])
```

### Comparing `necessaryconditionanalysis-0.1.0/src/NecessaryConditionAnalysis.egg-info/PKG-INFO` & `necessaryconditionanalysis-0.1.1/src/NecessaryConditionAnalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NecessaryConditionAnalysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: Necessary Condition Analysis in Python
 Author-email: Ricardo Chavelas Manzo <R.ChavelasManzo@tilburguniversity.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

