# Comparing `tmp/FreeBack-4.1.0a0.tar.gz` & `tmp/FreeBack-4.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-4.1.0a0.tar", last modified: Sat Apr 20 04:07:36 2024, max compression
+gzip compressed data, was "FreeBack-4.1.3a0.tar", last modified: Sat Apr 20 07:21:42 2024, max compression
```

## Comparing `FreeBack-4.1.0a0.tar` & `FreeBack-4.1.3a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 04:07:36.319091 FreeBack-4.1.0a0/
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 04:07:36.317746 FreeBack-4.1.0a0/FreeBack/
--rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.1.0a0/FreeBack/__init__.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    39658 2024-04-16 13:23:25.000000 FreeBack-4.1.0a0/FreeBack/alpha.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    33125 2024-04-11 18:28:29.000000 FreeBack-4.1.0a0/FreeBack/barbybar.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    12161 2024-04-19 14:28:57.000000 FreeBack-4.1.0a0/FreeBack/display.py
--rw-r--r--   0 h1nlee     (501) staff       (20)     9898 2024-04-13 14:29:24.000000 FreeBack-4.1.0a0/FreeBack/event.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    15290 2024-04-09 12:56:42.000000 FreeBack-4.1.0a0/FreeBack/my_pd.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    30696 2024-04-20 04:03:29.000000 FreeBack-4.1.0a0/FreeBack/post.py
--rw-r--r--   0 h1nlee     (501) staff       (20)     3757 2024-04-20 02:54:09.000000 FreeBack-4.1.0a0/FreeBack/strat.py
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 04:07:36.318621 FreeBack-4.1.0a0/FreeBack.egg-info/
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/SOURCES.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/dependency_links.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)       63 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/requires.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/top_level.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.1.0a0/LICENSE
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 04:07:36.318811 FreeBack-4.1.0a0/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.1.0a0/README.md
--rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-20 04:07:36.319143 FreeBack-4.1.0a0/setup.cfg
--rw-r--r--   0 h1nlee     (501) staff       (20)     1248 2024-04-19 18:48:22.000000 FreeBack-4.1.0a0/setup.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 07:21:42.154640 FreeBack-4.1.3a0/
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 07:21:42.153264 FreeBack-4.1.3a0/FreeBack/
+-rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.1.3a0/FreeBack/__init__.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    39658 2024-04-16 13:23:25.000000 FreeBack-4.1.3a0/FreeBack/alpha.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    33125 2024-04-11 18:28:29.000000 FreeBack-4.1.3a0/FreeBack/barbybar.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    12237 2024-04-20 06:25:35.000000 FreeBack-4.1.3a0/FreeBack/display.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     9898 2024-04-13 14:29:24.000000 FreeBack-4.1.3a0/FreeBack/event.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    15856 2024-04-20 07:06:42.000000 FreeBack-4.1.3a0/FreeBack/my_pd.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    31210 2024-04-20 06:21:59.000000 FreeBack-4.1.3a0/FreeBack/post.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     3757 2024-04-20 02:54:09.000000 FreeBack-4.1.3a0/FreeBack/strat.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 07:21:42.154192 FreeBack-4.1.3a0/FreeBack.egg-info/
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/SOURCES.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/dependency_links.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)       63 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/requires.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/top_level.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.1.3a0/LICENSE
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 07:21:42.154379 FreeBack-4.1.3a0/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.1.3a0/README.md
+-rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-20 07:21:42.154685 FreeBack-4.1.3a0/setup.cfg
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1248 2024-04-20 07:14:27.000000 FreeBack-4.1.3a0/setup.py
```

### Comparing `FreeBack-4.1.0a0/FreeBack/alpha.py` & `FreeBack-4.1.3a0/FreeBack/alpha.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.0a0/FreeBack/barbybar.py` & `FreeBack-4.1.3a0/FreeBack/barbybar.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.0a0/FreeBack/display.py` & `FreeBack-4.1.3a0/FreeBack/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     plt.subplots_adjust(left=None, bottom=None, right=None, top=None, hspace = None, wspace=0.5)
         
     plt.gcf().autofmt_xdate()
 
     return plt, fig, ax
 
 # 月度数据热力图  
