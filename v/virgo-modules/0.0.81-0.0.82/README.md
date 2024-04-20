# Comparing `tmp/virgo_modules-0.0.81.tar.gz` & `tmp/virgo_modules-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.81.tar", last modified: Fri Apr 19 12:56:41 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.82.tar", last modified: Sat Apr 20 13:56:40 2024, max compression
```

## Comparing `virgo_modules-0.0.81.tar` & `virgo_modules-0.0.82.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 12:56:41.031851 virgo_modules-0.0.81/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.81/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-19 12:56:41.028850 virgo_modules-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.81/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 12:56:41.031851 virgo_modules-0.0.81/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-19 12:55:21.000000 virgo_modules-0.0.81/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:56:40.896190 virgo_modules-0.0.81/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-19 12:56:40.923193 virgo_modules-0.0.81/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:56:41.022849 virgo_modules-0.0.81/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    71590 2024-04-19 12:55:21.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.81/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:56:40.961588 virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-19 12:56:40.000000 virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-19 12:56:40.000000 virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 12:56:40.000000 virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-19 12:56:40.000000 virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 12:56:40.000000 virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.289166 virgo_modules-0.0.82/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.82/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-04-20 13:56:40.286166 virgo_modules-0.0.82/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.82/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:56:40.289166 virgo_modules-0.0.82/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-20 13:56:03.000000 virgo_modules-0.0.82/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.203163 virgo_modules-0.0.82/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.238168 virgo_modules-0.0.82/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.283165 virgo_modules-0.0.82/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    71590 2024-04-19 12:55:21.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   144162 2024-04-20 13:56:03.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.259163 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.81/LICENSE` & `virgo_modules-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.81/PKG-INFO` & `virgo_modules-0.0.82/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.81
+Version: 0.0.82
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.81/setup.py` & `virgo_modules-0.0.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.81",
+    version="0.0.82",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.82/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.82/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.82/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.82/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.82/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -2700,15 +2700,15 @@
         Parameters
         ----------
         test_size (int): test data size
         feature_name (str): name of the feature to assess
         days_list (list): list of integers [3,8,10] to assess
         threshold (float): alpha or z threshold
         verbose (boolean): print metrics
-        signal_position (int): if true, the signal is taken at the given step in the signal
+        signal_position (int): if true, the signal is taken at the given step after the signal end
 
         Returns
         -------
         None
         """
         data = self.data
         self.feature_name = feature_name
@@ -2717,14 +2717,15 @@
 
         df = data[features_base].sort_values('Date').iloc[0:-test_size,:]
         returns_list = list()
 
         for days in days_list:
 
             feature_ = f'return_{days}d'
+            days = days + signal_position if signal_position else days
             df[feature_] = (df['Close'].shift(-days)/df['Close']-1)*100
             returns_list.append(feature_)
 
         df['signal_type'] = np.where(
             df[up_signal] == 1,
             'up',
             np.where(
@@ -2754,17 +2755,24 @@
         self.df_signal = df
 
         n_signals_up = len(list(df[df.signal_type == 'up'].chain_id.unique()))
         n_signals_down = len(list(df[df.signal_type == 'down'].chain_id.unique()))
         p_scores = list()
         medians_down = list()
         validations = list()
-        if not signal_position: ### for now it is based on the last signal on a chain
-            df_melt = df[df.last_in_chain == True].melt(id_vars=['signal_type'], value_vars=returns_list, var_name='time', value_name='value')
-            df_melt = df_melt.dropna()
+
+        if signal_position:
+            df['open_long'] = np.where(df.last_in_chain == True, True, np.nan)
+            df['open_long'] = df['open_long'].shift(signal_position)
+        else:
+            df['open_long'] = np.where(df.last_in_chain == True, True, np.nan)
+            
+        # df_melt = df[df.last_in_chain == True].melt(id_vars=['signal_type'], value_vars=returns_list, var_name='time', value_name='value')
+        df_melt = df[df.open_long == True].melt(id_vars=['signal_type'], value_vars=returns_list, var_name='time', value_name='value')
+        df_melt = df_melt.dropna()
 
         for evalx in returns_list:
 
             sample1 = df_melt[(df_melt.time == evalx) & (df_melt.signal_type == 'up')].value.values
             sample2 = df_melt[(df_melt.time == evalx) & (df_melt.signal_type == 'down')].value.values
             pvalue = stats.ttest_ind(sample1, sample2).pvalue
             median_down = np.median(sample2)
@@ -2790,28 +2798,33 @@
             if verbose:
                 print('success evals')
             self.mean_median_return = mean_median_return
         else:
             self.mean_median_return = np.nan
 
         df2 = df.copy()
-        df2 = df2[df2.last_in_chain == True]
+        df2 = df2[df2.open_long == True]
 
 
         df2['lagdate'] = df2.Date.shift(1)
         df2['span'] = (pd.to_datetime(df2['Date']) - pd.to_datetime(df2['lagdate'])).dt.days
 
         fig, axs = plt.subplots(1, 3, figsize = (15,5))
 
-        sns.boxplot(data=df2, y="span",ax = axs[0])
+        sns.violinplot(data=df2, y="span",ax = axs[0], color = 'lightblue', linewidth=0.7,inner="quart")
+        sns.stripplot(data=df2, y="span",ax = axs[0], jitter=True, zorder=1)
         axs[0].set_title('span between last signals')
         del df2
-        sns.boxplot(data=df[df.last_in_chain == True], y="internal_rn",ax = axs[1])
+        sns.violinplot(data=df[df.last_in_chain == True], y="internal_rn",ax = axs[1], color = 'lightblue', linewidth=0.7,inner="quart")
+        sns.stripplot(data=df[df.last_in_chain == True], y="internal_rn",ax = axs[1], jitter=True, zorder=1)
         axs[1].set_title('signal duration distribution')
-        sns.boxplot(data=df_melt, x="time", y="value", hue="signal_type",ax = axs[2])
+
+        palette ={"go down": "tomato", "go up": "lightblue"}
+        df_melt.signal_type = df_melt.signal_type.map({'up':'go down', 'down': 'go up'})
+        sns.violinplot(data=df_melt, x="time", y="value", hue="signal_type",ax = axs[2], split=True, gap=0.1, inner="quart",palette = palette, linewidth=0.8)
         axs[2].axhline(y=0, color='grey', linestyle='--')
         axs[2].set_title('signal type expected returns distribution at different time lapses')
 
         if self.show_plot:
             plt.show()
 
         if self.save_path:
@@ -2826,26 +2839,27 @@
             plt.close()
 
         del df
 
         if self.return_fig:
             return fig
 
-    def create_backtest_signal(self,days_strategy, test_size, feature_name, high_exit = False, low_exit = False):
+    def create_backtest_signal(self,days_strategy, test_size, feature_name, high_exit = False, low_exit = False, signal_position = False):
         """
         perform backtest signal analysis
 
         Parameters
         ----------
         days_strategy (list): list of days to assess returns
         test_size (str): test data size
         feature_name (str): name of the feature to assess
         high_exit (float): high exit thrshold return in backtest
         low_exit (float): loss exit thrshold return in backtest