-# period_value格式为 index month ‘2023-7-1’  value  0: ***
+# period_value 为pd.Series index month ‘2023-7-1’  value  0: ***
 # color_threshold 为红绿色分界点
 def month_thermal(period_value, color_threshold=0):   
     # 数值>0红色，<0为绿色。转化为颜色[R,G,B]
     def color_map(x, max_r):
         if x>0:
             return [1,1-x/max_r,1-x/max_r]
         elif x == 0:
@@ -72,25 +72,26 @@
     # 绝对值最大为纯红（绿）
         max_r = np.abs(data).max().max()
         mat_color = [color_map(i-color_threshold,max_r) for i in data]
         plot[i,j] = np.array(mat_color)
         return i, j, plot, calendar
 
     # 纵坐标为年份，横坐标为月份, 填充值
-    dates, data = list(period_value.index), period_value.iloc[:,0].values
+    dates, data = list(period_value.index), period_value.values
+    #period_value.iloc[:,0].values
     i, j, plot, calendar = calendar_array(dates, data)
     # 绘制热力图
     plt, fig, ax = matplot()
     ax.imshow(plot, aspect='auto')
     # 设置纵坐标 年份
     i = np.array(list(set(i)))
     i.sort()
     ax.set(yticks=i)
     # 年份
-    years = list(set([i.year for i in period_value.index]))
+    years = sorted(list(set([i.year for i in period_value.index])))
     ax.set_yticklabels(years)
     # 设置横坐标 月份
     j = np.array(list(set(j)))
     j.sort()
     ax.set(xticks=j)
     ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
                                 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
@@ -98,23 +99,23 @@
     ax.grid(False)
     # 显示数值
     for i_ in i:
         for j_ in j:
             if not np.isnan(calendar[i_][j_]):
                 ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
     return plt, fig, ax
-
+'''
 # 月度收益热力图    输入对数收益率的series 
 def plot_thermal(df_returns):
     # 先转化为对数收益率
     #df_lr = df_returns.apply(lambda x: np.log(x+1))
     df_lr = df_returns.reset_index()
     # 筛出同月数据
     df_lr['month'] = df_lr['date'].apply(lambda x: x - datetime.timedelta(x.day-1))
-    df_lr = df_lr[['month', df_returns.name]]
+    df_lr = df_lr[['month', (lambda x: 0 if x==None else x)(df_returns.name)]]
     df_lr = df_lr.set_index('month')
     # 月度收益 %
     period_return = (np.exp(df_lr.groupby('month').sum()) - 1)*100
     # 收益率转化为颜色[R,G,B]
     def color_map(x,max_r):
         if x>0:
             return [1,1-x/max_r,1-x/max_r]
@@ -167,15 +168,15 @@
     # 显示数值
     for i_ in i:
         for j_ in j:
             if not np.isnan(calendar[i_][j_]):
                 ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
 
     return plt, fig, ax
-
+'''
 
 
 
 ###########################################################
 ######################## 动态交互图 ###########################
 ###########################################################
```

### Comparing `FreeBack-4.1.0a0/FreeBack/event.py` & `FreeBack-4.1.3a0/FreeBack/event.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.0a0/FreeBack/my_pd.py` & `FreeBack-4.1.3a0/FreeBack/my_pd.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,74 +146,93 @@
 
 # 行情数据的常用计算
 # 数据格式为 mutiindex (date,code)   close...
 
 # 输入series返回series
 # 有并行选项的函数默认并行
 # a 函数可选参数
+
+
 def cal_ts(ser, func_name='Max', period=20, a=1, parallel=True, n_core=12):
     if func_name=='MA':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).mean()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).mean()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='EMA':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').ewm(\
+            span=period, min_periods=1).mean()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='Max':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).max()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).max()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='Min':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).min()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).min()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='Std':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).std()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).std()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='Skew':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).skew()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).skew()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='Kurt':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).kurt()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).kurt()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='Sum':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).sum()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).sum()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
     elif func_name=='rank':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).rank()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
+            period, min_periods=1).rank()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
     elif func_name=='quantile':
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).quantile(a)).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
+            period, min_periods=1).quantile(a)).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
     elif func_name=='Zscore':
         MA = ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).mean()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).mean()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
         Std = ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).std()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).std()).reset_index().sort_values(by='date').\
+                set_index(['date', 'code']).loc[ser.index].iloc[:,0]
         return ((ser-MA)/Std).fillna(0)
     elif func_name=='HV':
         returns = np.log(ser/ser.groupby(level='code').shift()).fillna(0)
         return np.exp(returns.groupby(level='code').apply(lambda x: x.droplevel('code').rolling(\
             period, min_periods=1).std()*np.sqrt(250)).reset_index().sort_values(\
                 by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0])-1
     elif func_name in ['WMA']:
         if parallel:
             def func(ser):
                 return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
                     period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2)))
             result = parallel_group(ser, func, n_core=n_core)
             return result.reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2))).reset_index().sort_values(by='date').set_index(\
-                ['date', 'code']).loc[ser.index].iloc[:,0]
+            period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2))).reset_index().\
+                sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    # 在rolling中无法直接调用的函数只能通过这种方法，速度慢几个数量级
     elif func_name in ['argmin', 'argmax', 'prod']:
         if parallel:
             def func(ser):
                 return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
                     period, min_periods=1).apply(getattr(np, func_name)))
             result = parallel_group(ser, func, n_core=n_core)
             return result.reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
         return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
             period, min_periods=1).apply(getattr(np, func_name))).reset_index().sort_values(by='date').set_index(\
                 ['date', 'code']).loc[ser.index].iloc[:,0]
 
+
 # 按照look列的阈值筛选得到cal列，求和
 def cal_select_sum(df, key, threshold_left, threshold_right, sum, n, n_core=12):
     # 按条件筛选滚动求和
     def rolling_select_sum(df, key, threshold_left, threshold_right, sum, n):
         # 如果这一字段的df长度小于n，直接返回nan,对应index
         if df.shape[0]<n:
             result_nan = np.ones(df.shape[0])*np.nan
```

### Comparing `FreeBack-4.1.0a0/FreeBack/post.py` & `FreeBack-4.1.3a0/FreeBack/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,27 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 import datetime
 import statsmodels.api as sm
 from plottable import ColumnDefinition, ColDef, Table
 from matplotlib.colors import LinearSegmentedColormap
 from FreeBack.display import *
+import FreeBack as FB
 import os
 # 该模块处理策略的后处理(业绩评价、归因）工作，主要包含：
 # 1. ReturnsPost 收益率序列后处理
 # 2. HoldPost 持仓矩阵后处理
 # 3. WorldPost barbybar模块World对象后处理
 
+# 结果文件保存于output中
+def check_output():
+    if 'output' in os.listdir():
+        pass
+    else:
+        os.mkdir('output')
 
 ############################################################################################
 ####################### 处理收益率序列（简单收益率，非对数收益率） ###########################
 ############################################################################################
 class ReturnsPost():
     # benchmark dataframe 收益率序列
     def __init__(self, returns, benchmark=0, stratname='策略'):
@@ -89,15 +96,15 @@
         ## 索提诺比率   单位下行风险的超额收益
         #self.sortino = (self.return_annual - self.rf)/(self.sigma_down*np.sqrt(250))
         # 特雷诺指数  单位beta的超额收益
         self.treynor  = (self.return_annual - self.rf)/self.beta 
 # 净值曲线
 # 时间起止（默认全部），是否显示细节,是否自定义输出图片名称，是否显示对数，是否显示超额
     def pnl(self, timerange=None, detail=True, filename=None, log=False, excess=False):
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
         if type(timerange) != type(None):
             # 时间段内净值与基准
             net = self.net.loc[timerange[0]:timerange[1]]
             returns = self.returns.loc[timerange[0]:timerange[1]]
             # 计算夏普
             years = (pd.to_datetime(timerange[1])-pd.to_datetime(timerange[0])).days/365