-
+        signal_position (int): if true, the signal is taken at the given step after the signal end
+        
         Returns
         -------
         fig (obj): plots
         messages (dict): dictionary with key metrics
         """
         asset_1 = 'Close'
         up_signal, low_signal= f'signal_up_{feature_name}', f'signal_low_{feature_name}'
@@ -2883,27 +2897,36 @@
         dft = df1.merge(df2,how = 'left',left_index=True, right_index=True )
 
         dft['chain_id'] = dft.sort_values(['Date']).groupby(['last_in_chain']).cumcount() + 1
         dft['chain_id'] = np.where(dft['last_in_chain'] == True, dft['chain_id'], np.nan )
         dft['chain_id'] = dft['chain_id'].fillna(method = 'ffill')
 
         dft['internal_rn'] = dft.sort_values(['Date']).groupby(['chain_id']).cumcount() + 1
-        dft['flag'] = np.where(dft['internal_rn'] < days_strategy, 1,0)
-
+        
         dft['lrets_bench'] = np.log(dft[asset_1]/dft[asset_1].shift(1))
         dft['bench_prod'] = dft['lrets_bench'].cumsum()
         dft['bench_prod_exp'] = np.exp(dft['bench_prod']) - 1
 
+        if signal_position:
+            dft['open_long'] = np.where(dft.last_in_chain == True, True, np.nan)
+            dft['open_long'] = dft.groupby(['chain_id'])['open_long'].shift(signal_position)
+            dft['flag'] = np.where(dft['internal_rn'] < days_strategy + signal_position, 1,0)
+            dft['flag'] = dft.groupby(['chain_id'])['flag'].shift(signal_position)
+        else:
+            dft['open_long'] = np.where(dft.last_in_chain == True, True, np.nan)
+            dft['flag'] = np.where(dft['internal_rn'] < days_strategy, 1,0)
+            
         if high_exit and low_exit:
-            dft['open_strat'] = np.where(dft.last_in_chain == True, dft.Open, np.nan)
+            dft['open_strat'] = np.where(dft.open_long == True, dft.Open, np.nan)
             dft['open_strat'] = dft['open_strat'].fillna(method = 'ffill')
             dft['open_strat'] = np.where(dft.flag == 1, dft.open_strat, np.nan)
             dft['high_strat_ret'] = (dft['High']/dft['open_strat']-1)*100
             dft['low_strat_ret'] = (dft['Low']/dft['open_strat']-1)*100
-            dft['high_exit'] =  np.where(((dft['high_strat_ret'] >= high_exit) | (dft['internal_rn'] == days_strategy)), 1, np.nan)
+            dft['max_step_chain'] = dft.groupby(['chain_id'])['internal_rn'].transform('max')
+            dft['high_exit'] =  np.where(((dft['high_strat_ret'] >= high_exit) | (dft['internal_rn'] == days_strategy) | (dft['max_step_chain'] == dft['internal_rn'])), 1, np.nan)
             dft['low_exit'] =  np.where((dft['low_strat_ret'] <= low_exit), -1, np.nan)
 
             dft["exit_type"] = dft[["high_exit", "low_exit"]].max(axis=1)
             dft['exit_type'] = np.where(dft["exit_type"] == 1, 1, np.where(dft["exit_type"] == -1,-1,np.nan))
             dft['exit'] = np.where(dft['exit_type'].isnull(), np.nan, 1)
             dft['exit_order'] = dft.sort_values(['Date']).groupby(['chain_id','exit']).cumcount() + 1
             dft['exit'] = np.where(dft['exit_order'] == 1, True, np.nan)
@@ -2912,16 +2935,18 @@
             max_id = dft.chain_id.max()
             dft['max_internal_rn'] = dft.sort_values(['Date']).groupby(['chain_id']).internal_rn.transform('max')
             dft['exit'] = np.where((dft.chain_id == max_id) & (dft.max_internal_rn < days_strategy) & (dft.max_internal_rn == dft.internal_rn), 1, dft['exit'])
 
             dft['exit_step'] = np.where(dft.exit == 1, dft.internal_rn, np.nan)
             dft['exit_step'] = dft.sort_values(['Date']).groupby(['chain_id']).exit_step.transform('max')
 
-            dft['flag'] = np.where(dft.internal_rn <= dft.exit_step, 1, 0)
-            dft = dft.drop(columns = ['open_strat', 'high_strat_ret', 'low_strat_ret','exit_step', 'exit','exit_type','high_exit','low_exit', 'max_internal_rn'])
+            if signal_position:
+                dft['flag'] = np.where( (dft.internal_rn >= signal_position + 1) & (dft.internal_rn <= dft.exit_step) , 1,0)
+            else:
+                dft['flag'] = np.where(dft.internal_rn <= dft.exit_step, 1, 0)
 
         dft['lrets_strat'] = np.log(dft[asset_1].shift(-1)/dft[asset_1]) * dft['flag']
         dft['lrets_strat'] = np.where(dft['lrets_strat'].isna(),-0.0,dft['lrets_strat'])
         dft['lrets_prod'] = dft['lrets_strat'].cumsum()
         dft['strat_prod_exp'] = np.exp(dft['lrets_prod']) - 1
 
         bench_rets = round(dft['bench_prod_exp'].values[-1]*100,1)
@@ -2941,35 +2966,34 @@
         }
         if self.show_plot:
             print('----------------------------')
             print(messages)
             print('----------------------------')
 
         fig = plt.figure(1)
-        plt.plot(dft.bench_prod_exp.values, label = 'benchmark')
+        plt.plot(dft.bench_prod_exp.values, label = 'benchmark', color = 'steelblue')
         plt.scatter(range(len(dft)),np.where(dft[low_signal] == 1,dft.bench_prod_exp.values,np.nan),color = 'red', label = 'signal')
-        plt.plot(dft.strat_prod_exp.values, label = 'strategy')
+        plt.plot(dft.strat_prod_exp.values, label = 'strategy', color = 'darksalmon')
+        plt.xlabel("index")
+        plt.ylabel("comulative return")
         plt.legend()
         plt.title('strategy and cumulative returns based on signal strategy')
         if self.show_plot:
             plt.plot()
 
         if self.save_path:
             result_json_name = f'signals_strategy_return_{feature_name}.json'
             result_plot_name = f'signals_strategy_return_{feature_name}.png'
 
             plt.savefig(self.save_path+result_plot_name)
-            # pickle.dump(fig, open(self.save_path+result_plot_name, 'wb'))
 
             with open(self.save_path+result_json_name, "w") as outfile:
                 json.dump(messages, outfile)
 
         if self.save_path and self.save_aws:
-            # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_json_name ,input_path = self.save_path+result_json_name)
-            # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_plot_name,input_path = self.save_path+result_plot_name)
 
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_plot_name, input_path = self.save_path + result_plot_name, aws_credentials = self.aws_credentials)
 
         if not self.show_plot:
             plt.close()
```

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.81
+Version: 0.0.82
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.81/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