@@ -165,23 +172,111 @@
             ax2 = ax.twinx()
             ax2.fill_between(self.drawdown.index,-100*self.drawdown, 0, color='C1', alpha=0.1)
             ax.set_ylabel('累计净值')
             ax.set_xlabel('日期')
             ax2.set_ylabel('回撤 (%)')
             ax.set_xlim(self.net.index[0], self.net.index[-1])
             plt.gcf().autofmt_xdate()
-        if 'output' in os.listdir():
-            pass
-        else:
-            os.mkdir('output')
+        check_output()
         if type(filename) == type(None):
             plt.savefig('./output/pnl.png')
         else:
             plt.savefig('./output/'+filename)
         plt.show()
+# 滚动收益与夏普
+    def rolling_return(self, key='return'):
+        plt, fig, ax = FB.display.matplot()
+        if key=='return':
+            ax.plot((self.net/self.net.shift(120)-1)*100, c='C0', label='滚动半年收益')
+            ax2 = ax.twinx()
+            ax2.plot((self.net/self.net.shift(250)-1)*100, c='C3', label='滚动年度收益')
+            ax.legend(loc='upper left')
+            ax2.legend(loc='upper right')
+            ax.set_ylabel('(%)')
+            ax2.set_ylabel('(%)')
+        elif key=='sharpe':
+            halfyearly_sharpe = (np.exp(self.lr.rolling(120).mean()*250)-1)/\
+            ((np.exp(self.lr.rolling(120).std())-1)*np.sqrt(250))
+            yearly_sharpe = (np.exp(self.lr.rolling(250).mean()*250)-1)/\
+            ((np.exp(self.lr.rolling(250).std())-1)*np.sqrt(250))
+            ax.plot(halfyearly_sharpe, c='C0', label='滚动半年sharpe')
+            ax2 = ax.twinx()
+            ax2.plot(yearly_sharpe, c='C3', label='滚动年度sharpe')
+            ax.legend(loc='upper left')
+            ax2.legend(loc='upper right')
+            ax.set_ylim(-3, 10)
+        ax.set_xlim(self.returns.index[0], self.returns.index[-1]) 
+        plt.gcf().autofmt_xdate()
+        check_output()
+        plt.savefig('./output/rolling.png')
+        plt.show()
+# 年度与月度收益
+    def pnl_yearly(self):
+        lr = self.lr
+        lr.name = 'lr'
+        bench = np.log(self.benchmark[self.benchmark.columns[0]].fillna(0)+1)
+        bench.name = 'bench'
+        year = pd.Series(dict(zip(self.returns.index, self.returns.index.map(lambda x: x.year))))
+        year.name = 'year'
+        yearly_returns = pd.concat([year, lr, bench], axis=1)
+        yearly_returns = (np.exp(yearly_returns.groupby('year').sum())*100-100)
+
+        plt, fig, ax = FB.display.matplot()
+
+        len_years = len(yearly_returns)
+        plot_x = range(len_years)
+        plot_index = yearly_returns.index
+        plot_height = yearly_returns['lr'].values
+        plot_height1 = yearly_returns['bench'].values
+        # 如果benchmark是0的话就不画对比了
+        if not (self.benchmark==0).any().values[0]:
+            ax.bar([i-0.225  for i in plot_x], plot_height, width=0.45, color='C0', label='策略')
+            ax.bar([i+0.225  for i in plot_x], plot_height1, width=0.45, color='C4',\
+                    label=self.benchmark.columns[0])
+        else:
+            ax.bar([i  for i in plot_x], plot_height, width=0.45, color='C0', label='策略')
+        max_height = max(np.hstack([plot_height, plot_height1]))
+        min_height = min(np.hstack([plot_height, plot_height1]))
+        height = max_height-min_height
+        plt.ylim(min_height-0.1*height, max_height+0.1*height)
+
+        for x, contri in zip(plot_x, plot_height):
+            if contri>0:
+                plt.text(x-0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
+            else:
+                plt.text(x-0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
+        for x, contri in zip(plot_x, plot_height1):
+            if contri>0:
+                plt.text(x+0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
+            else:
+                plt.text(x+0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
+        plt.legend()
+        plt.title('年度收益')
+        plt.xticks(plot_x, labels=plot_index)
+        check_output()
+        plt.ylabel('(%)')
+        plt.savefig('./output/pnl_yearly.png')
+        plt.show()
+    def pnl_monthly(self, excess=False):
+        if excess:
+            df = self.excess_lr
+        else:
+            df = self.lr
+        name = (lambda x: 0 if x==None else x)(df.name) 
+        df = df.reset_index()
+        # 筛出同月数据
+        df['month'] = df['date'].apply(lambda x: x - datetime.timedelta(x.day-1))
+        df = df[['month', name]]
+        df = df.set_index('month')[name]
+        # 月度收益 %
+        period_return = (np.exp(df.groupby('month').sum()) - 1)*100
+        plt, fig, ax = FB.display.month_thermal(period_return)
+        check_output()
+        plt.savefig('./output/pnl_monthly.png')
+        plt.show()
 
 
 
 ############################################################################################
 ################################### 处理持仓表 ##############################################
 ############################################################################################
 class HoldPost(ReturnsPost):
@@ -466,98 +561,14 @@
             ax.set_xlim(self.net.index[0], self.net.index[-1])
             plt.gcf().autofmt_xdate()
         if type(filename) == type(None):
             plt.savefig('pnl.png')
         else:
             plt.savefig(filename)
         plt.show()
-# 滚动收益
-    def rolling_return(self):
-        plt, fig, ax = matplot()
-        ax.plot((self.net/self.net.shift(120)-1)*100, c='C0', label='滚动半年收益')
-        #ax.plot((post0.net/post0.net.shift(60)-1)*4, c='C1', label='quarter return')
-        #ax.plot((post0.net/post0.net.shift(120)-1)*2, c='C3', label='half year return')
-        ax2 = ax.twinx()
-        ax2.plot((self.net/self.net.shift(250)-1)*100, c='C3', label='滚动年度收益')
-        ax.legend(loc='upper left')
-        ax2.legend(loc='upper right')
-        ax.set_ylabel(' (%)')
-        ax2.set_ylabel('(%)')
-        ax.set_xlim(self.returns.index[0], self.returns.index[-1])
-        plt.gcf().autofmt_xdate()
-        plt.savefig('rolling_return.png')
-        plt.show()
-# 滚动sharpe
-    def rolling_sharpe(self):
-        plt, fig, ax = matplot()
-        halfyearly_sharpe = (np.exp(self.lr.rolling(120).mean()*250)-1)/\
-            ((np.exp(self.lr.rolling(120).std())-1)*np.sqrt(250))
-        yearly_sharpe = (np.exp(self.lr.rolling(250).mean()*250)-1)/\
-            ((np.exp(self.lr.rolling(250).std())-1)*np.sqrt(250))
-        ax.plot(halfyearly_sharpe, c='C0', label='滚动半年sharpe')
-        ax2 = ax.twinx()
-        ax2.plot(yearly_sharpe, c='C3', label='滚动年度sharpe')
-        ax.legend(loc='upper left')
-        ax2.legend(loc='upper right')
-        ax.set_ylim(-3, 10)
-        ax.set_xlim(self.returns.index[0], self.returns.index[-1])
-        plt.gcf().autofmt_xdate()
-        plt.savefig('rolling_sharpe.png')
-# 月度收益
-    def pnl_monthly(self):
-        plt,fig,ax = plot_thermal(self.lr)
-        plt.savefig('pnl_monthly.png')
-        plt.show()
-    def pnl_yearly(self):
-        lr = self.lr
-        lr.name = 'lr'
-        bench = np.log(self.benchmark[self.benchmark.columns[0]].fillna(0)+1)
-        bench.name = 'bench'
-        year = pd.Series(dict(zip(self.returns.index, self.returns.index.map(lambda x: x.year))))
-        year.name = 'year'
-        yearly_returns = pd.concat([year, lr, bench], axis=1)
-        yearly_returns = (np.exp(yearly_returns.groupby('year').sum())*100-100)
-
-        plt, fig, ax = matplot()
-
-        len_years = len(yearly_returns)
-        plot_x = range(len_years)
-        plot_index = yearly_returns.index
-        plot_height = yearly_returns['lr'].values
-        plot_height1 = yearly_returns['bench'].values
-
-        ax.bar([i-0.225  for i in plot_x], plot_height, width=0.45, color='C0', label='策略')
-        ax.bar([i+0.225  for i in plot_x], plot_height1, width=0.45, color='C4', label=self.benchmark.columns[0])
-
-        max_height = max(np.hstack([plot_height, plot_height1]))
-        min_height = min(np.hstack([plot_height, plot_height1]))
-        height = max_height-min_height
-        plt.ylim(min_height-0.1*height, max_height+0.1*height)
-
-        for x, contri in zip(plot_x, plot_height):
-            if contri>0:
-                plt.text(x-0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
-            else:
-                plt.text(x-0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
-        for x, contri in zip(plot_x, plot_height1):
-            if contri>0:
-                plt.text(x+0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
-            else:
-                plt.text(x+0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
-        plt.legend()
-        plt.title('年度收益')
-        plt.xticks(plot_x, labels=plot_index)
-        plt.ylabel('(%)')
-        plt.savefig('pnl_yearly.png')
-        plt.show()
-# 月度超额收益
-    def pnl_excess_monthly(self):
-        plt,fig,ax = plot_thermal(self.excess_lr)
-        plt.savefig('pnl_excess_monthly.png')
-        plt.show()
 # 交易分析
     def trade(self):
         self.CashFlow = self.excute.apply(lambda x: x['occurance_amount'] - x['comm'] if x['BuyOrSell']=='Sell' else -x['occurance_amount'] - x['comm'], axis=1)
         # 获取持仓卖出变为0时的订单unique，记为一次交易结束(有可能会出现同时两个卖出订单误判为两次交易)
         completes = list(self.excute[(self.excute['remain_vol'] == 0)&(self.excute['BuyOrSell']=='Sell')].reset_index()['unique'])
         # 对每个标的的累积现金流
         CumCashFlow = self.CashFlow.groupby('code').cumsum()
```

### Comparing `FreeBack-4.1.0a0/FreeBack/strat.py` & `FreeBack-4.1.3a0/FreeBack/strat.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.0a0/FreeBack.egg-info/PKG-INFO` & `FreeBack-4.1.3a0/FreeBack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.1.0a0
+Version: 4.1.3a0
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeBack-4.1.0a0/LICENSE` & `FreeBack-4.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.0a0/PKG-INFO` & `FreeBack-4.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.1.0a0
+Version: 4.1.3a0
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeBack-4.1.0a0/README.md` & `FreeBack-4.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.0a0/setup.py` & `FreeBack-4.1.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 setup(
     name="FreeBack",
     # 版本号: 第几次模块增加，第几次函数增加，第几次函数功能修改
     # (每次高级别序号增加后,低级别序号归0)
     # alpha为调试版,beta为测试版,stable为稳定版 
-    version="4.1.0-alpha",
+    version="4.1.3-alpha",
     author="LH.Li,zzq",
     author_email="lh98lee@zju.edu.cn",  
     description='Package for backtest',
     long_description=long_description, 
     # 描述文件为md格式
     long_description_content_type="text/markdown",
     url="https://github.com/LHanLi/FreeBack",
```

