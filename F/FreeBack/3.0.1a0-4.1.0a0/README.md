# Comparing `tmp/FreeBack-3.0.1a0.tar.gz` & `tmp/FreeBack-4.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-3.0.1a0.tar", last modified: Tue Apr 16 09:36:06 2024, max compression
+gzip compressed data, was "FreeBack-4.1.0a0.tar", last modified: Sat Apr 20 04:07:36 2024, max compression
```

## Comparing `FreeBack-3.0.1a0.tar` & `FreeBack-4.1.0a0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 09:36:06.862022 FreeBack-3.0.1a0/
-drwxrwxrwx   0        0        0        0 2024-04-16 09:36:06.829229 FreeBack-3.0.1a0/FreeBack/
--rw-rw-rw-   0        0        0       77 2024-04-11 06:17:47.000000 FreeBack-3.0.1a0/FreeBack/__init__.py
--rw-rw-rw-   0        0        0    40491 2024-04-16 09:31:17.000000 FreeBack-3.0.1a0/FreeBack/alpha.py
--rw-rw-rw-   0        0        0    33890 2024-04-11 00:53:14.000000 FreeBack-3.0.1a0/FreeBack/barbybar.py
--rw-rw-rw-   0        0        0    12401 2024-04-11 06:17:47.000000 FreeBack-3.0.1a0/FreeBack/display.py
--rw-rw-rw-   0        0        0    10140 2024-04-12 10:51:57.000000 FreeBack-3.0.1a0/FreeBack/event.py
--rw-rw-rw-   0        0        0    15629 2024-04-10 06:43:08.000000 FreeBack-3.0.1a0/FreeBack/my_pd.py
--rw-rw-rw-   0        0        0    35554 2024-04-16 07:31:49.000000 FreeBack-3.0.1a0/FreeBack/post.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:36:06.861025 FreeBack-3.0.1a0/FreeBack.egg-info/
--rw-rw-rw-   0        0        0     1232 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2024-04-12 01:34:50.000000 FreeBack-3.0.1a0/LICENSE
--rw-rw-rw-   0        0        0     1232 2024-04-16 09:36:06.861025 FreeBack-3.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0      596 2024-04-15 01:34:55.000000 FreeBack-3.0.1a0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 09:36:06.862022 FreeBack-3.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-04-16 07:24:51.000000 FreeBack-3.0.1a0/setup.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 04:07:36.319091 FreeBack-4.1.0a0/
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 04:07:36.317746 FreeBack-4.1.0a0/FreeBack/
+-rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.1.0a0/FreeBack/__init__.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    39658 2024-04-16 13:23:25.000000 FreeBack-4.1.0a0/FreeBack/alpha.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    33125 2024-04-11 18:28:29.000000 FreeBack-4.1.0a0/FreeBack/barbybar.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    12161 2024-04-19 14:28:57.000000 FreeBack-4.1.0a0/FreeBack/display.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     9898 2024-04-13 14:29:24.000000 FreeBack-4.1.0a0/FreeBack/event.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    15290 2024-04-09 12:56:42.000000 FreeBack-4.1.0a0/FreeBack/my_pd.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    30696 2024-04-20 04:03:29.000000 FreeBack-4.1.0a0/FreeBack/post.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     3757 2024-04-20 02:54:09.000000 FreeBack-4.1.0a0/FreeBack/strat.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 04:07:36.318621 FreeBack-4.1.0a0/FreeBack.egg-info/
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/SOURCES.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/dependency_links.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)       63 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/requires.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-20 04:07:36.000000 FreeBack-4.1.0a0/FreeBack.egg-info/top_level.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.1.0a0/LICENSE
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 04:07:36.318811 FreeBack-4.1.0a0/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.1.0a0/README.md
+-rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-20 04:07:36.319143 FreeBack-4.1.0a0/setup.cfg
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1248 2024-04-19 18:48:22.000000 FreeBack-4.1.0a0/setup.py
```

### Comparing `FreeBack-3.0.1a0/FreeBack/alpha.py` & `FreeBack-4.1.0a0/FreeBack/alpha.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,833 +1,833 @@
-import pandas as pd
-import numpy as np
-from scipy import stats
-import statsmodels.api as sm
-from FreeBack.post import matplot
-from FreeBack import my_pd
-import os
-# 该模块包含：
-# 因子计算常用函数
-# 单因子与多因子检验模块（组合法、回归法）
-
-
-#######################################################################################################
-####################################### 因子计算常用函数 #################################################
-#######################################################################################################
-# 无特殊说明下 factor,price的格式为pd.Series,其中index的格式为multiindex (date code)
-# Rank      
-# 每日全部index的因子值从小到大排序,均匀映射到(0,1)
-# Norm      
-# 将每日因子值在截面上标准化到 \mu = 0 \sigma = 1 分布
-# scale     
-# 使得截面上因子值满足sum(abs(x)) = 1(a) 
-# Gauss     
-# 将每日的因子值转化为正态分布
-# resample_fill/select  
-# 因子降频（日频因子换月频/周频）
-# QQ        绘制因子分布的QQ图，观察是否符合正态分布
-
-
-def Rank(factor, norm=False):
-    # 因子排名
-    rank = factor.groupby('date').rank()
-    if norm:
-        return 2*3**0.5*(rank/(rank.groupby('date').max()+1)-0.5)
-    return rank/(rank.groupby('date').max()+1)
-def Norm(factor):
-    return (factor - factor.groupby('date').mean())/factor.groupby('date').std()
-
-def scale(factor, a=1):
-    return a*factor/factor.groupby('date').apply(lambda x:abs(x).sum())
-# 通过正态分布累计概率函数的逆函数将[p,1-p]的均匀分布转化为正态分布，转换为正态分布后默认产生3sigma内的样本，99.7% p=0.003
-def Gauss(factor, p=0.003, slice=False):
-    # 开启slice选项时为仅转化一个截面启代表仅有一个截面数据
-    if not slice:
-        rank = factor.groupby('date').rank()
-        continuous = p/2+(1-p)*(rank-1)/(rank.groupby('date').max()-1)
-        def func(ser):
-            return ser.map(lambda x: stats.norm.ppf(x))
-        result = my_pd.parallel(continuous, func)
-        # 如果所有值相同则替换为0
-        if_same = result.groupby('date').apply(lambda x: (~x.duplicated()).sum())
-        result.loc[if_same[if_same==1].index] = 0
-        return result
-    else:
-        rank = factor.rank()
-        continuous = p/2+(1-p)*(rank-1)/(rank.max()-1)
-        return continuous.map(lambda x: stats.norm.ppf(x))
-# 每月、每周内的因子值替换为月初、周初因子值
-def resample_fill(factor, freq='month'):
-    factor.name=0
-    df = pd.DataFrame(factor)
-    df['th'] = df.index.map(lambda x:getattr(x[0], freq))
-    df['yesterday_th'] = df['th'].groupby('code').shift()
-    df = df.fillna(getattr(df.index[0][0], freq))
-    df['after'] = df.apply(lambda x: x[0] if x.th!=x.yesterday_th else np.nan, axis=1)
-    df = df.groupby('code').fillna(method='ffill')
-    df = df.groupby('code').fillna(method='bfill')
-    return df['after']
-# 直接只选用原数据的周初、月初值
-# 没有周一和1号的月份用下一个第一个出现的值***
-def resample_select(market, freq='month'):
-    if freq=='month':
-        return market[market.index.map(lambda x:getattr(x[0], 'day'))==1]
-    elif freq=='week':
-        return market[market.index.map(lambda x:getattr(x[0], 'weekday')())==0]
-def QQ(factor, date=None):
-    plt, fig, ax = matplot(w=6, d=4)
-    if date==None:
-        norm_dis = pd.Series(np.random.randn(len(factor))).sort_values()
-        ax.scatter(norm_dis, factor.sort_values())
-    else:
-        norm_dis = pd.Series(np.random.randn(len(factor.loc[date]))).sort_values()
-        ax.scatter(norm_dis, factor.loc[date].sort_values())
-    ax.plot(norm_dis, norm_dis, c='C3', ls='--')
-    ax.set_title('Q-Q plot')
-    ax.set_aspect('equal')
-    plt.show()
-
-
-
-#######################################################################################################
-######################################### 单因子检测 ####################################################
-#######################################################################################################
-# 1. 组合法， 计算各因子分层组合的收益及其他特征。
-    # Porfolio, 因子投资组合表现
-    # factorgroup
-# 2. 回归法， 假设截面上因子与未来收益率线性相关，计算该线性关系的一系列统计量。
-    # Reg
-
-########################################## 组合法 #######################################################
-
-class Portfolio():
-# factor 数据类型pd.Series, multiindex(date,code)   T日因子值(可以在此排除涨停板)
-# price 数据类型pd.Series, multiindex(date,code) T日交易价格(最宽松情况可以使用当日收盘价，\
-# 使用后一天开盘价或者VWAP等是接近实际情况的(全市场数据即可) 
-# norm 是否按照因子值的排序来对投资组合分组,默认开启。否则使用原始因子值进行分组 
-# divide 
-# 数据类型为tuple时，给出全部阈值确定连续分组；
-# 数据类型为list， 给出每个分组的前后阈值,例：[(0,0.1),(0.9,1)]表示选取最小10%和最大10%构建组合，前开后闭。
-# norm开启时，元素<=1时表示百分比，大于1时表示绝对数量，如(0,0.2)表示持有钱20%，(0，10)表示持有前十只。
-# 否则表示因子值的阈值。
-# justdivide 是否仅计算给出分组的收益而不计算全市场组合收益，默认计算全市场组合收益(权重由holdweight确定)
-# periods (1, 5, 20)同时计算1天5天20天轮动的结果
-# holdweight pd.Series, multiindex(data,code)  T日的投资组合权重，默认等权
-# comm 每次单边换手的交易成本，默认为0
-## 当日收益率为当日收盘价相对昨日收盘价收益率*前一日持仓权重
-## comm 不影响结果，仅仅在result中给出多头费后年化收益率 
-    def __init__(self, factor, price, norm=True, divide=(0, 0.2, 0.4, 0.6, 0.8, 1),\
-                 justdivide=False, periods=(1, ), \
-                  holdweight=None, comm=0):
-        self.comm = comm
-        self.norm = norm
-        self.justdivide=justdivide
-        # 一个确定持有张数（不去除停牌），一个确定收益率(去除停牌)
-        self.price = pd.DataFrame(price.rename('price')).pivot_table('price', 'date' ,'code')
-        # 每日收益率(当日收盘相比上日收盘)
-        returns = self.price/self.price.shift() - 1
-        self.returns = returns.fillna(0)
-#        # 先按照截面排序归一化
-        if norm:
-            self.factor = Rank(pd.DataFrame(factor.rename('factor')))
-        else:
-            self.factor = pd.DataFrame(factor.rename('factor'))
-        self.variable = factor
-        # 组合权重 
-        if type(holdweight) != type(None):
-            # 没有权重则按0计
-            holdweight = holdweight.fillna(0)
-            self.holdweight = holdweight.apply(lambda x: x/x.sum(), axis=1)
-        else:
-            self.holdweight = None
-        # 结果dataframe 行：时间周期  列：IC、ICIR（分组计算的IC、ICIR(非rank)）、 多空组合收益、多头收益、 等权收益、
-        # 考虑换手率多空收益、 夏普、 多空平均换手率
-        self.result = pd.DataFrame(columns=['group IC', 'group ICIR', 'L&S return', 'L return',\
-                 'market return', 'L&S sharpe', 'L sharpe', 'market sharpe', 'real return', \
-                    'real sharpe', 'turnover'])
-        self.result.index.name = 'holding period'
-        # 运行
-        self.run(divide, periods)
-    def run(self, divide, periods):
-        self.divide = divide
-        self.periods = periods
-        # self.a_b表示对因子分隔的阈值，如果是list则直接为a_b
-        if type(self.divide) == type(list()):
-            self.a_b = self.divide
-        # 如果是tuple则转化成list
-        else:
-            self.a_b = [(self.divide[i],self.divide[i+1]) for i in range(len(self.divide)-1)]
-        # 如果justdivide为False,则增加一个可以选中全部标的的组合
-        if not self.justdivide:
-            if self.norm == True:
-                # 按百分比划分
-                if self.a_b[-1][1]<=1:
-                    self.a_b = self.a_b + [(0,1)]
-                else:
-                    self.a_b = self.a_b + [(0, 99999)]
-            else:
-                self.a_b = self.a_b + [(self.factor.min().values[0], self.factor.max().values[0])]
-    # 生成持仓表 -> 获得 df_contri(index date  columns code) -> 获得净值每日对数收益率 -> 获得换手率
-    # 全部为矩阵操作
-        self.matrix_hold()
-        self.matrix_contri()
-        self.matrix_lr()
-        self.matrix_holdn()
-        self.matrix_turnover()
-        if not self.justdivide:
-            self.get_result()
-# mat[period][factor range]  list[factor range]
-# 获得每个持仓周期 每个因子区间的虚拟持仓(只保证比例关系正确) 
-# a_b factor range from a to b 区间内市值等权重
-    def matrix_hold(self):
-    # 每个bar按标的等权配置需要的持仓
-        if self.norm:
-            if self.a_b[-1][1]<=1:
-                look_factor = self.factor.groupby('date').rank(pct=True)
-            else:
-                print('整数排序')
-                look_factor = self.factor.groupby('date').rank()
-        else:
-            look_factor = self.factor
-        look_factor = look_factor.reset_index()
-        # 选取因子值 满足a_b list中全部条件的 放置于list_hold (前开后闭，与Rank函数返回的(0，1]对应)
-        bar_hold = [look_factor[(i[0]<look_factor['factor']) &\
-                                 (look_factor['factor']<=i[1])] for i in self.a_b]
-        # 每一组合选中的标的个数
-        self.group_number = [i.groupby('date').count() for i in bar_hold]
-        # 在date没有出现的code补np.nan
-        bar_hold = [pd.DataFrame(i.pivot_table('factor', 'date', 'code'),\
-                                 index=self.factor.index.get_level_values(0).unique())\
-                                     for i in bar_hold]
-        # 等权情况下持有标的的持仓数量为 1/price（持仓金额相等）
-        #bar_hold = [(i.isnull().replace([True,False],[0,1])*\
-        #             (1/self.price)).fillna(0) for i in bar_hold]
-        bar_hold = [((~i.isnull()).astype(int)*\
-                     (1/self.price)).fillna(0) for i in bar_hold]
-        # 当holdweight不为None时考虑此权重
-        if type(self.holdweight) != type(None):
-            bar_hold = [i*self.holdweight for i in bar_hold]
-        # 当period不等于1时需要按照period调整持仓
-        mat_hold = []
-        for period in self.periods:
-            # 以period为周期 调整持仓的持仓表
-            # 选取的index  period = 3  0,0,0,3,3,3,6...
-            list_take_hold = [[hold.index[int(i/period)*period]\
-                                for i in range(len(hold.index))]
-                    for hold in bar_hold]
-            list_hold = [bar_hold[i].loc[list_take_hold[i]]
-                    for i in range(len(bar_hold))]
-            # 提取的index非连续，复原到原来的连续交易日index
-            for hold in list_hold:
-                hold.index = bar_hold[0].index
-            mat_hold.append(list_hold)
-        self.mat_hold = mat_hold
-# 每个时间持仓标的数量
-    def matrix_holdn(self):
-        mat_holdn = []
-        for period_list in self.mat_hold:
-            list_holdn = [(i!=0).sum(axis=1) for i in period_list]
-            mat_holdn.append(list_holdn)
-        self.mat_holdn = mat_holdn 
-# matrix contri     每日净值对数收益率： np.log(matrix_contri[i_period][i_a_b].sum(axis=1)+1)
-    def matrix_contri(self):
-        mat_weight = []
-        mat_contri = []
-        for list_hold in self.mat_hold: 
-            # 合约市值权重  不是真实的市值 
-            list_cap = [hold * self.price for hold in list_hold]
-            list_weight = [cap.apply(lambda x: x/x.sum(), axis=1).fillna(0) for cap in list_cap]
-            # 当日收益(return*昨日weight)
-            list_contri = [(weight.shift()*self.returns).fillna(0) for weight in list_weight]
-            mat_contri.append(list_contri)
-            mat_weight.append(list_weight)
-        self.mat_contri = mat_contri
-        self.mat_weight = mat_weight
-# matrix logreturn  and returns
-    def matrix_lr(self):
-        mat_lr = []
-        mat_returns = []
-        for list_contri in self.mat_contri:
-            list_returns = [contri.sum(axis=1) for contri in list_contri]
-            list_lr = [np.log(returns+1) for returns in list_returns]
-            mat_lr.append(list_lr)
-            mat_returns.append(list_returns)
-        self.mat_lr = mat_lr
-        self.mat_returns = mat_returns
-    def matrix_turnover(self):
-        mat_turnover = []
-        # 假设当期没有换仓的权重与当期权重的差值即为换手率
-        # 换仓周期
-        for i in range(len(self.mat_weight)):
-            list_weight = self.mat_weight[i]
-            list_contri = self.mat_contri[i]
-            list_NoAdjustWeight = \
-                [list_weight[j].shift().fillna(0) + list_contri[j] for j in range(len(list_weight))]
-            list_NoAdjustWeight = [NoAdjustWeight.div(NoAdjustWeight.sum(axis=1), axis='rows') \
-                                   for NoAdjustWeight in list_NoAdjustWeight]
-            list_NoAdjustWeight = [NoAdjustWeight.fillna(0) for NoAdjustWeight in list_NoAdjustWeight]
-            list_turnover = \
-                [np.abs((list_weight[j]-list_NoAdjustWeight[j])).sum(axis=1) for j in range(len(list_weight))]
-            # 年化换手率
-            #list_turnover = [i.mean()*250 for i in list_turnover]
-            mat_turnover.append(list_turnover)
-        self.mat_turnover = mat_turnover
-    def get_result(self):
-        # 每一个period
-        for i in range(len(self.periods)):
-            #  每一个分组 每个时刻的每个分组收益率对其分组序号做回归
-            df_corr = pd.DataFrame()
-            for j in range(len(self.a_b)-1):
-                returns = pd.DataFrame(self.mat_returns[i][j])
-                returns['factor']=j
-                df_corr = pd.concat([df_corr, returns])
-            df_corr = df_corr.groupby('date').corr(method='spearman')
-            IC_series = df_corr.loc[(slice(None), 'factor'), 0]
-            # 因子指标
-            IC = IC_series.mean()
-            ICIR = IC/IC_series.std()
-            # 年化收益率和sharpe ratio
-            duryears = (self.returns.index[-1] - self.returns.index[0]).days/365
-            # 多空组合
-            LS_returns = self.mat_lr[i][-2] - self.mat_lr[i][0]
-            LS_std = LS_returns.std()*np.sqrt(250)
-            LS_return_annual = np.exp(LS_returns.sum()/duryears) - 1
-            LS_sharpe = (LS_return_annual-0.03)/LS_std
-            # 多头组合
-            L_returns = self.mat_lr[i][-2] 
-            L_std = L_returns.std()*np.sqrt(250)
-            L_return_annual = np.exp(L_returns.sum()/duryears) - 1
-            L_sharpe = (L_return_annual-0.03)/L_std
-            # 市场组合（等权）
-            M_returns = self.mat_lr[i][-1]
-            M_std = M_returns.std()*np.sqrt(250)
-            M_return_annual = np.exp(M_returns.sum()/duryears) - 1
-            M_sharpe = (M_return_annual-0.03)/M_std
-            # 多头换手率
-            turnover = self.mat_turnover[i][-2].mean()*250
-            # 考虑换手率造成的交易成本后的多头收益率
-            real_return = (L_return_annual+1)*(1-self.comm/10000)**(turnover) - 1
-            real_sharpe = (real_return-0.03)/L_std
-            record = {'group IC':IC, 'group ICIR':ICIR, 'L&S return': LS_return_annual, 
-                      'L return':L_return_annual, 'market return':M_return_annual, 
-                      'L&S sharpe':LS_sharpe, 'L sharpe':L_sharpe, 'market sharpe':M_sharpe, 
-                        'real return':real_return, 'real sharpe':real_sharpe, 'turnover':turnover}
-            self.result.loc[self.periods[i]] = record
-
-# plot
-# 因子组合收益（单边做多，考虑交易成本（默认单边万7））
-    def HoldReturn(self, i_period=0, dateleft=None, dateright=None, cost=0):
-        if dateleft==None:
-            dateleft = self.factor.index[0][0]
-        if dateright==None:
-            dateright = self.factor.index[-1][0]
-        plt, fig, ax = matplot()
-        ax2 = ax.twinx()
-        # 画图曲线颜色和透明度区分
-        # 不包含等权指数
-        if self.justdivide:
-            number = len(self.a_b)
-        else:
-            number = len(self.a_b)-1
-        number0 = int(number/2)
-        number1 = number - number0
-        #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
-        color_list = ['C2']*number0 + ['C3']*number1
-        # 颜色越靠近中心越浅
-        alpha0 = (np.arange(number0)+1)[::-1]/number0
-        alpha1 = (np.arange(number1)+1)/number1
-        alpha_list = np.append(alpha0, alpha1)
-        for i in range(number):
-            returns = self.mat_returns[i_period][i].loc[dateleft:dateright]
-#            ax.plot((1+returns).cumprod(), label=str(self.a_b[i]), alpha=0.3)
-            turnover = self.mat_turnover[i_period][i].loc[dateleft:dateright]
-            holdn = self.mat_holdn[i_period][i].loc[dateleft:dateright]
-            # 真实净值变化
-            returns = (1-turnover.shift().fillna(0)*cost/10000)*(1+returns)
-            #ax.plot(returns.cumprod(), label=str(self.a_b[i])+' 换手率=%.1f'%(turnover.mean()*250))
-            ax.plot(returns.cumprod(), c=color_list[i], alpha=alpha_list[i],\
-                    label=str(self.a_b[i])+' 换手=%.1f'%(turnover.mean()*250))
-            # 持有数量
-            #ax2.plot(holdn, c=color_list[i], alpha=alpha_list[i], ls='--')
-            ax2.plot(holdn, c=color_list[i], alpha=0.2, ls='--')
-        if not self.justdivide:
-            # 等权指数
-            returns = self.mat_returns[i_period][-1].loc[dateleft:dateright]
-            turnover = self.mat_turnover[i_period][-1].loc[dateleft:dateright]
-            returns = (1-turnover.shift().fillna(0)*cost/10000)*(1+returns)
-            ax.plot(returns.cumprod(), c='C1',\
-                    label='等权指数 '+' 换手=%.1f'%(turnover.mean()*250))
-        #ax.legend()
-        if number<8:
-            ax.legend(bbox_to_anchor=(0.5, -0.55), loc=8, ncol=2)
-        elif number<10:
-            ax.legend(bbox_to_anchor=(0.5, -0.65), loc=8, ncol=2)
-        else:
-            ax.legend(bbox_to_anchor=(0.5, -0.7), loc=8, ncol=2)
-        ax.set_title('调整频率: %d 日'%self.periods[i_period])
-        ax.set_ylabel('累计净值')
-        ax.set_xlim(dateleft, dateright)
-        #ax.set_xlabel('日期')
-        ax2.set_ylabel('持有数量')
-        plt.gcf().autofmt_xdate()
-        if 'output' in os.listdir():
-            pass
-        else:
-            os.mkdir('output')
-        plt.savefig('./output/alpha-Portfolio-HoldReturn.png',\
-                     bbox_inches='tight')
-        plt.show()
-# 各组对数收益率-等权对数收益率
-    def LogCompare(self, i_period=0, dateleft=None, dateright=None, ifbench=True):
-        if dateleft==None:
-            dateleft = self.factor.index[0][0]
-        if dateright==None:
-            dateright = self.factor.index[-1][0]
-        plt, fig, ax = matplot()
-        if ifbench:
-            benchmark = self.mat_lr[i_period][-1].cumsum()
-        else:
-            benchmark = 0
-        # 画图曲线颜色和透明度区分
-        # 等权指数不画
-        number = len(self.a_b)-1
-        number0 = int(number/2)
-        number1 = number - number0
-        #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
-        color_list = ['C2']*number0 + ['C3']*number1
-        # 颜色越靠近中心越浅
-        alpha0 = (np.arange(number0)+1)[::-1]/number0
-        alpha1 = (np.arange(number1)+1)/number1
-        alpha_list = np.append(alpha0, alpha1)
-        for i in range(number):
-            log_return = self.mat_lr[i_period][i].cumsum()
-            ax.plot(log_return - benchmark, \
-                    label=str(self.a_b[i]) + '%.1f'%(self.mat_turnover[i_period][i].mean()*250),
-                    c=color_list[i], alpha=alpha_list[i])
-        # 因子收益
-        LS = (self.mat_lr[i_period][-2] - self.mat_lr[i_period][0]).cumsum()
-        factor_return =  100*(np.exp(LS.iloc[-1])**(365/(LS.index[-1]-LS.index[0]).days)-1) 
-        ax.plot(LS, c='C0', label='L&S  anu.{r:.2f}%'.format(r=factor_return))
-        ax.legend()
-        ax.set_title('Period: %d bar(s)'%self.periods[i_period])
-        ax.set_ylabel('Cumulative Log Return')
-        ax.set_xlabel('Date')
-        ax.set_xlim(dateleft, dateright)
-        plt.gcf().autofmt_xdate()
-        if 'output' in os.listdir():
-            pass
-        else:
-            os.mkdir('output')
-        plt.savefig('./output/alpha-Portfolio-LogCompare.png',\
-                     bbox_inches='tight')
-        plt.show()
-# 柱状图
-    def Bar(self, i_period=0):
-        # 按年度划分收益率
-        df_returns = pd.concat(self.mat_lr[i_period], axis=1)\
-            .rename(columns=dict(zip(range(len(self.a_b)), self.a_b)))
-        df_returns['year'] = df_returns.index.year
-        df_returns = 100*(np.exp(df_returns.groupby('year').sum())-1)
-        # 作图
-        plt, fig, ax = matplot()
-        x = np.arange(len(df_returns))
-        width = 0.08
-        # 偏移量
-        move = np.arange(-len(self.a_b)*width/2,len(self.a_b)*width/2,width)
-        for n in range(len(self.a_b)):
-            ax.bar(np.arange(len(df_returns))+move[n], df_returns[self.a_b[n]].values,\
-                    width=width, label='%s'%(str(self.a_b[n])))
-        ax.legend(bbox_to_anchor=(0.5,-0.3), loc=10, ncol=3)
-        plt.xticks(x, list(df_returns.index), fontsize=20)
-        ax.set_ylabel("(%)")
-        if 'output' in os.listdir():
-            pass
-        else:
-            os.mkdir('output')
-        plt.savefig('./output/alpha-Portfolio-Bar.png',\
-                     bbox_inches='tight')
-        plt.show()
-# 各组分组因子值阈值和数量
-    def FactorThreshold(self):
-        plt, fig, ax = matplot()
-        # 颜色与LogCompare中相同，最大值和最小值为橙色C1
-        # 等权指数不画
-        number = len(self.a_b)-1
-        number0 = int(number/2)
-        number1 = number - number0
-        #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
-        color_list = ['C2']*number0 + ['C3']*number1
-        # 颜色越靠近中心越浅
-        alpha0 = (np.arange(number0)+1)[::-1]/number0
-        alpha1 = (np.arange(number1)+1)/number1
-        alpha_list = np.append(alpha0, alpha1)
-        ax2 = ax.twinx()
-        #ax.plot(self.threshold[0], label='low bound',
-        #        c='C1')
-        for i in range(number):
-            # 按分位数分组则显示因子值，按因子值分组则显示分位数
-            if self.norm==True:
-                #ax.plot(self.threshold[i+1].rolling(20).mean(), label=str(self.a_b[i][1]),
-                #    c=color_list[i], alpha=alpha_list[i])
-                ax.plot(self.threshold[i+1], label=str(self.a_b[i][1]),
-                    c=color_list[i], alpha=alpha_list[i])
-            else:
-                line = pd.Series(index=self.returns.index).copy()
-                line.loc[:] = self.threshold[i+1]
-                ax.plot(line, label=str(self.a_b[i][1]),
-                    c=color_list[i], alpha=alpha_list[i])
-            ax2.plot(self.group_number[i], ls='--', 
-                    c=color_list[i], alpha=alpha_list[i])
-        ax.legend()
-        ax.set_ylabel('Factor thershold')
-        # 避免显示异常值
-        ax2.set_ylabel('Factor group stock number')
-        ax.set_xlabel('Date')
-        ax.set_xlim(self.returns.index[0], self.returns.index[-1])
-        plt.gcf().autofmt_xdate()
-        if 'output' in os.listdir():
-            pass
-        else:
-            os.mkdir('output')
-        plt.savefig('./output/alpha-Portfolio-FactorThreshold.png',\
-                     bbox_inches='tight')
-        plt.show()
-
-
-
-# 因子分组计算
-# market, 分组变量1， 分组变量2， 分组数，取平均值变量(T日的未来收益)
-def FactorGroup(market, group_value0, group_value1=None,\
-        group_value0_num=5, group_value1_num=3, returns_key='f-returns', delay=0,\
-            level0s=None, level1s=None):
-    market_factor = market.copy()
-    if market_factor[group_value0].dtype in [float, np.int64]:
-        group0 = 'group_' + group_value0
-        market_factor[group0] = Rank(market_factor[group_value0]).groupby('code'\
-                                ).shift(delay).dropna().map(lambda x: int(x*group_value0_num))
-        #threshold = [market[group_value0].quantile(i/group_value0_num) \
-        #             for i in range(group_value0_num+1)]
-        #market_factor[group0] = pd.cut(market[group_value0],\
-        #                                bins=threshold).groupby('code').shift(delay).dropna()
-    else:
-        group0 = group_value0
-        market_factor[group0] = market_factor[group0].groupby('code').shift(delay).dropna()
-    if group_value1==None:
-        group = market_factor.groupby([group0, 'date'])
-        result_returns = group[returns_key].mean()
-
-        plt, fig, ax = matplot()
-        ax1 = ax.twinx()
-        for i in result_returns.index.get_level_values(0).unique():
-            ax.plot(result_returns.loc[i].cumsum(), label='group %s, %.2lf'%(i, \
-                        100*np.exp(250*result_returns.loc[i].mean())-100))
-            ax1.plot(group['close'].count().loc[i], alpha=0.3)
-        ax.legend()
-        ax.set_ylabel('累计收益率（单利）')
-        ax1.set_ylabel('分组个数')
-        ax.set_xlim(market_factor.index[0][0], market_factor.index[-1][0])
-        plt.savefig('MutiFactorGroup.png')
-        return
-    # 计算指标的分组标签
-    if market_factor[group_value1].dtype in [float, np.int64]:
-        group1 = 'group_' + group_value1
-        market_factor[group1] = Rank(market_factor[group_value1]).groupby('code'\
-                                ).shift(delay).dropna().map(lambda x: int(x*group_value1_num))
-    else:
-        group1 = group_value1
-        market_factor[group1] = market_factor[group1].groupby('code').shift(delay).dropna()
-    # 分组
-    tradeday = market_factor.index.get_level_values(0).unique()
-    group = market_factor.groupby([group0, group1, 'date'])
-    result_returns = group[returns_key].mean()
-    result_num = group['close'].count().loc[:, :, tradeday[-20]:tradeday[-1]]
-    if level0s==None:
-        level0s = result_returns.index.get_level_values(0).unique()
-    if level1s==None:
-        level1s = result_returns.index.get_level_values(1).unique()
-    # 结果矩阵（收益率、组内个数）
-    dict_returns = {}
-    dict_num = {}
-    for level0 in level0s:
-        for level1 in level1s:
-            try:
-                dict_returns[(level0, level1)] = \
-                    100*np.exp(250*result_returns.loc[level0, level1].mean())-100
-                dict_num[(level0, level1)] = result_num.loc[level0, level1].mean()
-            except:
-                dict_returns[(level0, level1)] = 0
-                dict_num[(level0, level1)] = 0
-    # 将绝对值转化为颜色
-    def color_map(x, min_r, max_r):
-        if x>0:
-            return [1,1-(x-min_r)/max_r,1-(x-min_r)/max_r]
-        elif x == 0:
-            return [1,1,1]
-        else:
-            return [1+(x-min_r)/max_r,1,1+(x-min_r)/max_r]
-    # 
-    plot = np.ones((len(level0s),len(level1s),3))
-    plt, fig, ax = matplot()
-    for level0 in range(len(level0s)):
-        for level1 in range(len(level1s)):
-            # 先列再行
-            plot[level0][level1] = color_map(dict_returns[(level0s[level0], level1s[level1])], \
-                                    0.9*min(dict_returns.values()), 1.1*max(dict_returns.values()))
-            # 先行再列
-            ax.text(level1, level0, 
-        round(dict_returns[(level0s[level0], level1s[level1])], 1),
-                ha='center', va='center')
-            ax.text(level1, level0, 
-        '    ' + str(int(dict_num[(level0s[level0], level1s[level1])])),
-                ha='left', va='top', fontsize=10, color='C0')
-    ax.imshow(plot, aspect='auto')
-    ax.set(xticks=list(range(len(level1s))))
-    ax.set_xticklabels([i for i in level1s])
-    ax.set_xlabel(group1)
-    ax.set(yticks=list(range(len(level0s))))
-    ax.set_yticklabels([i for i in level0s])
-    ax.set_ylabel(group0)
-    ax.set_title('双因子分组')
-    ax.grid(False)
-    plt.savefig('MutiFactorGroup.png')
-
-
-
-######################################################### 回归法 ####################################################################
-
-
-
-# 截面一元线性回归
-def cal_CrossReg(df, x_name, y_name, series=False):
-    name = y_name + '-' + x_name + '--alpha'
-
-    # 使用sm模块
-    result = df.groupby('date', sort=False).apply(lambda d: sm.OLS(d[y_name], sm.add_constant(d[x_name])).fit())
-    
-    # 如果d[x_name]中所有数相同为C且不为零，这时params中没有const，x_name为d[y_name].mean()/C
-    # rsquared为0
-    # 当d[x_name]全为0时，params['const']为0，params[x_name]为d[y_name].mean()
-    # rsquared可能为极小的负数
-    def func(x, name):
-        try:
-            return x.params[name]
-        except:
-            print('sm reg warning')
-            return 0
-    gamma = result.map(lambda x: func(x, 'const'))
-    beta = result.map(lambda x: func(x,x_name))
-    r = result.map(lambda x: np.sign(func(x, x_name))*np.sqrt(abs(x.rsquared)))
-
-    if series:
-        return beta, gamma, r
-    else:
-        df[name] = df.groupby('date').apply(lambda x: x[y_name] - beta[x.index[0][0]]*x[x_name] - gamma[x.index[0][0]]).values
-        return df
-    
-# 回归法
-# 此处回归获得的因子收益率即为回归的斜率，对应的是等权做多/做空因子值（标准化后）
-# 大于+/小于-0.302或者因子值最大/最小38.13%(61.87%)的组合收益
-# 直接market_factor标准的market以及因子column名
-class Reg():
-    # factor_name为IC_series列名
-    def __init__(self, factor, price, periods=(1, 5, 20), factor_name = 'alpha0', \
-                 gauss=False, point=True):
-        #import time
-        #start = time.time()
-        self.price = pd.DataFrame(price.rename('price')).pivot_table('price', 'date' ,'code')
-        self.periods = periods
-        self.point = point
-        if gauss:
-            factor = Gauss(factor)
-        else:
-            factor = Rank(factor, norm=True)
-        self.factor = factor
-        self.factor.name = factor_name
-        factor = pd.DataFrame(factor.rename('factor'))
-        # 输出结果 列：IC绝对值均值， IC均值， ICIR， 年化因子收益率， 年化夏普， 年化换手， 
-        # 交易成本万3\10\30
-        #   行：时间周期
-        result = pd.DataFrame(columns = ['absIC', 'IC', 'ICIR', 'annual return',\
-                     'sharpe', 'turnover',\
-                'comm3_r', 'comm3_s', 'comm10_r', 'comm10_s'])
-        result.index.name='period'
-        # 多周期IC\因子收益率序列
-        IC_dict = {}
-        #rankIC_dict = {}
-        fr_dict = {}
-        # 每日回归截距
-        gamma_dict = {}
-        cross_dict = {}
-        # 多空单位因子收益率组合平均换手率
-        turnover_dict = {}
-        #print(time.time()-start)
-        #start = time.time()
-        for period in self.periods:
-            if point: # 预测因子出现之后间隔n期的收益率
-                returns = ((self.price.shift(-1) - self.price)/self.price).shift(1-period)
-            else: # 预测收益率  预测n期内收益率
-                returns = (self.price.shift(-period) - self.price)/self.price
-            returns = returns.reset_index().melt(id_vars=['date']).\
-                sort_values(by='date').set_index(['date','code']).dropna()
-            # 合并df
-            df_corr = pd.concat([factor, returns], axis=1).dropna()
-            cross_dict[period] = df_corr
-            #print(time.time()-start)
-            #start = time.time()
-            ## 计算IC序列
-            beta, gamma, r = cal_CrossReg(df_corr, 'factor', 'value', True)
-            gamma_dict[period] = gamma
-            #print(time.time()-start)
-            #start = time.time()
-            # 因子指标
-            #rankIC_dict[period] = df_corr.groupby('date').corr(method='spearman')['factor'].loc[:, 'value']
-            #rankIC = rankIC_dict[period].mean()
-            IC_dict[period] = r
-            IC = r.mean()
-            ICIR = IC/r.std()
-            absIC = (abs(r)).mean()
-            # 因子收益率(单位预测周期 1day)
-            if point:
-                fr_dict[period] = beta
-                fr = beta.mean()
-            else:
-                fr_dict[period] = beta/period
-                fr = beta.mean()/period
-            frIR = np.sqrt(period)*fr/beta.std()
-            # 换手率
-            # 多头组合成分
-            factor_L = self.factor[self.factor>0.302].copy()
-            name = factor_L.name
-            factor_L = factor_L.reset_index()
-            factor_L[name] = 1
-            # 组合权重
-            weight_L = factor_L.pivot_table(name, 'date', 'code')
-            weight_L = weight_L.div(weight_L.sum(axis=1), axis='rows').fillna(0)
-            # 如果未调整period日后的组合权重
-            noadjust_weight = (weight_L.shift(period)*(self.price/self.price.shift(period)))[weight_L.columns]
-            noadjust_weight = noadjust_weight.div(noadjust_weight.sum(axis=1), axis='rows').fillna(0)
-            turnover_L = (abs(weight_L-noadjust_weight).sum(axis=1)).mean()/period
-            # 空头组合成分
-            factor_S = self.factor[self.factor<-0.302].copy()
-            name = factor_S.name
-            factor_S = factor_S.reset_index()
-            factor_S[name] = 1
-            # 组合权重
-            weight_S = factor_S.pivot_table(name, 'date', 'code')
-            weight_S = weight_S.div(weight_S.sum(axis=1), axis='rows').fillna(0)
-            # 如果未调整period日后的组合权重
-            noadjust_weight = (weight_S.shift(period)*(self.price/self.price.shift(period)))[weight_S.columns]
-            noadjust_weight = noadjust_weight.div(noadjust_weight.sum(axis=1), axis='rows').fillna(0)
-            turnover_S = (abs(weight_S-noadjust_weight).sum(axis=1)).mean()/period
-            turnover = ((turnover_S+turnover_L)/2).mean()*250
-            turnover_dict[period] = turnover
-            # 费后收益及夏普
-            comm3_return = ((1+250*fr)*(1-3/1e4)**turnover-1)
-            comm3_sharpe = comm3_return/(np.sqrt(250)*beta.std()) 
-            comm10_return = ((1+250*fr)*(1-10/1e4)**turnover-1)
-            comm10_sharpe = comm10_return/(np.sqrt(250)*beta.std()) 
-            #record = {'absIC':round(absIC*100,1), 'IC':round(IC*100,1), 'rankIC':round(100*rankIC,1),\
-            record = {'absIC':round(absIC*100,1), 'IC':round(IC*100,1),\
-                      'ICIR':round(10*ICIR,1), \
-                      'annual return':round(250*fr*100,1), \
-                      'sharpe':round(np.sqrt(250)*frIR,1), 'turnover':round(turnover,1),\
-                'comm3_r':round(100*comm3_return,1), 'comm3_s':round(comm3_sharpe,1),\
-                    'comm10_r':round(100*comm10_return,1), 'comm10_s':round(comm10_sharpe,1)}
-            result.loc[period] = record
-            #print(time.time()-start)
-            #start = time.time()
-        self.IC_dict = IC_dict
-        self.fr_dict = fr_dict
-        self.cross_dict = cross_dict
-        self.gamma_dict = gamma_dict
-        self.result = result
-        display(result)
-    # 因子收益率
-    def factor_return(self, period=1, rolling_period=20):
-        plt, fig, ax = matplot()
-        cumsum_fr = 250*self.fr_dict[period].cumsum()
-        ax.plot(cumsum_fr, label='累计因子收益率', c='C0')
-        ax.plot(cumsum_fr.rolling(20).min(),\
-                 alpha=0.5, c='C2')
-        ax.plot(cumsum_fr.rolling(20).max(),\
-                  alpha=0.5, c='C3')
-        ax.legend(loc='lower left')
-        ax.legend(bbox_to_anchor=(0.17, 1.06), loc=10, ncol=1)
-        ax2 = ax.twinx()
-        ax2.plot(250*self.fr_dict[period].rolling(rolling_period).mean(), label='滚动因子收益率（右）', c='C1')
-        #ax2.legend(loc='lower right')
-        ax2.legend(bbox_to_anchor=(0.78, 1.06), loc=10, ncol=1)
-        ax.set_xlim(self.factor.index[0][0], self.factor.index[-1][0])
-        plt.show() 
-    # 截面因子与收益率（散点图） n为分级靠档组数
-    def cross(self, date=None, period=1, n=100):
-        plt, fig, ax = matplot()
-        df_corr = self.cross_dict[period].copy()
-        if self.point:
-            beta = self.fr_dict[period]
-        else:
-            beta = self.fr_dict[period]*period
-        gamma = self.gamma_dict[period]
-        r = self.IC_dict[period]
-        if type(date)==type(None):
-            # 如果因子值少于n个（因子值重复过多）则不需要分级靠档
-            # 因子值按分位数分级靠档为n组
-            if len(df_corr['factor'].unique())<n:
-                factor_group = df_corr.groupby('factor')['value'].mean()
-            else:
-                threshold = [df_corr['factor'].quantile(i/n) for i in range(n+1)]
-                label = [(i+j)/2 for i,j in zip(threshold[:-1],threshold[1:])]
-                df_corr['factor_group'] = pd.cut(df_corr['factor'], bins=threshold, labels=label)
-                factor_group = df_corr.groupby('factor_group')['value'].mean()
-            ax.scatter(factor_group.index, factor_group.values, s=4)
-            ax.plot(np.linspace(-3,3,100), beta.mean()*np.linspace(-3,3,100) + gamma.mean(), c='C3')
-            plt.title('r = %.2lf beta(万) = %.2lf gamma(万) = %.2lf'%(r.mean(), beta.mean()*10000, gamma.mean()*10000))
-        else:
-            ax.scatter(df_corr.loc[date]['factor'], df_corr.loc[date]['value'])
-            ax.plot(np.linspace(-3,3,100), beta.loc[date]*np.linspace(-3,3,100) + gamma.loc[date], c='C3')
-            plt.title('r = %.2lf beta(万) = %.2lf gamma(万) = %.2lf'%(r.loc[date], beta.loc[date]*10000, gamma.loc[date]*10000))
-        plt.show()
-    # 因子自相关系数组合
-    def autocorr(self):
-        self.corr_dic = {}
-        for period in self.periods:
-            # 初始位置
-            factor_original = self.factor.copy()
-            factor_original.name = 'original'
-            factor_latter = self.factor.groupby('code').shift(period).copy()
-            factor_latter.name = 'latter'
-            self.corr_dic[period] = pd.concat([factor_original, factor_latter], axis=1).groupby('date').corr(method='pearson').loc[:, 'original', :]['latter'].mean()
-
-
-
-'''
-因子中性化函数
-market: index格式为date,code
-col1: str 被中心化列名
-col2: str 中心化参考列名
-group_num: int 分组数量;
-返回: seires, category
-'''
-def Factor_Neutralization(market, col1, col2, col1_group_num=5, col2_group_num=10):
-    def fun(x):
-        label1 = [i for i in range(col1_group_num)]
-        label2 = [i for i in range(col2_group_num)]
-        s = x.groupby(pd.qcut(x[col2], col2_group_num, labels=label2))\
-            .apply(lambda x: pd.qcut(x[col1], col1_group_num, labels=label1)).droplevel(0)
-        return s
-
-    df = market.copy(deep=True)
-    s = df.groupby(level='date').apply(lambda x: fun(x.droplevel(0)))
-    s.name = col1 + '_de' + col2
-    return s
-    
-
-
-
-
-
-
-
-
-
-
-
+import pandas as pd
+import numpy as np
+from scipy import stats
+import statsmodels.api as sm
+from FreeBack.post import matplot
+from FreeBack import my_pd
+import os
+# 该模块包含：
+# 因子计算常用函数
+# 单因子与多因子检验模块（组合法、回归法）
+
+
+#######################################################################################################
+####################################### 因子计算常用函数 #################################################
+#######################################################################################################
+# 无特殊说明下 factor,price的格式为pd.Series,其中index的格式为multiindex (date code)
+# Rank      
+# 每日全部index的因子值从小到大排序,均匀映射到(0,1)
+# Norm      
+# 将每日因子值在截面上标准化到 \mu = 0 \sigma = 1 分布
+# scale     
+# 使得截面上因子值满足sum(abs(x)) = 1(a) 
+# Gauss     
+# 将每日的因子值转化为正态分布
+# resample_fill/select  
+# 因子降频（日频因子换月频/周频）
+# QQ        绘制因子分布的QQ图，观察是否符合正态分布
+
+
+def Rank(factor, norm=False):
+    # 因子排名
+    rank = factor.groupby('date').rank()
+    if norm:
+        return 2*3**0.5*(rank/(rank.groupby('date').max()+1)-0.5)
+    return rank/(rank.groupby('date').max()+1)
+def Norm(factor):
+    return (factor - factor.groupby('date').mean())/factor.groupby('date').std()
+
+def scale(factor, a=1):
+    return a*factor/factor.groupby('date').apply(lambda x:abs(x).sum())
+# 通过正态分布累计概率函数的逆函数将[p,1-p]的均匀分布转化为正态分布，转换为正态分布后默认产生3sigma内的样本，99.7% p=0.003
+def Gauss(factor, p=0.003, slice=False):
+    # 开启slice选项时为仅转化一个截面启代表仅有一个截面数据
+    if not slice:
+        rank = factor.groupby('date').rank()
+        continuous = p/2+(1-p)*(rank-1)/(rank.groupby('date').max()-1)
+        def func(ser):
+            return ser.map(lambda x: stats.norm.ppf(x))
+        result = my_pd.parallel(continuous, func)
+        # 如果所有值相同则替换为0
+        if_same = result.groupby('date').apply(lambda x: (~x.duplicated()).sum())
+        result.loc[if_same[if_same==1].index] = 0
+        return result
+    else:
+        rank = factor.rank()
+        continuous = p/2+(1-p)*(rank-1)/(rank.max()-1)
+        return continuous.map(lambda x: stats.norm.ppf(x))
+# 每月、每周内的因子值替换为月初、周初因子值
+def resample_fill(factor, freq='month'):
+    factor.name=0
+    df = pd.DataFrame(factor)
+    df['th'] = df.index.map(lambda x:getattr(x[0], freq))
+    df['yesterday_th'] = df['th'].groupby('code').shift()
+    df = df.fillna(getattr(df.index[0][0], freq))
+    df['after'] = df.apply(lambda x: x[0] if x.th!=x.yesterday_th else np.nan, axis=1)
+    df = df.groupby('code').fillna(method='ffill')
+    df = df.groupby('code').fillna(method='bfill')
+    return df['after']
+# 直接只选用原数据的周初、月初值
+# 没有周一和1号的月份用下一个第一个出现的值***
+def resample_select(market, freq='month'):
+    if freq=='month':
+        return market[market.index.map(lambda x:getattr(x[0], 'day'))==1]
+    elif freq=='week':
+        return market[market.index.map(lambda x:getattr(x[0], 'weekday')())==0]
+def QQ(factor, date=None):
+    plt, fig, ax = matplot(w=6, d=4)
+    if date==None:
+        norm_dis = pd.Series(np.random.randn(len(factor))).sort_values()
+        ax.scatter(norm_dis, factor.sort_values())
+    else:
+        norm_dis = pd.Series(np.random.randn(len(factor.loc[date]))).sort_values()
+        ax.scatter(norm_dis, factor.loc[date].sort_values())
+    ax.plot(norm_dis, norm_dis, c='C3', ls='--')
+    ax.set_title('Q-Q plot')
+    ax.set_aspect('equal')
+    plt.show()
+
+
+
+#######################################################################################################
+######################################### 单因子检测 ####################################################
+#######################################################################################################
+# 1. 组合法， 计算各因子分层组合的收益及其他特征。
+    # Porfolio, 因子投资组合表现
+    # factorgroup
+# 2. 回归法， 假设截面上因子与未来收益率线性相关，计算该线性关系的一系列统计量。
+    # Reg
+
+########################################## 组合法 #######################################################
+
+class Portfolio():
+# factor 数据类型pd.Series, multiindex(date,code)   T日因子值(可以在此排除涨停板)
+# price 数据类型pd.Series, multiindex(date,code) T日交易价格(最宽松情况可以使用当日收盘价，\
+# 使用后一天开盘价或者VWAP等是接近实际情况的(全市场数据即可) 
+# norm 是否按照因子值的排序来对投资组合分组,默认开启。否则使用原始因子值进行分组 
+# divide 
+# 数据类型为tuple时，给出全部阈值确定连续分组；
+# 数据类型为list， 给出每个分组的前后阈值,例：[(0,0.1),(0.9,1)]表示选取最小10%和最大10%构建组合，前开后闭。
+# norm开启时，元素<=1时表示百分比，大于1时表示绝对数量，如(0,0.2)表示持有钱20%，(0，10)表示持有前十只。
+# 否则表示因子值的阈值。
+# justdivide 是否仅计算给出分组的收益而不计算全市场组合收益，默认计算全市场组合收益(权重由holdweight确定)
+# periods (1, 5, 20)同时计算1天5天20天轮动的结果
+# holdweight pd.Series, multiindex(data,code)  T日的投资组合权重，默认等权
+# comm 每次单边换手的交易成本，默认为0
+## 当日收益率为当日收盘价相对昨日收盘价收益率*前一日持仓权重
+## comm 不影响结果，仅仅在result中给出多头费后年化收益率 
+    def __init__(self, factor, price, norm=True, divide=(0, 0.2, 0.4, 0.6, 0.8, 1),\
+                 justdivide=False, periods=(1, ), \
+                  holdweight=None, comm=0):
+        self.comm = comm
+        self.norm = norm
+        self.justdivide=justdivide
+        # 一个确定持有张数（不去除停牌），一个确定收益率(去除停牌)
+        self.price = pd.DataFrame(price.rename('price')).pivot_table('price', 'date' ,'code')
+        # 每日收益率(当日收盘相比上日收盘)
+        returns = self.price/self.price.shift() - 1
+        self.returns = returns.fillna(0)
+#        # 先按照截面排序归一化
+        if norm:
+            self.factor = Rank(pd.DataFrame(factor.rename('factor')))
+        else:
+            self.factor = pd.DataFrame(factor.rename('factor'))
+        self.variable = factor
+        # 组合权重 
+        if type(holdweight) != type(None):
+            # 没有权重则按0计
+            holdweight = holdweight.fillna(0)
+            self.holdweight = holdweight.apply(lambda x: x/x.sum(), axis=1)
+        else:
+            self.holdweight = None
+        # 结果dataframe 行：时间周期  列：IC、ICIR（分组计算的IC、ICIR(非rank)）、 多空组合收益、多头收益、 等权收益、
+        # 考虑换手率多空收益、 夏普、 多空平均换手率
+        self.result = pd.DataFrame(columns=['group IC', 'group ICIR', 'L&S return', 'L return',\
+                 'market return', 'L&S sharpe', 'L sharpe', 'market sharpe', 'real return', \
+                    'real sharpe', 'turnover'])
+        self.result.index.name = 'holding period'
+        # 运行
+        self.run(divide, periods)
+    def run(self, divide, periods):
+        self.divide = divide
+        self.periods = periods
+        # self.a_b表示对因子分隔的阈值，如果是list则直接为a_b
+        if type(self.divide) == type(list()):
+            self.a_b = self.divide
+        # 如果是tuple则转化成list
+        else:
+            self.a_b = [(self.divide[i],self.divide[i+1]) for i in range(len(self.divide)-1)]
+        # 如果justdivide为False,则增加一个可以选中全部标的的组合
+        if not self.justdivide:
+            if self.norm == True:
+                # 按百分比划分
+                if self.a_b[-1][1]<=1:
+                    self.a_b = self.a_b + [(0,1)]
+                else:
+                    self.a_b = self.a_b + [(0, 99999)]
+            else:
+                self.a_b = self.a_b + [(self.factor.min().values[0], self.factor.max().values[0])]
+    # 生成持仓表 -> 获得 df_contri(index date  columns code) -> 获得净值每日对数收益率 -> 获得换手率
+    # 全部为矩阵操作
+        self.matrix_hold()
+        self.matrix_contri()
+        self.matrix_lr()
+        self.matrix_holdn()
+        self.matrix_turnover()
+        if not self.justdivide:
+            self.get_result()
+# mat[period][factor range]  list[factor range]
+# 获得每个持仓周期 每个因子区间的虚拟持仓(只保证比例关系正确) 
+# a_b factor range from a to b 区间内市值等权重
+    def matrix_hold(self):
+    # 每个bar按标的等权配置需要的持仓
+        if self.norm:
+            if self.a_b[-1][1]<=1:
+                look_factor = self.factor.groupby('date').rank(pct=True)
+            else:
+                print('整数排序')
+                look_factor = self.factor.groupby('date').rank()
+        else:
+            look_factor = self.factor
+        look_factor = look_factor.reset_index()
+        # 选取因子值 满足a_b list中全部条件的 放置于list_hold (前开后闭，与Rank函数返回的(0，1]对应)
+        bar_hold = [look_factor[(i[0]<look_factor['factor']) &\
+                                 (look_factor['factor']<=i[1])] for i in self.a_b]
+        # 每一组合选中的标的个数
+        self.group_number = [i.groupby('date').count() for i in bar_hold]
+        # 在date没有出现的code补np.nan
+        bar_hold = [pd.DataFrame(i.pivot_table('factor', 'date', 'code'),\
+                                 index=self.factor.index.get_level_values(0).unique())\
+                                     for i in bar_hold]
+        # 等权情况下持有标的的持仓数量为 1/price（持仓金额相等）
+        #bar_hold = [(i.isnull().replace([True,False],[0,1])*\
+        #             (1/self.price)).fillna(0) for i in bar_hold]
+        bar_hold = [((~i.isnull()).astype(int)*\
+                     (1/self.price)).fillna(0) for i in bar_hold]
+        # 当holdweight不为None时考虑此权重
+        if type(self.holdweight) != type(None):
+            bar_hold = [i*self.holdweight for i in bar_hold]
+        # 当period不等于1时需要按照period调整持仓
+        mat_hold = []
+        for period in self.periods:
+            # 以period为周期 调整持仓的持仓表
+            # 选取的index  period = 3  0,0,0,3,3,3,6...
+            list_take_hold = [[hold.index[int(i/period)*period]\
+                                for i in range(len(hold.index))]
+                    for hold in bar_hold]
+            list_hold = [bar_hold[i].loc[list_take_hold[i]]
+                    for i in range(len(bar_hold))]
+            # 提取的index非连续，复原到原来的连续交易日index
+            for hold in list_hold:
+                hold.index = bar_hold[0].index
+            mat_hold.append(list_hold)
+        self.mat_hold = mat_hold
+# 每个时间持仓标的数量
+    def matrix_holdn(self):
+        mat_holdn = []
+        for period_list in self.mat_hold:
+            list_holdn = [(i!=0).sum(axis=1) for i in period_list]
+            mat_holdn.append(list_holdn)
+        self.mat_holdn = mat_holdn 
+# matrix contri     每日净值对数收益率： np.log(matrix_contri[i_period][i_a_b].sum(axis=1)+1)
+    def matrix_contri(self):
+        mat_weight = []
+        mat_contri = []
+        for list_hold in self.mat_hold: 
+            # 合约市值权重  不是真实的市值 
+            list_cap = [hold * self.price for hold in list_hold]
+            list_weight = [cap.apply(lambda x: x/x.sum(), axis=1).fillna(0) for cap in list_cap]
+            # 当日收益(return*昨日weight)
+            list_contri = [(weight.shift()*self.returns).fillna(0) for weight in list_weight]
+            mat_contri.append(list_contri)
+            mat_weight.append(list_weight)
+        self.mat_contri = mat_contri
+        self.mat_weight = mat_weight
+# matrix logreturn  and returns
+    def matrix_lr(self):
+        mat_lr = []
+        mat_returns = []
+        for list_contri in self.mat_contri:
+            list_returns = [contri.sum(axis=1) for contri in list_contri]
+            list_lr = [np.log(returns+1) for returns in list_returns]
+            mat_lr.append(list_lr)
+            mat_returns.append(list_returns)
+        self.mat_lr = mat_lr
+        self.mat_returns = mat_returns
+    def matrix_turnover(self):
+        mat_turnover = []
+        # 假设当期没有换仓的权重与当期权重的差值即为换手率
+        # 换仓周期
+        for i in range(len(self.mat_weight)):
+            list_weight = self.mat_weight[i]
+            list_contri = self.mat_contri[i]
+            list_NoAdjustWeight = \
+                [list_weight[j].shift().fillna(0) + list_contri[j] for j in range(len(list_weight))]
+            list_NoAdjustWeight = [NoAdjustWeight.div(NoAdjustWeight.sum(axis=1), axis='rows') \
+                                   for NoAdjustWeight in list_NoAdjustWeight]
+            list_NoAdjustWeight = [NoAdjustWeight.fillna(0) for NoAdjustWeight in list_NoAdjustWeight]
+            list_turnover = \
+                [np.abs((list_weight[j]-list_NoAdjustWeight[j])).sum(axis=1) for j in range(len(list_weight))]
+            # 年化换手率
+            #list_turnover = [i.mean()*250 for i in list_turnover]
+            mat_turnover.append(list_turnover)
+        self.mat_turnover = mat_turnover
+    def get_result(self):
+        # 每一个period
+        for i in range(len(self.periods)):
+            #  每一个分组 每个时刻的每个分组收益率对其分组序号做回归
+            df_corr = pd.DataFrame()
+            for j in range(len(self.a_b)-1):
+                returns = pd.DataFrame(self.mat_returns[i][j])
+                returns['factor']=j
+                df_corr = pd.concat([df_corr, returns])
+            df_corr = df_corr.groupby('date').corr(method='spearman')
+            IC_series = df_corr.loc[(slice(None), 'factor'), 0]
+            # 因子指标
+            IC = IC_series.mean()
+            ICIR = IC/IC_series.std()
+            # 年化收益率和sharpe ratio
+            duryears = (self.returns.index[-1] - self.returns.index[0]).days/365
+            # 多空组合
+            LS_returns = self.mat_lr[i][-2] - self.mat_lr[i][0]
+            LS_std = LS_returns.std()*np.sqrt(250)
+            LS_return_annual = np.exp(LS_returns.sum()/duryears) - 1
+            LS_sharpe = (LS_return_annual-0.03)/LS_std
+            # 多头组合
+            L_returns = self.mat_lr[i][-2] 
+            L_std = L_returns.std()*np.sqrt(250)
+            L_return_annual = np.exp(L_returns.sum()/duryears) - 1
+            L_sharpe = (L_return_annual-0.03)/L_std
+            # 市场组合（等权）
+            M_returns = self.mat_lr[i][-1]
+            M_std = M_returns.std()*np.sqrt(250)
+            M_return_annual = np.exp(M_returns.sum()/duryears) - 1
+            M_sharpe = (M_return_annual-0.03)/M_std
+            # 多头换手率
+            turnover = self.mat_turnover[i][-2].mean()*250
+            # 考虑换手率造成的交易成本后的多头收益率
+            real_return = (L_return_annual+1)*(1-self.comm/10000)**(turnover) - 1
+            real_sharpe = (real_return-0.03)/L_std
+            record = {'group IC':IC, 'group ICIR':ICIR, 'L&S return': LS_return_annual, 
+                      'L return':L_return_annual, 'market return':M_return_annual, 
+                      'L&S sharpe':LS_sharpe, 'L sharpe':L_sharpe, 'market sharpe':M_sharpe, 
+                        'real return':real_return, 'real sharpe':real_sharpe, 'turnover':turnover}
+            self.result.loc[self.periods[i]] = record
+
+# plot
+# 因子组合收益（单边做多，考虑交易成本（默认单边万7））
+    def HoldReturn(self, i_period=0, dateleft=None, dateright=None, cost=0):
+        if dateleft==None:
+            dateleft = self.factor.index[0][0]
+        if dateright==None:
+            dateright = self.factor.index[-1][0]
+        plt, fig, ax = matplot()
+        ax2 = ax.twinx()
+        # 画图曲线颜色和透明度区分
+        # 不包含等权指数
+        if self.justdivide:
+            number = len(self.a_b)
+        else:
+            number = len(self.a_b)-1
+        number0 = int(number/2)
+        number1 = number - number0
+        #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
+        color_list = ['C2']*number0 + ['C3']*number1
+        # 颜色越靠近中心越浅
+        alpha0 = (np.arange(number0)+1)[::-1]/number0
+        alpha1 = (np.arange(number1)+1)/number1
+        alpha_list = np.append(alpha0, alpha1)
+        for i in range(number):
+            returns = self.mat_returns[i_period][i].loc[dateleft:dateright]
+#            ax.plot((1+returns).cumprod(), label=str(self.a_b[i]), alpha=0.3)
+            turnover = self.mat_turnover[i_period][i].loc[dateleft:dateright]
+            holdn = self.mat_holdn[i_period][i].loc[dateleft:dateright]
+            # 真实净值变化
+            returns = (1-turnover.shift().fillna(0)*cost/10000)*(1+returns)
+            #ax.plot(returns.cumprod(), label=str(self.a_b[i])+' 换手率=%.1f'%(turnover.mean()*250))
+            ax.plot(returns.cumprod(), c=color_list[i], alpha=alpha_list[i],\
+                    label=str(self.a_b[i])+' 换手=%.1f'%(turnover.mean()*250))
+            # 持有数量
+            #ax2.plot(holdn, c=color_list[i], alpha=alpha_list[i], ls='--')
+            ax2.plot(holdn, c=color_list[i], alpha=0.2, ls='--')
+        if not self.justdivide:
+            # 等权指数
+            returns = self.mat_returns[i_period][-1].loc[dateleft:dateright]
+            turnover = self.mat_turnover[i_period][-1].loc[dateleft:dateright]
+            returns = (1-turnover.shift().fillna(0)*cost/10000)*(1+returns)
+            ax.plot(returns.cumprod(), c='C1',\
+                    label='等权指数 '+' 换手=%.1f'%(turnover.mean()*250))
+        #ax.legend()
+        if number<8:
+            ax.legend(bbox_to_anchor=(0.5, -0.55), loc=8, ncol=2)
+        elif number<10:
+            ax.legend(bbox_to_anchor=(0.5, -0.65), loc=8, ncol=2)
+        else:
+            ax.legend(bbox_to_anchor=(0.5, -0.7), loc=8, ncol=2)
+        ax.set_title('调整频率: %d 日'%self.periods[i_period])
+        ax.set_ylabel('累计净值')
+        ax.set_xlim(dateleft, dateright)
+        #ax.set_xlabel('日期')
+        ax2.set_ylabel('持有数量')
+        plt.gcf().autofmt_xdate()
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-HoldReturn.png',\
+                     bbox_inches='tight')
+        plt.show()
+# 各组对数收益率-等权对数收益率
+    def LogCompare(self, i_period=0, dateleft=None, dateright=None, ifbench=True):
+        if dateleft==None:
+            dateleft = self.factor.index[0][0]
+        if dateright==None:
+            dateright = self.factor.index[-1][0]
+        plt, fig, ax = matplot()
+        if ifbench:
+            benchmark = self.mat_lr[i_period][-1].cumsum()
+        else:
+            benchmark = 0
+        # 画图曲线颜色和透明度区分
+        # 等权指数不画
+        number = len(self.a_b)-1
+        number0 = int(number/2)
+        number1 = number - number0
+        #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
+        color_list = ['C2']*number0 + ['C3']*number1
+        # 颜色越靠近中心越浅
+        alpha0 = (np.arange(number0)+1)[::-1]/number0
+        alpha1 = (np.arange(number1)+1)/number1
+        alpha_list = np.append(alpha0, alpha1)
+        for i in range(number):
+            log_return = self.mat_lr[i_period][i].cumsum()
+            ax.plot(log_return - benchmark, \
+                    label=str(self.a_b[i]) + '%.1f'%(self.mat_turnover[i_period][i].mean()*250),
+                    c=color_list[i], alpha=alpha_list[i])
+        # 因子收益
+        LS = (self.mat_lr[i_period][-2] - self.mat_lr[i_period][0]).cumsum()
+        factor_return =  100*(np.exp(LS.iloc[-1])**(365/(LS.index[-1]-LS.index[0]).days)-1) 
+        ax.plot(LS, c='C0', label='L&S  anu.{r:.2f}%'.format(r=factor_return))
+        ax.legend()
+        ax.set_title('Period: %d bar(s)'%self.periods[i_period])
+        ax.set_ylabel('Cumulative Log Return')
+        ax.set_xlabel('Date')
+        ax.set_xlim(dateleft, dateright)
+        plt.gcf().autofmt_xdate()
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-LogCompare.png',\
+                     bbox_inches='tight')
+        plt.show()
+# 柱状图
+    def Bar(self, i_period=0):
+        # 按年度划分收益率
+        df_returns = pd.concat(self.mat_lr[i_period], axis=1)\
+            .rename(columns=dict(zip(range(len(self.a_b)), self.a_b)))
+        df_returns['year'] = df_returns.index.year
+        df_returns = 100*(np.exp(df_returns.groupby('year').sum())-1)
+        # 作图
+        plt, fig, ax = matplot()
+        x = np.arange(len(df_returns))
+        width = 0.08
+        # 偏移量
+        move = np.arange(-len(self.a_b)*width/2,len(self.a_b)*width/2,width)
+        for n in range(len(self.a_b)):
+            ax.bar(np.arange(len(df_returns))+move[n], df_returns[self.a_b[n]].values,\
+                    width=width, label='%s'%(str(self.a_b[n])))
+        ax.legend(bbox_to_anchor=(0.5,-0.3), loc=10, ncol=3)
+        plt.xticks(x, list(df_returns.index), fontsize=20)
+        ax.set_ylabel("(%)")
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-Bar.png',\
+                     bbox_inches='tight')
+        plt.show()
+# 各组分组因子值阈值和数量
+    def FactorThreshold(self):
+        plt, fig, ax = matplot()
+        # 颜色与LogCompare中相同，最大值和最小值为橙色C1
+        # 等权指数不画
+        number = len(self.a_b)-1
+        number0 = int(number/2)
+        number1 = number - number0
+        #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
+        color_list = ['C2']*number0 + ['C3']*number1
+        # 颜色越靠近中心越浅
+        alpha0 = (np.arange(number0)+1)[::-1]/number0
+        alpha1 = (np.arange(number1)+1)/number1
+        alpha_list = np.append(alpha0, alpha1)
+        ax2 = ax.twinx()
+        #ax.plot(self.threshold[0], label='low bound',
+        #        c='C1')
+        for i in range(number):
+            # 按分位数分组则显示因子值，按因子值分组则显示分位数
+            if self.norm==True:
+                #ax.plot(self.threshold[i+1].rolling(20).mean(), label=str(self.a_b[i][1]),
+                #    c=color_list[i], alpha=alpha_list[i])
+                ax.plot(self.threshold[i+1], label=str(self.a_b[i][1]),
+                    c=color_list[i], alpha=alpha_list[i])
+            else:
+                line = pd.Series(index=self.returns.index).copy()
+                line.loc[:] = self.threshold[i+1]
+                ax.plot(line, label=str(self.a_b[i][1]),
+                    c=color_list[i], alpha=alpha_list[i])
+            ax2.plot(self.group_number[i], ls='--', 
+                    c=color_list[i], alpha=alpha_list[i])
+        ax.legend()
+        ax.set_ylabel('Factor thershold')
+        # 避免显示异常值
+        ax2.set_ylabel('Factor group stock number')
+        ax.set_xlabel('Date')
+        ax.set_xlim(self.returns.index[0], self.returns.index[-1])
+        plt.gcf().autofmt_xdate()
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-FactorThreshold.png',\
+                     bbox_inches='tight')
+        plt.show()
+
+
+
+# 因子分组计算
+# market, 分组变量1， 分组变量2， 分组数，取平均值变量(T日的未来收益)
+def FactorGroup(market, group_value0, group_value1=None,\
+        group_value0_num=5, group_value1_num=3, returns_key='f-returns', delay=0,\
+            level0s=None, level1s=None):
+    market_factor = market.copy()
+    if market_factor[group_value0].dtype in [float, np.int64]:
+        group0 = 'group_' + group_value0
+        market_factor[group0] = Rank(market_factor[group_value0]).groupby('code'\
+                                ).shift(delay).dropna().map(lambda x: int(x*group_value0_num))
+        #threshold = [market[group_value0].quantile(i/group_value0_num) \
+        #             for i in range(group_value0_num+1)]
+        #market_factor[group0] = pd.cut(market[group_value0],\
+        #                                bins=threshold).groupby('code').shift(delay).dropna()
+    else:
+        group0 = group_value0
+        market_factor[group0] = market_factor[group0].groupby('code').shift(delay).dropna()
+    if group_value1==None:
+        group = market_factor.groupby([group0, 'date'])
+        result_returns = group[returns_key].mean()
+
+        plt, fig, ax = matplot()
+        ax1 = ax.twinx()
+        for i in result_returns.index.get_level_values(0).unique():
+            ax.plot(result_returns.loc[i].cumsum(), label='group %s, %.2lf'%(i, \
+                        100*np.exp(250*result_returns.loc[i].mean())-100))
+            ax1.plot(group['close'].count().loc[i], alpha=0.3)
+        ax.legend()
+        ax.set_ylabel('累计收益率（单利）')
+        ax1.set_ylabel('分组个数')
+        ax.set_xlim(market_factor.index[0][0], market_factor.index[-1][0])
+        plt.savefig('MutiFactorGroup.png')
+        return
+    # 计算指标的分组标签
+    if market_factor[group_value1].dtype in [float, np.int64]:
+        group1 = 'group_' + group_value1
+        market_factor[group1] = Rank(market_factor[group_value1]).groupby('code'\
+                                ).shift(delay).dropna().map(lambda x: int(x*group_value1_num))
+    else:
+        group1 = group_value1
+        market_factor[group1] = market_factor[group1].groupby('code').shift(delay).dropna()
+    # 分组
+    tradeday = market_factor.index.get_level_values(0).unique()
+    group = market_factor.groupby([group0, group1, 'date'])
+    result_returns = group[returns_key].mean()
+    result_num = group['close'].count().loc[:, :, tradeday[-20]:tradeday[-1]]
+    if level0s==None:
+        level0s = result_returns.index.get_level_values(0).unique()
+    if level1s==None:
+        level1s = result_returns.index.get_level_values(1).unique()
+    # 结果矩阵（收益率、组内个数）
+    dict_returns = {}
+    dict_num = {}
+    for level0 in level0s:
+        for level1 in level1s:
+            try:
+                dict_returns[(level0, level1)] = \
+                    100*np.exp(250*result_returns.loc[level0, level1].mean())-100
+                dict_num[(level0, level1)] = result_num.loc[level0, level1].mean()
+            except:
+                dict_returns[(level0, level1)] = 0
+                dict_num[(level0, level1)] = 0
+    # 将绝对值转化为颜色
+    def color_map(x, min_r, max_r):
+        if x>0:
+            return [1,1-(x-min_r)/max_r,1-(x-min_r)/max_r]
+        elif x == 0:
+            return [1,1,1]
+        else:
+            return [1+(x-min_r)/max_r,1,1+(x-min_r)/max_r]
+    # 
+    plot = np.ones((len(level0s),len(level1s),3))
+    plt, fig, ax = matplot()
+    for level0 in range(len(level0s)):
+        for level1 in range(len(level1s)):
+            # 先列再行
+            plot[level0][level1] = color_map(dict_returns[(level0s[level0], level1s[level1])], \
+                                    0.9*min(dict_returns.values()), 1.1*max(dict_returns.values()))
+            # 先行再列
+            ax.text(level1, level0, 
+        round(dict_returns[(level0s[level0], level1s[level1])], 1),
+                ha='center', va='center')
+            ax.text(level1, level0, 
+        '    ' + str(int(dict_num[(level0s[level0], level1s[level1])])),
+                ha='left', va='top', fontsize=10, color='C0')
+    ax.imshow(plot, aspect='auto')
+    ax.set(xticks=list(range(len(level1s))))
+    ax.set_xticklabels([i for i in level1s])
+    ax.set_xlabel(group1)
+    ax.set(yticks=list(range(len(level0s))))
+    ax.set_yticklabels([i for i in level0s])
+    ax.set_ylabel(group0)
+    ax.set_title('双因子分组')
+    ax.grid(False)
+    plt.savefig('MutiFactorGroup.png')
+
+
+
+######################################################### 回归法 ####################################################################
+
+
+
+# 截面一元线性回归
+def cal_CrossReg(df, x_name, y_name, series=False):
+    name = y_name + '-' + x_name + '--alpha'
+
+    # 使用sm模块
+    result = df.groupby('date', sort=False).apply(lambda d: sm.OLS(d[y_name], sm.add_constant(d[x_name])).fit())
+    
+    # 如果d[x_name]中所有数相同为C且不为零，这时params中没有const，x_name为d[y_name].mean()/C
+    # rsquared为0
+    # 当d[x_name]全为0时，params['const']为0，params[x_name]为d[y_name].mean()
+    # rsquared可能为极小的负数
+    def func(x, name):
+        try:
+            return x.params[name]
+        except:
+            print('sm reg warning')
+            return 0
+    gamma = result.map(lambda x: func(x, 'const'))
+    beta = result.map(lambda x: func(x,x_name))
+    r = result.map(lambda x: np.sign(func(x, x_name))*np.sqrt(abs(x.rsquared)))
+
+    if series:
+        return beta, gamma, r
+    else:
+        df[name] = df.groupby('date').apply(lambda x: x[y_name] - beta[x.index[0][0]]*x[x_name] - gamma[x.index[0][0]]).values
+        return df
+    
+# 回归法
+# 此处回归获得的因子收益率即为回归的斜率，对应的是等权做多/做空因子值（标准化后）
+# 大于+/小于-0.302或者因子值最大/最小38.13%(61.87%)的组合收益
+# 直接market_factor标准的market以及因子column名
+class Reg():
+    # factor_name为IC_series列名
+    def __init__(self, factor, price, periods=(1, 5, 20), factor_name = 'alpha0', \
+                 gauss=False, point=True):
+        #import time
+        #start = time.time()
+        self.price = pd.DataFrame(price.rename('price')).pivot_table('price', 'date' ,'code')
+        self.periods = periods
+        self.point = point
+        if gauss:
+            factor = Gauss(factor)
+        else:
+            factor = Rank(factor, norm=True)
+        self.factor = factor
+        self.factor.name = factor_name
+        factor = pd.DataFrame(factor.rename('factor'))
+        # 输出结果 列：IC绝对值均值， IC均值， ICIR， 年化因子收益率， 年化夏普， 年化换手， 
+        # 交易成本万3\10\30
+        #   行：时间周期
+        result = pd.DataFrame(columns = ['absIC', 'IC', 'ICIR', 'annual return',\
+                     'sharpe', 'turnover',\
+                'comm3_r', 'comm3_s', 'comm10_r', 'comm10_s'])
+        result.index.name='period'
+        # 多周期IC\因子收益率序列
+        IC_dict = {}
+        #rankIC_dict = {}
+        fr_dict = {}
+        # 每日回归截距
+        gamma_dict = {}
+        cross_dict = {}
+        # 多空单位因子收益率组合平均换手率
+        turnover_dict = {}
+        #print(time.time()-start)
+        #start = time.time()
+        for period in self.periods:
+            if point: # 预测因子出现之后间隔n期的收益率
+                returns = ((self.price.shift(-1) - self.price)/self.price).shift(1-period)
+            else: # 预测收益率  预测n期内收益率
+                returns = (self.price.shift(-period) - self.price)/self.price
+            returns = returns.reset_index().melt(id_vars=['date']).\
+                sort_values(by='date').set_index(['date','code']).dropna()
+            # 合并df
+            df_corr = pd.concat([factor, returns], axis=1).dropna()
+            cross_dict[period] = df_corr
+            #print(time.time()-start)
+            #start = time.time()
+            ## 计算IC序列
+            beta, gamma, r = cal_CrossReg(df_corr, 'factor', 'value', True)
+            gamma_dict[period] = gamma
+            #print(time.time()-start)
+            #start = time.time()
+            # 因子指标
+            #rankIC_dict[period] = df_corr.groupby('date').corr(method='spearman')['factor'].loc[:, 'value']
+            #rankIC = rankIC_dict[period].mean()
+            IC_dict[period] = r
+            IC = r.mean()
+            ICIR = IC/r.std()
+            absIC = (abs(r)).mean()
+            # 因子收益率(单位预测周期 1day)
+            if point:
+                fr_dict[period] = beta
+                fr = beta.mean()
+            else:
+                fr_dict[period] = beta/period
+                fr = beta.mean()/period
+            frIR = np.sqrt(period)*fr/beta.std()
+            # 换手率
+            # 多头组合成分
+            factor_L = self.factor[self.factor>0.302].copy()
+            name = factor_L.name
+            factor_L = factor_L.reset_index()
+            factor_L[name] = 1
+            # 组合权重
+            weight_L = factor_L.pivot_table(name, 'date', 'code')
+            weight_L = weight_L.div(weight_L.sum(axis=1), axis='rows').fillna(0)
+            # 如果未调整period日后的组合权重
+            noadjust_weight = (weight_L.shift(period)*(self.price/self.price.shift(period)))[weight_L.columns]
+            noadjust_weight = noadjust_weight.div(noadjust_weight.sum(axis=1), axis='rows').fillna(0)
+            turnover_L = (abs(weight_L-noadjust_weight).sum(axis=1)).mean()/period
+            # 空头组合成分
+            factor_S = self.factor[self.factor<-0.302].copy()
+            name = factor_S.name
+            factor_S = factor_S.reset_index()
+            factor_S[name] = 1
+            # 组合权重
+            weight_S = factor_S.pivot_table(name, 'date', 'code')
+            weight_S = weight_S.div(weight_S.sum(axis=1), axis='rows').fillna(0)
+            # 如果未调整period日后的组合权重
+            noadjust_weight = (weight_S.shift(period)*(self.price/self.price.shift(period)))[weight_S.columns]
+            noadjust_weight = noadjust_weight.div(noadjust_weight.sum(axis=1), axis='rows').fillna(0)
+            turnover_S = (abs(weight_S-noadjust_weight).sum(axis=1)).mean()/period
+            turnover = ((turnover_S+turnover_L)/2).mean()*250
+            turnover_dict[period] = turnover
+            # 费后收益及夏普
+            comm3_return = ((1+250*fr)*(1-3/1e4)**turnover-1)
+            comm3_sharpe = comm3_return/(np.sqrt(250)*beta.std()) 
+            comm10_return = ((1+250*fr)*(1-10/1e4)**turnover-1)
+            comm10_sharpe = comm10_return/(np.sqrt(250)*beta.std()) 
+            #record = {'absIC':round(absIC*100,1), 'IC':round(IC*100,1), 'rankIC':round(100*rankIC,1),\
+            record = {'absIC':round(absIC*100,1), 'IC':round(IC*100,1),\
+                      'ICIR':round(10*ICIR,1), \
+                      'annual return':round(250*fr*100,1), \
+                      'sharpe':round(np.sqrt(250)*frIR,1), 'turnover':round(turnover,1),\
+                'comm3_r':round(100*comm3_return,1), 'comm3_s':round(comm3_sharpe,1),\
+                    'comm10_r':round(100*comm10_return,1), 'comm10_s':round(comm10_sharpe,1)}
+            result.loc[period] = record
+            #print(time.time()-start)
+            #start = time.time()
+        self.IC_dict = IC_dict
+        self.fr_dict = fr_dict
+        self.cross_dict = cross_dict
+        self.gamma_dict = gamma_dict
+        self.result = result
+        display(result)
+    # 因子收益率
+    def factor_return(self, period=1, rolling_period=20):
+        plt, fig, ax = matplot()
+        cumsum_fr = 250*self.fr_dict[period].cumsum()
+        ax.plot(cumsum_fr, label='累计因子收益率', c='C0')
+        ax.plot(cumsum_fr.rolling(20).min(),\
+                 alpha=0.5, c='C2')
+        ax.plot(cumsum_fr.rolling(20).max(),\
+                  alpha=0.5, c='C3')
+        ax.legend(loc='lower left')
+        ax.legend(bbox_to_anchor=(0.17, 1.06), loc=10, ncol=1)
+        ax2 = ax.twinx()
+        ax2.plot(250*self.fr_dict[period].rolling(rolling_period).mean(), label='滚动因子收益率（右）', c='C1')
+        #ax2.legend(loc='lower right')
+        ax2.legend(bbox_to_anchor=(0.78, 1.06), loc=10, ncol=1)
+        ax.set_xlim(self.factor.index[0][0], self.factor.index[-1][0])
+        plt.show() 
+    # 截面因子与收益率（散点图） n为分级靠档组数
+    def cross(self, date=None, period=1, n=100):
+        plt, fig, ax = matplot()
+        df_corr = self.cross_dict[period].copy()
+        if self.point:
+            beta = self.fr_dict[period]
+        else:
+            beta = self.fr_dict[period]*period
+        gamma = self.gamma_dict[period]
+        r = self.IC_dict[period]
+        if type(date)==type(None):
+            # 如果因子值少于n个（因子值重复过多）则不需要分级靠档
+            # 因子值按分位数分级靠档为n组
+            if len(df_corr['factor'].unique())<n:
+                factor_group = df_corr.groupby('factor')['value'].mean()
+            else:
+                threshold = [df_corr['factor'].quantile(i/n) for i in range(n+1)]
+                label = [(i+j)/2 for i,j in zip(threshold[:-1],threshold[1:])]
+                df_corr['factor_group'] = pd.cut(df_corr['factor'], bins=threshold, labels=label)
+                factor_group = df_corr.groupby('factor_group')['value'].mean()
+            ax.scatter(factor_group.index, factor_group.values, s=4)
+            ax.plot(np.linspace(-3,3,100), beta.mean()*np.linspace(-3,3,100) + gamma.mean(), c='C3')
+            plt.title('r = %.2lf beta(万) = %.2lf gamma(万) = %.2lf'%(r.mean(), beta.mean()*10000, gamma.mean()*10000))
+        else:
+            ax.scatter(df_corr.loc[date]['factor'], df_corr.loc[date]['value'])
+            ax.plot(np.linspace(-3,3,100), beta.loc[date]*np.linspace(-3,3,100) + gamma.loc[date], c='C3')
+            plt.title('r = %.2lf beta(万) = %.2lf gamma(万) = %.2lf'%(r.loc[date], beta.loc[date]*10000, gamma.loc[date]*10000))
+        plt.show()
+    # 因子自相关系数组合
+    def autocorr(self):
+        self.corr_dic = {}
+        for period in self.periods:
+            # 初始位置
+            factor_original = self.factor.copy()
+            factor_original.name = 'original'
+            factor_latter = self.factor.groupby('code').shift(period).copy()
+            factor_latter.name = 'latter'
+            self.corr_dic[period] = pd.concat([factor_original, factor_latter], axis=1).groupby('date').corr(method='pearson').loc[:, 'original', :]['latter'].mean()
+
+
+
+'''
+因子中性化函数
+market: index格式为date,code
+col1: str 被中心化列名
+col2: str 中心化参考列名
+group_num: int 分组数量;
+返回: seires, category
+'''
+def Factor_Neutralization(market, col1, col2, col1_group_num=5, col2_group_num=10):
+    def fun(x):
+        label1 = [i for i in range(col1_group_num)]
+        label2 = [i for i in range(col2_group_num)]
+        s = x.groupby(pd.qcut(x[col2], col2_group_num, labels=label2))\
+            .apply(lambda x: pd.qcut(x[col1], col1_group_num, labels=label1)).droplevel(0)
+        return s
+
+    df = market.copy(deep=True)
+    s = df.groupby(level='date').apply(lambda x: fun(x.droplevel(0)))
+    s.name = col1 + '_de' + col2
+    return s
+    
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `FreeBack-3.0.1a0/FreeBack/display.py` & `FreeBack-4.1.0a0/FreeBack/display.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,330 +1,332 @@
-import matplotlib.pyplot as plt
-import seaborn as sns
-from pyecharts import options as opts
-from pyecharts.charts import Kline,Bar,Grid,Line
-from pyecharts.commons.utils import JsCode
-import numpy as np
-
-###########################################################
-######################## 静态图 ###########################
-###########################################################
-
-
-# matplot绘图
-def matplot(r=1, c=1, sharex=False, sharey=False, w=8, d=5):
-    # don't use sns style
-    sns.reset_orig()
-    #plot
-    #run configuration 
-    plt.rcParams['font.size']=14
-    plt.rcParams['font.family'] = 'KaiTi'
-    #plt.rcParams['font.family'] = 'Arial'
-    plt.rcParams['font.sans-serif']=['Microsoft YaHei']
-    plt.rcParams["axes.unicode_minus"]=False #该语句解决图像中的“-”负号的乱码问题
-    plt.rcParams['axes.linewidth']=1
-    plt.rcParams['axes.grid']=True
-    plt.rcParams['grid.linestyle']='--'
-    plt.rcParams['grid.linewidth']=0.2
-    plt.rcParams["savefig.transparent"]='True'
-    plt.rcParams['lines.linewidth']=0.8
-    plt.rcParams['lines.markersize'] = 1
-    
-    #保证图片完全展示
-    plt.tight_layout()
-        
-    #subplot
-    fig,ax = plt.subplots(r,c,sharex=sharex, sharey=sharey,figsize=(w,d))
-    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, hspace = None, wspace=0.5)
-        
-    plt.gcf().autofmt_xdate()
-
-    return plt, fig, ax
-
-# 月度数据热力图  
-# period_value格式为 index month ‘2023-7-1’  value  0: ***
-# color_threshold 为红绿色分界点
-def month_thermal(period_value, color_threshold=0):   
-    # 数值>0红色，<0为绿色。转化为颜色[R,G,B]
-    def color_map(x, max_r):
-        if x>0:
-            return [1,1-x/max_r,1-x/max_r]
-        elif x == 0:
-            return [1,1,1]
-        else:
-            return [1+x/max_r,1,1+x/max_r]
-    # i 年份序号（纵坐标）  j 月份序号（横坐标） calendar是值， plot是颜色
-    def calendar_array(dates, data):
-    #    i, j = zip(*[d.isocalendar()[1:] for d in dates])
-    # 年份  月份 array
-        i, j = zip(*[(d.year,d.month) for d in dates])
-        i = np.array(i) - min(i)
-        j = np.array(j) - 1
-    # 总年份
-        ni = max(i) + 1
-    # 12个月
-    # 值 矩阵
-        calendar = np.nan * np.zeros((ni, 12))
-    # 颜色值 矩阵 默认白色[1,1,1]
-        plot =   np.ones((ni, 12, 3))
-        calendar[i, j] = data
-    # 绝对值最大为纯红（绿）
-        max_r = np.abs(data).max().max()
-        mat_color = [color_map(i-color_threshold,max_r) for i in data]
-        plot[i,j] = np.array(mat_color)
-        return i, j, plot, calendar
-
-    # 纵坐标为年份，横坐标为月份, 填充值
-    dates, data = list(period_value.index), period_value.iloc[:,0].values
-    i, j, plot, calendar = calendar_array(dates, data)
-    # 绘制热力图
-    plt, fig, ax = matplot()
-    ax.imshow(plot, aspect='auto')
-    # 设置纵坐标 年份
-    i = np.array(list(set(i)))
-    i.sort()
-    ax.set(yticks=i)
-    # 年份
-    years = list(set([i.year for i in period_value.index]))
-    ax.set_yticklabels(years)
-    # 设置横坐标 月份
-    j = np.array(list(set(j)))
-    j.sort()
-    ax.set(xticks=j)
-    ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
-                                'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
-    # 关闭网格
-    ax.grid(False)
-    # 显示数值
-    for i_ in i:
-        for j_ in j:
-            if not np.isnan(calendar[i_][j_]):
-                ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
-    return plt, fig, ax
-
-# 月度收益热力图    输入对数收益率的series 
-def plot_thermal(df_returns):
-    # 先转化为对数收益率
-    #df_lr = df_returns.apply(lambda x: np.log(x+1))
-    df_lr = df_returns.reset_index()
-    # 筛出同月数据
-    df_lr['month'] = df_lr['date'].apply(lambda x: x - datetime.timedelta(x.day-1))
-    df_lr = df_lr[['month', df_returns.name]]
-    df_lr = df_lr.set_index('month')
-    # 月度收益 %
-    period_return = (np.exp(df_lr.groupby('month').sum()) - 1)*100
-    # 收益率转化为颜色[R,G,B]
-    def color_map(x,max_r):
-        if x>0:
-            return [1,1-x/max_r,1-x/max_r]
-        elif x == 0:
-            return [1,1,1]
-        else:
-            return [1+x/max_r,1,1+x/max_r]
-    # i 年份序号（纵坐标）  j 月份序号（横坐标） calendar是值， plot是颜色
-    def calendar_array(dates, data):
-    #    i, j = zip(*[d.isocalendar()[1:] for d in dates])
-    # 年份  月份 array
-        i, j = zip(*[(d.year,d.month) for d in dates])
-        i = np.array(i) - min(i)
-        j = np.array(j) - 1
-    # 总年份
-        ni = max(i) + 1
-    # 12个月
-    # 收益率 矩阵
-        calendar = np.nan * np.zeros((ni, 12))
-    # 颜色值 矩阵 默认白色[1,1,1]
-        plot =   np.ones((ni, 12, 3))
-        calendar[i, j] = data
-    # 正最大收益为纯红 负最大收益为纯绿
-        max_r = np.abs(data).max().max()
-        mat_color = [color_map(i,max_r) for i in data]
-        plot[i,j] = np.array(mat_color)
-        return i, j, plot, calendar
-
-    # 纵坐标为年份，横坐标为月份, 填充值
-    dates, data = list(period_return.index), period_return.iloc[:,0].values
-    i, j, plot, calendar = calendar_array(dates, data)
-    # 绘制热力图
-    plt, fig, ax = matplot()
-    ax.imshow(plot, aspect='auto')
-    # 设置纵坐标 年份
-    i = np.array(list(set(i)))
-    i.sort()
-    ax.set(yticks=i)
-    # 年份
-    years = list(set([i.year for i in df_returns.index]))
-    ax.set_yticklabels(years)
-    # 设置横坐标 月份
-    j = np.array(list(set(j)))
-    j.sort()
-    ax.set(xticks=j)
-    ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
-                                'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
-    # 关闭网格
-    ax.grid(False)
-    # 显示数值
-    for i_ in i:
-        for j_ in j:
-            if not np.isnan(calendar[i_][j_]):
-                ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
-
-    return plt, fig, ax
-
-
-
-
-###########################################################
-######################## 动态交互图 ###########################
-###########################################################
-
-
-
-
-
-# plot_data:df格式,index为datetime,必要列为close,high,low,open,vol
-# 其他列自由添加，默认绘制于主图
-# 其中vol绘制于副图 其他列为指标列，绘制于主图
-def plot_kbar(plot_data, title='个股行情'):
-    # 画图大小
-    big_width = 1400
-    big_height = big_width*1000/1800
-    
-    # 主图，k线
-    kbar_data = plot_data[['open', 'close', 'low', 'high']].values.tolist()
-    kline = (
-        Kline()
-        .add_xaxis([str(i.date()) for i in plot_data.index])  # 日期坐标
-        .add_yaxis(                                           # k线
-            "kline",
-            kbar_data,
-            itemstyle_opts=opts.ItemStyleOpts(
-                color="#ec0000",
-                color0="#00da3c",
-                border_color="#8A0000",
-                border_color0="#008F28",
-            ),
-        )
-        .set_global_opts(
-            xaxis_opts=opts.AxisOpts(is_scale=True),
-            yaxis_opts=opts.AxisOpts(
-                is_scale=True,
-                splitarea_opts=opts.SplitAreaOpts(
-                    is_show=True, areastyle_opts=opts.AreaStyleOpts(opacity=1)
-                ),
-            ),
-            ## 滑块控制主图和幅图，滑块位置, 滑块起始左边位置，起始右边位置
-            # 隐藏幅图的滑轨
-            datazoom_opts=[\
-                opts.DataZoomOpts(type_='inside', xaxis_index=[0,1],\
-                                             #pos_top='60%', pos_bottom='65%',\
-                                             range_start=80,\
-                                             range_end=100,)],
-            ## 鼠标位于图中任意点展示详细信息 
-            tooltip_opts=opts.TooltipOpts(
-                    trigger="axis",
-                    axis_pointer_type="cross",
-                    background_color="rgba(245, 245, 245, 0.8)",
-                    border_width=1,
-                    border_color="#ccc",
-                    textstyle_opts=opts.TextStyleOpts(color="#000"),
-                ),
-            ##
-            #visualmap_opts=opts.VisualMapOpts(
-            #        is_show=False,
-            #        dimension=2,
-            #        series_index=5,
-            #        is_piecewise=True,
-            #        pieces=[
-            #            {"value": 1, "color": "#00da3c"},
-            #            {"value": -1, "color": "#ec0000"},
-            #        ],
-            #    ),
-            # 在主图显示幅图详情
-            axispointer_opts=opts.AxisPointerOpts(
-                    is_show=True,
-                    link=[{"xAxisIndex": "all"}],
-                    label=opts.LabelOpts(background_color="#777"),
-                ),
-            # 绘制阴影功能
-            brush_opts=opts.BrushOpts(
-                    x_axis_index="all",
-                    brush_link="all",
-                    out_of_brush={"colorAlpha": 0.1},
-                    brush_type="lineX",
-                ),
-            # 标题
-            title_opts=opts.TitleOpts(title="%s"%title),)
-        )
-    # 主图上绘制的其他数据
-    kline_others = (set(plot_data.columns)-set(['close', 'high','low','open','vol']))
-    lines_list = []
-    for i in kline_others:
-        lines_list.append((Line()
-                .add_xaxis(xaxis_data=[str(i.date()) for i in plot_data.index])
-                .add_yaxis(
-                    series_name=i,
-                    y_axis=plot_data[i].tolist(),
-                    xaxis_index=1,
-                    yaxis_index=1,
-                    label_opts=opts.LabelOpts(is_show=False),)
-            ))
-    # 子图1，成交量
-    bar = (
-            Bar()
-            .add_xaxis(xaxis_data=[str(i.date()) for i in plot_data.index])
-            .add_yaxis(
-                series_name="vol",
-                y_axis=plot_data["vol"].tolist(),
-                xaxis_index=1,
-                yaxis_index=1,
-                label_opts=opts.LabelOpts(is_show=False),
-                itemstyle_opts=opts.ItemStyleOpts(
-                    # 跟随主图颜色
-                    color=JsCode(
-                        """
-                    function(params) {
-                        var colorList;
-                        if (barData[params.dataIndex][1] > barData[params.dataIndex][0]) {
-                            colorList = '#ef232a';
-                        } else {
-                            colorList = '#14b143';
-                        }
-                        return colorList;
-                    }
-                    """
-                    )
-                ),
-            )\
-            .set_global_opts(
-                xaxis_opts=opts.AxisOpts(
-                    type_="category",
-                    grid_index=1,
-                    axislabel_opts=opts.LabelOpts(is_show=False),
-                ),
-                legend_opts=opts.LegendOpts(is_show=False),
-            ))
-    # 总图
-    grid_chart = Grid(
-            init_opts=opts.InitOpts(
-                width="%spx"%(big_width),
-                height="%spx"%(big_height),
-                animation_opts=opts.AnimationOpts(animation=False),
-            )
-        )
-    ## 导入open、close数据到barData改变交易量每个bar的颜色
-    grid_chart.add_js_funcs("var barData={}".format(plot_data[["open","close"]].values.tolist()))
-    # 添加主图，副图
-    for i in lines_list:
-        overlap_kline = kline.overlap(i)
-    grid_chart.add(
-            overlap_kline,
-            #kline,
-            grid_opts=opts.GridOpts(pos_left="0%", pos_right="0%", height="60%"),
-        )
-    grid_chart.add(
-            bar,
-            grid_opts=opts.GridOpts(
-                pos_left="0%", pos_right="0%", pos_top="70%", height="20%"
-            ),
-        )
-    grid_chart.render("个股行情.html")
+import matplotlib.pyplot as plt
+from mpl_toolkits.axisartist.parasite_axes import HostAxes, ParasiteAxes
+import seaborn as sns
+from pyecharts import options as opts
+from pyecharts.charts import Kline,Bar,Grid,Line
+from pyecharts.commons.utils import JsCode
+import numpy as np
+import datetime
+
+###########################################################
+######################## 静态图 ###########################
+###########################################################
+
+
+# matplot绘图
+def matplot(r=1, c=1, sharex=False, sharey=False, w=13, d=7):
+    # don't use sns style
+    sns.reset_orig()
+    #plot
+    #run configuration 
+    plt.rcParams['font.size']=14
+    plt.rcParams['font.family'] = 'KaiTi'
+    #plt.rcParams['font.family'] = 'Arial'
+    plt.rcParams['font.sans-serif']=['Microsoft YaHei']
+    plt.rcParams["axes.unicode_minus"]=False #该语句解决图像中的“-”负号的乱码问题
+    plt.rcParams['axes.linewidth']=1
+    plt.rcParams['axes.grid']=True
+    plt.rcParams['grid.linestyle']='--'
+    plt.rcParams['grid.linewidth']=0.2
+    plt.rcParams["savefig.transparent"]='True'
+    plt.rcParams['lines.linewidth']=0.8
+    plt.rcParams['lines.markersize'] = 1
+    
+    #保证图片完全展示
+    plt.tight_layout()
+        
+    #subplot
+    fig,ax = plt.subplots(r,c,sharex=sharex, sharey=sharey,figsize=(w,d))
+    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, hspace = None, wspace=0.5)
+        
+    plt.gcf().autofmt_xdate()
+
+    return plt, fig, ax
+
+# 月度数据热力图  
+# period_value格式为 index month ‘2023-7-1’  value  0: ***
+# color_threshold 为红绿色分界点
+def month_thermal(period_value, color_threshold=0):   
+    # 数值>0红色，<0为绿色。转化为颜色[R,G,B]
+    def color_map(x, max_r):
+        if x>0:
+            return [1,1-x/max_r,1-x/max_r]
+        elif x == 0:
+            return [1,1,1]
+        else:
+            return [1+x/max_r,1,1+x/max_r]
+    # i 年份序号（纵坐标）  j 月份序号（横坐标） calendar是值， plot是颜色
+    def calendar_array(dates, data):
+    #    i, j = zip(*[d.isocalendar()[1:] for d in dates])
+    # 年份  月份 array
+        i, j = zip(*[(d.year,d.month) for d in dates])
+        i = np.array(i) - min(i)
+        j = np.array(j) - 1
+    # 总年份
+        ni = max(i) + 1
+    # 12个月
+    # 值 矩阵
+        calendar = np.nan * np.zeros((ni, 12))
+    # 颜色值 矩阵 默认白色[1,1,1]
+        plot =   np.ones((ni, 12, 3))
+        calendar[i, j] = data
+    # 绝对值最大为纯红（绿）
+        max_r = np.abs(data).max().max()
+        mat_color = [color_map(i-color_threshold,max_r) for i in data]
+        plot[i,j] = np.array(mat_color)
+        return i, j, plot, calendar
+
+    # 纵坐标为年份，横坐标为月份, 填充值
+    dates, data = list(period_value.index), period_value.iloc[:,0].values
+    i, j, plot, calendar = calendar_array(dates, data)
+    # 绘制热力图
+    plt, fig, ax = matplot()
+    ax.imshow(plot, aspect='auto')
+    # 设置纵坐标 年份
+    i = np.array(list(set(i)))
+    i.sort()
+    ax.set(yticks=i)
+    # 年份
+    years = list(set([i.year for i in period_value.index]))
+    ax.set_yticklabels(years)
+    # 设置横坐标 月份
+    j = np.array(list(set(j)))
+    j.sort()
+    ax.set(xticks=j)
+    ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
+                                'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
+    # 关闭网格
+    ax.grid(False)
+    # 显示数值
+    for i_ in i:
+        for j_ in j:
+            if not np.isnan(calendar[i_][j_]):
+                ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
+    return plt, fig, ax
+
+# 月度收益热力图    输入对数收益率的series 
+def plot_thermal(df_returns):
+    # 先转化为对数收益率
+    #df_lr = df_returns.apply(lambda x: np.log(x+1))
+    df_lr = df_returns.reset_index()
+    # 筛出同月数据
+    df_lr['month'] = df_lr['date'].apply(lambda x: x - datetime.timedelta(x.day-1))
+    df_lr = df_lr[['month', df_returns.name]]
+    df_lr = df_lr.set_index('month')
+    # 月度收益 %
+    period_return = (np.exp(df_lr.groupby('month').sum()) - 1)*100
+    # 收益率转化为颜色[R,G,B]
+    def color_map(x,max_r):
+        if x>0:
+            return [1,1-x/max_r,1-x/max_r]
+        elif x == 0:
+            return [1,1,1]
+        else:
+            return [1+x/max_r,1,1+x/max_r]
+    # i 年份序号（纵坐标）  j 月份序号（横坐标） calendar是值， plot是颜色
+    def calendar_array(dates, data):
+    #    i, j = zip(*[d.isocalendar()[1:] for d in dates])
+    # 年份  月份 array
+        i, j = zip(*[(d.year,d.month) for d in dates])
+        i = np.array(i) - min(i)
+        j = np.array(j) - 1
+    # 总年份
+        ni = max(i) + 1
+    # 12个月
+    # 收益率 矩阵
+        calendar = np.nan * np.zeros((ni, 12))
+    # 颜色值 矩阵 默认白色[1,1,1]
+        plot =   np.ones((ni, 12, 3))
+        calendar[i, j] = data
+    # 正最大收益为纯红 负最大收益为纯绿
+        max_r = np.abs(data).max().max()
+        mat_color = [color_map(i,max_r) for i in data]
+        plot[i,j] = np.array(mat_color)
+        return i, j, plot, calendar
+
+    # 纵坐标为年份，横坐标为月份, 填充值
+    dates, data = list(period_return.index), period_return.iloc[:,0].values
+    i, j, plot, calendar = calendar_array(dates, data)
+    # 绘制热力图
+    plt, fig, ax = matplot()
+    ax.imshow(plot, aspect='auto')
+    # 设置纵坐标 年份
+    i = np.array(list(set(i)))
+    i.sort()
+    ax.set(yticks=i)
+    # 年份
+    years = list(set([i.year for i in df_returns.index]))
+    ax.set_yticklabels(years)
+    # 设置横坐标 月份
+    j = np.array(list(set(j)))
+    j.sort()
+    ax.set(xticks=j)
+    ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
+                                'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
+    # 关闭网格
+    ax.grid(False)
+    # 显示数值
+    for i_ in i:
+        for j_ in j:
+            if not np.isnan(calendar[i_][j_]):
+                ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
+
+    return plt, fig, ax
+
+
+
+
+###########################################################
+######################## 动态交互图 ###########################
+###########################################################
+
+
+
+
+
+# plot_data:df格式,index为datetime,必要列为close,high,low,open,vol
+# 其他列自由添加，默认绘制于主图
+# 其中vol绘制于副图 其他列为指标列，绘制于主图
+def plot_kbar(plot_data, title='个股行情'):
+    # 画图大小
+    big_width = 1400
+    big_height = big_width*1000/1800
+    
+    # 主图，k线
+    kbar_data = plot_data[['open', 'close', 'low', 'high']].values.tolist()
+    kline = (
+        Kline()
+        .add_xaxis([str(i.date()) for i in plot_data.index])  # 日期坐标
+        .add_yaxis(                                           # k线
+            "kline",
+            kbar_data,
+            itemstyle_opts=opts.ItemStyleOpts(
+                color="#ec0000",
+                color0="#00da3c",
+                border_color="#8A0000",
+                border_color0="#008F28",
+            ),
+        )
+        .set_global_opts(
+            xaxis_opts=opts.AxisOpts(is_scale=True),
+            yaxis_opts=opts.AxisOpts(
+                is_scale=True,
+                splitarea_opts=opts.SplitAreaOpts(
+                    is_show=True, areastyle_opts=opts.AreaStyleOpts(opacity=1)
+                ),
+            ),
+            ## 滑块控制主图和幅图，滑块位置, 滑块起始左边位置，起始右边位置
+            # 隐藏幅图的滑轨
+            datazoom_opts=[\
+                opts.DataZoomOpts(type_='inside', xaxis_index=[0,1],\
+                                             #pos_top='60%', pos_bottom='65%',\
+                                             range_start=80,\
+                                             range_end=100,)],
+            ## 鼠标位于图中任意点展示详细信息 
+            tooltip_opts=opts.TooltipOpts(
+                    trigger="axis",
+                    axis_pointer_type="cross",
+                    background_color="rgba(245, 245, 245, 0.8)",
+                    border_width=1,
+                    border_color="#ccc",
+                    textstyle_opts=opts.TextStyleOpts(color="#000"),
+                ),
+            ##
+            #visualmap_opts=opts.VisualMapOpts(
+            #        is_show=False,
+            #        dimension=2,
+            #        series_index=5,
+            #        is_piecewise=True,
+            #        pieces=[
+            #            {"value": 1, "color": "#00da3c"},
+            #            {"value": -1, "color": "#ec0000"},
+            #        ],
+            #    ),
+            # 在主图显示幅图详情
+            axispointer_opts=opts.AxisPointerOpts(
+                    is_show=True,
+                    link=[{"xAxisIndex": "all"}],
+                    label=opts.LabelOpts(background_color="#777"),
+                ),
+            # 绘制阴影功能
+            brush_opts=opts.BrushOpts(
+                    x_axis_index="all",
+                    brush_link="all",
+                    out_of_brush={"colorAlpha": 0.1},
+                    brush_type="lineX",
+                ),
+            # 标题
+            title_opts=opts.TitleOpts(title="%s"%title),)
+        )
+    # 主图上绘制的其他数据
+    kline_others = (set(plot_data.columns)-set(['close', 'high','low','open','vol']))
+    lines_list = []
+    for i in kline_others:
+        lines_list.append((Line()
+                .add_xaxis(xaxis_data=[str(i.date()) for i in plot_data.index])
+                .add_yaxis(
+                    series_name=i,
+                    y_axis=plot_data[i].tolist(),
+                    xaxis_index=1,
+                    yaxis_index=1,
+                    label_opts=opts.LabelOpts(is_show=False),)
+            ))
+    # 子图1，成交量
+    bar = (
+            Bar()
+            .add_xaxis(xaxis_data=[str(i.date()) for i in plot_data.index])
+            .add_yaxis(
+                series_name="vol",
+                y_axis=plot_data["vol"].tolist(),
+                xaxis_index=1,
+                yaxis_index=1,
+                label_opts=opts.LabelOpts(is_show=False),
+                itemstyle_opts=opts.ItemStyleOpts(
+                    # 跟随主图颜色
+                    color=JsCode(
+                        """
+                    function(params) {
+                        var colorList;
+                        if (barData[params.dataIndex][1] > barData[params.dataIndex][0]) {
+                            colorList = '#ef232a';
+                        } else {
+                            colorList = '#14b143';
+                        }
+                        return colorList;
+                    }
+                    """
+                    )
+                ),
+            )\
+            .set_global_opts(
+                xaxis_opts=opts.AxisOpts(
+                    type_="category",
+                    grid_index=1,
+                    axislabel_opts=opts.LabelOpts(is_show=False),
+                ),
+                legend_opts=opts.LegendOpts(is_show=False),
+            ))
+    # 总图
+    grid_chart = Grid(
+            init_opts=opts.InitOpts(
+                width="%spx"%(big_width),
+                height="%spx"%(big_height),
+                animation_opts=opts.AnimationOpts(animation=False),
+            )
+        )
+    ## 导入open、close数据到barData改变交易量每个bar的颜色
+    grid_chart.add_js_funcs("var barData={}".format(plot_data[["open","close"]].values.tolist()))
+    # 添加主图，副图
+    for i in lines_list:
+        overlap_kline = kline.overlap(i)
+    grid_chart.add(
+            overlap_kline,
+            #kline,
+            grid_opts=opts.GridOpts(pos_left="0%", pos_right="0%", height="60%"),
+        )
+    grid_chart.add(
+            bar,
+            grid_opts=opts.GridOpts(
+                pos_left="0%", pos_right="0%", pos_top="70%", height="20%"
+            ),
+        )
+    grid_chart.render("个股行情.html")
```

### Comparing `FreeBack-3.0.1a0/FreeBack/event.py` & `FreeBack-4.1.0a0/FreeBack/event.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-import pandas as pd
-import numpy as np
-from FreeBack.post import matplot
-from FreeBack.my_pd import parallel_group
-
-
-class Event():
-    '''
-    事件驱动测试
-    参数格式:
-    multi——index: date, code
-    signal: 入场信号,index格式
-    price: series
-    before: int, 事件前天数
-    after: int, 事件后天数
-    bench_type: zero:零, equal:等权
-    '''
-    def __init__(self, signal, price, before=5, after=30, bench_type='zero',\
-                  custom_bench=None, n_core=6, fast=True):
-        self.signal = signal
-        self.price = price
-        self.before = before
-        self.after = after
-        self.n_core = n_core
-        self.bench_type = bench_type
-        self.custom_bench = custom_bench
-        if fast:
-            self.fast_init()
-        else:
-            self.init_param()
-    
-    def sr(self, x):
-        sr = (x - x.shift(1))/x.shift(1)
-        return sr
-        
-    def init_param(self):
-        def fun1(x):
-            r = pd.DataFrame()
-            for i in cols:
-                r.loc[:, i] = x.shift(-i)
-            return r
-
-        self.length = self.before + self.after
-        self.sr = self.price.groupby('code').apply(lambda x: self.sr(x)).droplevel(0).sort_index(level=0)
-        # 基准按照等权计算
-        self.bench_sr = self.sr.groupby('date').mean()
-        if self.bench_type == 'zero':
-            self.bench_sr = pd.Series(index=self.bench_sr.index)
-            self.bench_sr.fillna(0, inplace=True)
-        elif self.bench_type == 'equal':
-            self.bench_sr = self.bench_sr
-        if type(self.custom_bench)==type(None):
-            self.bench_sr = self.custom_bench.loc[self.bench_sr.index]
-        self.sr = self.sr - self.bench_sr
-        self.sr.name = 'sr'
-        cols = [i-self.before+1 for i in range(self.length)]
-        self.signal_sr_df = parallel_group(self.sr, fun1, n_core=self.n_core).loc[self.signal]
-        self.number = self.signal_sr_df[0].groupby(level='date').count()
-        self.bench_net = (self.bench_sr + 1).cumprod()
-        self.net = (self.signal_sr_df+1).cumprod(axis=1)
-
-    def fast_init(self):
-        self.length = self.before + self.after
-        self.sr = (self.price/self.price.groupby('code').shift() - 1).fillna(0)
-        # 基准收益率，默认为0
-        self.bench_sr = self.sr.groupby('date').mean()
-        if self.bench_type == 'zero':
-            self.bench_sr = pd.Series(index=self.bench_sr.index)
-            self.bench_sr.fillna(0, inplace=True)
-        elif self.bench_type == 'equal':
-            self.bench_sr = self.bench_sr
-        self.sr = self.sr - self.bench_sr
-        self.sr.name = 'sr'
-        # 前后观察收益率
-        cols = [i-self.before+1 for i in range(self.length)]
-        signal_sr_df = pd.concat([self.sr.groupby('code').shift(-i) for i in cols], axis=1)
-        signal_sr_df.columns = cols
-        self.signal_sr_df = signal_sr_df.loc[self.signal].copy()
-        self.signal_sr_df.fillna(0, inplace=True)
-        # 触发次数
-        self.number = self.signal_sr_df[0].groupby(level='date').count()
-        # 净值
-        self.bench_net = (self.bench_sr + 1).cumprod()
-        self.net = (self.signal_sr_df+1).cumprod(axis=1)
-
-    # 每日触发信号数量, bench_type zero时没有bench
-    def draw_turnover(self):
-        plt0, fig0, ax0 = matplot()
-        ax1 = ax0.twinx()
-        num = self.number
-        ax1.plot(num.cumsum(), color='C2', label='累计样本量（右）')
-        # 触发次数过多的截断
-        index = num[num > (num.mean() + 5*num.std())].index
-        num.loc[index] = num.mean() + 5*num.std()
-        ax0.bar(num.index, num.values, color='grey', label='每日样本量')
-        #if self.bench_type != 'zero':
-            #ax1.plot(self.bench_net, color='steelblue', label='基准净值（右）')
-        #fig0.legend(bbox_to_anchor=(0.5, 0), loc=10, ncol=2)
-        fig0.legend(loc='lower center', ncol=2)
-        plt0.show()
-    
-    # 每日超额, 事件净值(取均值)
-    def draw_net(self):
-        plt0, fig0, ax0 = matplot()
-        sr = self.signal_sr_df.mean(axis=0)
-        ax0.bar(sr.index, sr.values, width=0.5,  label='单日超额', color='darkgoldenrod')
-        ax1 = ax0.twinx()
-        net = self.net.mean()
-        net = net/net.loc[1]
-        ax1.plot(net, color='crimson', label='累计净值（右）', linewidth=2.0)
-        ax1.hlines(1, sr.index[0], sr.index[-1], colors='k', linestyles='--')
-        fig0.legend(loc='lower center', ncol=2)
-        plt0.show()
-    
-    def draw_Kelly(self, direct='long'):
-        # 信号触发后价格变化结果
-        trade_result = (self.signal_sr_df.iloc[:, self.before+1:]+1).cumprod(axis=1)-1
-        # 胜率
-        winrate = (trade_result>0).sum()/len(trade_result.index)
-        # 赔率 按最大值
-        win = (trade_result*(trade_result>0)).replace(0, np.nan).max()
-        loss = (abs(trade_result)*(trade_result<0)).replace(0, np.nan).max()
-        odds = win/(loss+win)
-        # 根据交易多空修改赔率胜率
-        if direct=='short':
-            win,loss = loss,win
-            odds = win/(loss+win)
-            winrate = 1-winrate
-        ## Kelly公式确定仓位，负仓位为0
-        ## 收益率分布
-        ##plt, fig, ax = post.matplot()
-        ##sns.histplot(trade_result[2])
-        ##plt.show()
-        position = (winrate*win - (1-winrate)*loss)/(win*loss)
-        position[position<0] = 0
-        # 作图
-        plt, fig, ax = matplot()
-        ax.plot(100*winrate, c='C2', label='胜率')
-        ax.plot(100*odds, c='C0', label='赔率')
-        ax1 = ax.twinx()
-        ax1.plot(position, c='C3', label='最佳仓位')
-        ax.set_ylabel('（%）')
-        ax.set_xlabel('bar')
-        fig.legend(loc='lower center', ncol=3)
-        plt.show()
-
-
-    # 净值累计加减一个方差
-    def draw_std_net(self):
-        plt1, fig1, ax1 = matplot()
-        net = self.net.loc[:, 1:]
-        net_mean = net.mean()
-        net_up = net_mean + self.net.std()
-        net_low = net_mean - self.net.std()
-        ax1.plot(net_mean, color='darkblue', linewidth=2.0, label='均值')
-        ax1.plot(net_up, color='darkred', linewidth=2.0, label='均值+方差')
-        ax1.plot(net_low, color='darkgreen', linewidth=2.0, label='均值-方差')
-        ax1.legend(loc='upper left')
-        plt1.show()
-    
-    # 净值累计最大值&净值最小值
-    def draw_e_ratio(self):
-        plt1, fig1, ax1 = matplot()
-        net = self.net.loc[:, 1:]
-        net_max = net.cummax(axis=1).mean()
-        net_min = net.cummin(axis=1).mean()
-        e_ratio = net_max/net_min
-        ax1.plot(e_ratio, color='darkred', linewidth=2.0)
-        ax1.set_xlabel('set_xlabel')
-        plt1.show()
-    
-    # 仅一个信号
-    # i是siganl中第i个信号
-    def draw_one_signal_net(self, date, code):
-        plt0, fig0, ax0 = matplot()
-        sr = self.signal_sr_df.loc[date, code]
-        ax0.bar(sr.index, sr.values, width=0.5,  label='单日超额', color='darkgoldenrod')
-        ax1 = ax0.twinx()
-        net = self.net.loc[date, code]
-        net = net/net.loc[1]
-        ax1.plot(net, color='crimson', label='累计净值', linewidth=2.0)
-        fig0.legend(loc='lower center')
-        plt0.show()
-
-
-
-
-# # 在事件发生后，持有n日后(事件次bar open至+Tbar收盘价（T=0为次bar开盘至收盘的收益）)，收益率
-# #dict_date:  key thscode, value list of date(事件后可以买入的日期)
-# # hold_days = list(range(61))
-# #df_price:   date thscode  open close
-# def event_return(dict_date, df_price, hold_days):
-#     # 建立dataframe 前两列为合约与日期
-#     columns = ['thscode', 'date']
-#     # return_1 代表持有1天，即当天(0)的收盘价与开盘价之比
-#     for i in hold_days:
-#         columns.append('return_%d'%(i+1))
-#     df_return = pd.DataFrame(columns = columns)
-#     # 每个合约
-#     for i in list(dict_date.keys()):
-#         # 事件日期列表
-#         list_date = dict_date[i]
-#         # 如果在行情数据中没有,输出，跳过
-#         if(i not in df_price.thscode.unique()):
-#             print('not found',i)
-#             continue
-#         # 筛选出此合约行情
-#         df_ = df_price[df_price.thscode == i]
-#         # 按日期排序
-#         df_ = df_.sort_values(by = 'date')
-#         df_ = df_.reset_index(drop=True)
-#         # 每一次事件
-#         for start_date in list_date:
-#             # 公告日期为实际发布公告日期后次日，在此时可以直接买入
-#             # 为交易日则直接买入 
-#             if start_date in df_.date.values:
-#                 start = df_[df_.date == start_date]
-#             # 如果不是交易日则后延
-#             else:
-#                 # 最多尝试30天
-#                 try_num = 0
-#                 while try_num < 30:
-#                     try_num += 1
-#                     start_date += datetime.timedelta(1)
-#                     if start_date in df_.date.values:
-#                         start = df_[df_.date == start_date]
-#                         break
-#                 # 没有找到则下一个日期或转债
-#                 if(try_num==30):
-#                     print('fail: ', i, start_date)
-#                     continue
-#             # 持有到end，需存在行情数据
-#             dur = [start.index[0]+dur_i for dur_i in hold_days if (start.index[0]+dur_i) < len(df_.index)]
-#             end = df_.loc[dur]
-#     #       公告日开盘价到持有日收盘价 收益率
-#             return_list = list((end.close/start.open.values[0]).apply(lambda x: math.log(x)))
-#         # 字典 value
-#             dict_values = [i,start_date]
-#             dict_values.extend(return_list)
-#             append_dict = dict(zip(columns, dict_values))
-#             df_return = df_return.append(append_dict, ignore_index=True)
-        
+import pandas as pd
+import numpy as np
+from FreeBack.post import matplot
+from FreeBack.my_pd import parallel_group
+
+
+class Event():
+    '''
+    事件驱动测试
+    参数格式:
+    multi——index: date, code
+    signal: 入场信号,index格式
+    price: series
+    before: int, 事件前天数
+    after: int, 事件后天数
+    bench_type: zero:零, equal:等权
+    '''
+    def __init__(self, signal, price, before=5, after=30, bench_type='zero',\
+                  custom_bench=None, n_core=6, fast=True):
+        self.signal = signal
+        self.price = price
+        self.before = before
+        self.after = after
+        self.n_core = n_core
+        self.bench_type = bench_type
+        self.custom_bench = custom_bench
+        if fast:
+            self.fast_init()
+        else:
+            self.init_param()
+    
+    def sr(self, x):
+        sr = (x - x.shift(1))/x.shift(1)
+        return sr
+        
+    def init_param(self):
+        def fun1(x):
+            r = pd.DataFrame()
+            for i in cols:
+                r.loc[:, i] = x.shift(-i)
+            return r
+
+        self.length = self.before + self.after
+        self.sr = self.price.groupby('code').apply(lambda x: self.sr(x)).droplevel(0).sort_index(level=0)
+        # 基准按照等权计算
+        self.bench_sr = self.sr.groupby('date').mean()
+        if self.bench_type == 'zero':
+            self.bench_sr = pd.Series(index=self.bench_sr.index)
+            self.bench_sr.fillna(0, inplace=True)
+        elif self.bench_type == 'equal':
+            self.bench_sr = self.bench_sr
+        if type(self.custom_bench)==type(None):
+            self.bench_sr = self.custom_bench.loc[self.bench_sr.index]
+        self.sr = self.sr - self.bench_sr
+        self.sr.name = 'sr'
+        cols = [i-self.before+1 for i in range(self.length)]
+        self.signal_sr_df = parallel_group(self.sr, fun1, n_core=self.n_core).loc[self.signal]
+        self.number = self.signal_sr_df[0].groupby(level='date').count()
+        self.bench_net = (self.bench_sr + 1).cumprod()
+        self.net = (self.signal_sr_df+1).cumprod(axis=1)
+
+    def fast_init(self):
+        self.length = self.before + self.after
+        self.sr = (self.price/self.price.groupby('code').shift() - 1).fillna(0)
+        # 基准收益率，默认为0
+        self.bench_sr = self.sr.groupby('date').mean()
+        if self.bench_type == 'zero':
+            self.bench_sr = pd.Series(index=self.bench_sr.index)
+            self.bench_sr.fillna(0, inplace=True)
+        elif self.bench_type == 'equal':
+            self.bench_sr = self.bench_sr
+        self.sr = self.sr - self.bench_sr
+        self.sr.name = 'sr'
+        # 前后观察收益率
+        cols = [i-self.before+1 for i in range(self.length)]
+        signal_sr_df = pd.concat([self.sr.groupby('code').shift(-i) for i in cols], axis=1)
+        signal_sr_df.columns = cols
+        self.signal_sr_df = signal_sr_df.loc[self.signal].copy()
+        self.signal_sr_df.fillna(0, inplace=True)
+        # 触发次数
+        self.number = self.signal_sr_df[0].groupby(level='date').count()
+        # 净值
+        self.bench_net = (self.bench_sr + 1).cumprod()
+        self.net = (self.signal_sr_df+1).cumprod(axis=1)
+
+    # 每日触发信号数量, bench_type zero时没有bench
+    def draw_turnover(self):
+        plt0, fig0, ax0 = matplot()
+        ax1 = ax0.twinx()
+        num = self.number
+        ax1.plot(num.cumsum(), color='C2', label='累计样本量（右）')
+        # 触发次数过多的截断
+        index = num[num > (num.mean() + 5*num.std())].index
+        num.loc[index] = num.mean() + 5*num.std()
+        ax0.bar(num.index, num.values, color='grey', label='每日样本量')
+        #if self.bench_type != 'zero':
+            #ax1.plot(self.bench_net, color='steelblue', label='基准净值（右）')
+        #fig0.legend(bbox_to_anchor=(0.5, 0), loc=10, ncol=2)
+        fig0.legend(loc='lower center', ncol=2)
+        plt0.show()
+    
+    # 每日超额, 事件净值(取均值)
+    def draw_net(self):
+        plt0, fig0, ax0 = matplot()
+        sr = self.signal_sr_df.mean(axis=0)
+        ax0.bar(sr.index, sr.values, width=0.5,  label='单日超额', color='darkgoldenrod')
+        ax1 = ax0.twinx()
+        net = self.net.mean()
+        net = net/net.loc[1]
+        ax1.plot(net, color='crimson', label='累计净值（右）', linewidth=2.0)
+        ax1.hlines(1, sr.index[0], sr.index[-1], colors='k', linestyles='--')
+        fig0.legend(loc='lower center', ncol=2)
+        plt0.show()
+    
+    def draw_Kelly(self, direct='long'):
+        # 信号触发后价格变化结果
+        trade_result = (self.signal_sr_df.iloc[:, self.before+1:]+1).cumprod(axis=1)-1
+        # 胜率
+        winrate = (trade_result>0).sum()/len(trade_result.index)
+        # 赔率 按最大值
+        win = (trade_result*(trade_result>0)).replace(0, np.nan).max()
+        loss = (abs(trade_result)*(trade_result<0)).replace(0, np.nan).max()
+        odds = win/(loss+win)
+        # 根据交易多空修改赔率胜率
+        if direct=='short':
+            win,loss = loss,win
+            odds = win/(loss+win)
+            winrate = 1-winrate
+        ## Kelly公式确定仓位，负仓位为0
+        ## 收益率分布
+        ##plt, fig, ax = post.matplot()
+        ##sns.histplot(trade_result[2])
+        ##plt.show()
+        position = (winrate*win - (1-winrate)*loss)/(win*loss)
+        position[position<0] = 0
+        # 作图
+        plt, fig, ax = matplot()
+        ax.plot(100*winrate, c='C2', label='胜率')
+        ax.plot(100*odds, c='C0', label='赔率')
+        ax1 = ax.twinx()
+        ax1.plot(position, c='C3', label='最佳仓位')
+        ax.set_ylabel('（%）')
+        ax.set_xlabel('bar')
+        fig.legend(loc='lower center', ncol=3)
+        plt.show()
+
+
+    # 净值累计加减一个方差
+    def draw_std_net(self):
+        plt1, fig1, ax1 = matplot()
+        net = self.net.loc[:, 1:]
+        net_mean = net.mean()
+        net_up = net_mean + self.net.std()
+        net_low = net_mean - self.net.std()
+        ax1.plot(net_mean, color='darkblue', linewidth=2.0, label='均值')
+        ax1.plot(net_up, color='darkred', linewidth=2.0, label='均值+方差')
+        ax1.plot(net_low, color='darkgreen', linewidth=2.0, label='均值-方差')
+        ax1.legend(loc='upper left')
+        plt1.show()
+    
+    # 净值累计最大值&净值最小值
+    def draw_e_ratio(self):
+        plt1, fig1, ax1 = matplot()
+        net = self.net.loc[:, 1:]
+        net_max = net.cummax(axis=1).mean()
+        net_min = net.cummin(axis=1).mean()
+        e_ratio = net_max/net_min
+        ax1.plot(e_ratio, color='darkred', linewidth=2.0)
+        ax1.set_xlabel('set_xlabel')
+        plt1.show()
+    
+    # 仅一个信号
+    # i是siganl中第i个信号
+    def draw_one_signal_net(self, date, code):
+        plt0, fig0, ax0 = matplot()
+        sr = self.signal_sr_df.loc[date, code]
+        ax0.bar(sr.index, sr.values, width=0.5,  label='单日超额', color='darkgoldenrod')
+        ax1 = ax0.twinx()
+        net = self.net.loc[date, code]
+        net = net/net.loc[1]
+        ax1.plot(net, color='crimson', label='累计净值', linewidth=2.0)
+        fig0.legend(loc='lower center')
+        plt0.show()
+
+
+
+
+# # 在事件发生后，持有n日后(事件次bar open至+Tbar收盘价（T=0为次bar开盘至收盘的收益）)，收益率
+# #dict_date:  key thscode, value list of date(事件后可以买入的日期)
+# # hold_days = list(range(61))
+# #df_price:   date thscode  open close
+# def event_return(dict_date, df_price, hold_days):
+#     # 建立dataframe 前两列为合约与日期
+#     columns = ['thscode', 'date']
+#     # return_1 代表持有1天，即当天(0)的收盘价与开盘价之比
+#     for i in hold_days:
+#         columns.append('return_%d'%(i+1))
+#     df_return = pd.DataFrame(columns = columns)
+#     # 每个合约
+#     for i in list(dict_date.keys()):
+#         # 事件日期列表
+#         list_date = dict_date[i]
+#         # 如果在行情数据中没有,输出，跳过
+#         if(i not in df_price.thscode.unique()):
+#             print('not found',i)
+#             continue
+#         # 筛选出此合约行情
+#         df_ = df_price[df_price.thscode == i]
+#         # 按日期排序
+#         df_ = df_.sort_values(by = 'date')
+#         df_ = df_.reset_index(drop=True)
+#         # 每一次事件
+#         for start_date in list_date:
+#             # 公告日期为实际发布公告日期后次日，在此时可以直接买入
+#             # 为交易日则直接买入 
+#             if start_date in df_.date.values:
+#                 start = df_[df_.date == start_date]
+#             # 如果不是交易日则后延
+#             else:
+#                 # 最多尝试30天
+#                 try_num = 0
+#                 while try_num < 30:
+#                     try_num += 1
+#                     start_date += datetime.timedelta(1)
+#                     if start_date in df_.date.values:
+#                         start = df_[df_.date == start_date]
+#                         break
+#                 # 没有找到则下一个日期或转债
+#                 if(try_num==30):
+#                     print('fail: ', i, start_date)
+#                     continue
+#             # 持有到end，需存在行情数据
+#             dur = [start.index[0]+dur_i for dur_i in hold_days if (start.index[0]+dur_i) < len(df_.index)]
+#             end = df_.loc[dur]
+#     #       公告日开盘价到持有日收盘价 收益率
+#             return_list = list((end.close/start.open.values[0]).apply(lambda x: math.log(x)))
+#         # 字典 value
+#             dict_values = [i,start_date]
+#             dict_values.extend(return_list)
+#             append_dict = dict(zip(columns, dict_values))
+#             df_return = df_return.append(append_dict, ignore_index=True)
+        
 #     return df_return
```

### Comparing `FreeBack-3.0.1a0/FreeBack/my_pd.py` & `FreeBack-4.1.0a0/FreeBack/my_pd.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-import pandas as pd
-import numpy as np
-from numpy_ext import rolling_apply
-from joblib import Parallel, delayed
-import copy, math
-
-# 关于pandas经常使用到的一些操作 以及对现有函数的改进
-
-# dataframe, 查找的列， 为value时删除，包括np.nan 
-# return 操作后df 与被删除的df
-def drop_row(df, col, value_list):
-    drop_all = pd.DataFrame(columns = df.columns)
-    for value in value_list:
-        # nan特殊处理
-        if type(value) == type(np.nan):
-            if np.isnan(value):
-                # 重新排序
-                df = df.reset_index(drop = True)
-                beishanchu = df[df[col].isnull() == True]
-                df = df.drop(df.index[df[col].isnull() == True].values)
-                df = df.reset_index(drop = True)
-        else:
-            df = df.reset_index(drop = True)
-            beishanchu = df[df[col] == value]
-            df = df.drop(df.index[df[col] == value].values)
-            df = df.reset_index(drop = True)
-        drop_all = pd.concat([drop_all, beishanchu], ignore_index=True)
-    return df, drop_all
-
-# merge的改进， 避免列被重新命名(新加的为a_，并且保持on的列不变
-def nmerge(df, df_add, on):
-    new_name = ['a_' + x for x in df_add.columns]
-    new_name = dict(zip(df_add.columns,new_name))
-    df_add = df_add.rename(columns = new_name)
-    # 将 on 列 改回
-    new_name = ['a_' + x for x in on]
-    new_name = dict(zip(new_name,on))
-    # on
-    df_add = df_add.rename(columns = new_name)
-
-    # merge
-    return df.merge(df_add, on=on)
-
-# 将df中所有行按照年份划分，返回一个列表包含各年度的行，从最早开始
-def divide_row(df):
-    first_year = df['date'].min().year
-    last_year = df['date'].max().year
-    result = []
-    for y in range(first_year, last_year+1):
-        select = list(map(lambda x: x.year==y, df['date']))
-        df_ = df[select]
-        result.append(df_)
-    return result
-
-# 按sortby排序，使用unique_id列第一次出现的行组成新的df
-def extract_first(df, unique_id = 'thscode', sortby = 'date'):
-    df_result = pd.DataFrame(columns = df.columns)
-    df = df.sort_values(by = sortby)
-    for i in df[unique_id].unique():
-        # 默认按时间第一行
-        df_ = df[df[unique_id]==i].iloc[0]
-        df_ = df_.to_frame().T
-        df_result = pd.concat([df_result, df_], ignore_index = True)
-    
-    return df_result
-
-# 按unique_col将所有combine_col的值合并为所有values的list
-def combine_row(df, unique_col='date', combine_col='order_status'):
-    df_result = pd.DataFrame(columns = list(df.columns))
-    for date in list(df[unique_col].unique()):
-        list_status = list(df[df[unique_col] == date][combine_col].values)
-        df_ = pd.DataFrame({unique_col:date, combine_col:[list_status]})
-        df_result = pd.concat([df_result, df_])
-    return df_result
-
-# x, y 自变量与因变量的列名（单自变量）
-# 返回DataFrame  0，1分别为回归系数与截距
-def rolling_reg(df, x_name, y_name, n):
-    # 如果这一字段的df长度小于n，直接返回nan,对应index
-    if df.shape[0]<n:
-        result_nan = np.ones(df.shape[0])*np.nan
-        result = pd.Series(result_nan, df.index)
-        return result
-    # 回归的x和y
-    x = df[x_name]
-    y = df[y_name]
-#    def func(x, y):
-#        # 可能出现连续0值造成错误，这时使用np.nan填充
-#        try:
-#            result = np.polyfit(x, y, deg=1)
-#        except:
-#            # 一元回归情况
-#            result = np.ones(2)*np.nan
-#        return result
-    def func(x, y):
-        lxx = ((x-x.mean())**2).sum()
-        #lyy = ((y-y.mean())**2).sum()
-        lxy = ((x-x.mean())*(y-y.mean())).sum()
-    # 斜率与截距
-        beta = lxy/lxx
-        alpha = y.mean() - beta*x.mean()
-    # Sum of Reg/Error/Total  r2
-        #SSE2 = ((y-(alpha+x*beta))**2).sum()
-        #SSR2 = ((alpha+x*beta - y.mean())**2).sum()
-        #SST2 = SSR2 + SSE2
-        #r2 = SSR2/SST2 
-        r = x.corr(y)
-    # corr**2  = r2 一元线性回归
-        #corr = x.corr(y)
-        return beta, alpha, r 
-    result = rolling_apply(func, n, x, y)
-# 添加index
-    result = pd.DataFrame(result, index=df.index)
-    return result
-
-def rolling_corr(df, x_name, y_name, n):
-    # 如果这一字段的df长度小于n，直接返回nan,对应index
-    if df.shape[0]<n:
-        result_nan = np.ones(df.shape[0])*np.nan
-        result = pd.Series(result_nan, df.index)
-        return result
-    # 相关性的x和y
-    x = df[x_name]
-    y = df[y_name]
-    def func(x, y):
-        r = x.corr(y)
-        return r 
-    result = rolling_apply(func, n, x, y)
-# 添加index
-    result = pd.DataFrame(result, index=df.index)
-    return result
-
-# 并行计算df, func为对df/ser的操作,返回df/ser 可以保留顺序
-def parallel(df, func, n_core=12):
-    len_df = len(df)
-    sp = list(range(len_df)[::int(len_df/n_core+0.5)])[:-1] # 最后一个节点改为末尾
-    sp.append(len_df)
-    slc_gen = (slice(*idx) for idx in zip(sp[:-1],sp[1:]))
-    results = Parallel(n_jobs=n_core)(delayed(func)(df[slc]) for slc in slc_gen)
-    return pd.concat(results)
-
-# 并行group
-def parallel_group(df, func, n_core=12, sort_by='code'):
-    results = Parallel(n_jobs=n_core)(delayed(func)(group) for name, group in df.groupby(sort_by))
-    return pd.concat(results)
-
-# 行情数据的常用计算
-# 数据格式为 mutiindex (date,code)   close...
-
-# 输入series返回series
-# 有并行选项的函数默认并行
-# a 函数可选参数
-def cal_ts(ser, func_name='Max', period=20, a=1, parallel=True, n_core=12):
-    if func_name=='MA':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).mean()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='Max':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).max()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='Min':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).min()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='Std':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).std()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='Skew':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).skew()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='Kurt':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).kurt()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='Sum':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).sum()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name=='rank':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).rank()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
-    elif func_name=='quantile':
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).quantile(a)).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
-    elif func_name=='Zscore':
-        MA = ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).mean()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-        Std = ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).std()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-        return ((ser-MA)/Std).fillna(0)
-    elif func_name=='HV':
-        returns = np.log(ser/ser.groupby(level='code').shift()).fillna(0)
-        return np.exp(returns.groupby(level='code').apply(lambda x: x.droplevel('code').rolling(\
-            period, min_periods=1).std()*np.sqrt(250)).reset_index().sort_values(\
-                by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0])-1
-    elif func_name in ['WMA']:
-        if parallel:
-            def func(ser):
-                return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-                    period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2)))
-            result = parallel_group(ser, func, n_core=n_core)
-            return result.reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2))).reset_index().sort_values(by='date').set_index(\
-                ['date', 'code']).loc[ser.index].iloc[:,0]
-    elif func_name in ['argmin', 'argmax', 'prod']:
-        if parallel:
-            def func(ser):
-                return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-                    period, min_periods=1).apply(getattr(np, func_name)))
-            result = parallel_group(ser, func, n_core=n_core)
-            return result.reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
-        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
-            period, min_periods=1).apply(getattr(np, func_name))).reset_index().sort_values(by='date').set_index(\
-                ['date', 'code']).loc[ser.index].iloc[:,0]
-
-# 按照look列的阈值筛选得到cal列，求和
-def cal_select_sum(df, key, threshold_left, threshold_right, sum, n, n_core=12):
-    # 按条件筛选滚动求和
-    def rolling_select_sum(df, key, threshold_left, threshold_right, sum, n):
-        # 如果这一字段的df长度小于n，直接返回nan,对应index
-        if df.shape[0]<n:
-            result_nan = np.ones(df.shape[0])*np.nan
-            result = pd.Series(result_nan, df.index)
-            return result
-        # 相关性的x和y
-        x = df[key]
-        tl = df[threshold_left]
-        tr = df[threshold_right]
-        y = df[sum]
-        def func(x, tl, tr, y):
-            return ((x>=tl.iloc[-1])*(x<=tr.iloc[-1])*y).sum()
-        result = rolling_apply(func, n, x, tl, tr, y)
-# 添加  index
-        result = pd.DataFrame(result, index=df.index)
-        return result
-    # 按代码并行
-    df = copy.deepcopy(df)
-    # inde必须为 'code'和'date'，并且code内部的date排序
-    df = df.reset_index()
-    df = df.sort_values(by='code')
-    df = df.set_index(['code','date'])
-    df = df.sort_index(level=['code','date'])
-    # 命名规则
-    name_r = str(sum) + '_' + 'Sum' + str(n) + '-' + str(key) + ',' + str(threshold_left) + ';' + str(threshold_right)
-    def func(df):
-        return rolling_select_sum(df.reset_index('code'), key, threshold_left, threshold_right, sum, n)
-    df[[name_r]] =  parallel_group(df, func, n_core=n_core).values
-    # 将index变回 date code
-    df = df.reset_index()
-    df = df.sort_values(by='date')
-    df = df.set_index(['date','code'])
-    df = df.sort_index(level=['date','code'])
-    return df[name_r]
-
-
-# 获得df中x_name列为自变量 y_name列为因变量的线性回归结果 
-def cal_reg(df, x_name, y_name, n, parallel=True, n_core=12):
-    df = copy.deepcopy(df)
-    # inde必须为 'code'和'date'，并且code内部的date排序
-    df = df.reset_index()
-    df = df.sort_values(by='code')
-    df = df.set_index(['code','date'])
-    df = df.sort_index(level=['code','date'])
-    # 命名规则
-    name_beta = str(x_name) + '-' + str(y_name) + '--beta' +str(n)
-    name_alpha = str(x_name) + '-' + str(y_name) + '--alpha'+str(n)
-    name_r = str(x_name) + '-' + str(y_name) + '--r'+str(n)
-    if parallel:
-        def func(df):
-            return rolling_reg(df.reset_index('code'), x_name, y_name, n)
-        df[[name_beta, name_alpha, name_r]] =  parallel_group(df, func, n_core=n_core).values
-    else:
-        # 回归    去掉二级index中的code
-        df_reg = df.groupby('code', sort=False).apply(lambda df: rolling_reg(df.reset_index('code'), x_name, y_name, n))
-        df[[name_beta,name_alpha, name_r]] = df_reg
-    # 将index变回 date code
-    df = df.reset_index()
-    df = df.sort_values(by='date')
-    df = df.set_index(['date','code'])
-    df = df.sort_index(level=['date','code']) 
-    return df
-
-def cal_corr(df, x_name, y_name, n, parallel=True, n_core=12):
-    df = copy.deepcopy(df)
-    # inde必须为 'code'和'date'，并且code内部的date排序
-    df = df.reset_index()
-    df = df.sort_values(by='code')
-    df = df.set_index(['code','date'])
-    df = df.sort_index(level=['code','date'])
-    # 命名规则
-    name_r = str(x_name) + '-' + str(y_name) + '--r'+str(n)
-    if parallel:
-        def func(df):
-            return rolling_corr(df.reset_index('code'), x_name, y_name, n)
-        df[[name_r]] =  parallel_group(df, func, n_core=n_core).values
-    else:
-        # 回归    去掉二级index中的code
-        df_reg = df.groupby('code', sort=False).apply(lambda df: \
-                        rolling_corr(df.reset_index('code'), x_name, y_name, n))
-        df[[name_r]] = df_reg
-    # 将index变回 date code
-    df = df.reset_index()
-    df = df.sort_values(by='date')
-    df = df.set_index(['date','code'])
-    df = df.sort_index(level=['date','code']) 
-    return df
-
-
-# x_name list, y_nmae column
-# 截面多元线性回归
-def cal_CrossReg(df, x_name, y_name, residual=False):
-    import statsmodels.api as sm
-    # 使用sm模块
-    result = df.groupby('date', sort=False).apply(lambda d:\
-                 sm.OLS(d[y_name], sm.add_constant(d[x_name])).fit())
-    
-    # 如果d[x_name]中所有数相同为C且不为零，这时params中没有const，x_name为d[y_name].mean()/C
-    # rsquared为0
-    # 当d[x_name]全为0时，params['const']为0，params[x_name]为d[y_name].mean()
-    # rsquared可能为极小的负数
-    def func(x, name):
-        try:
-            return x.params[name]
-        except:
-            print('sm reg warning')
-            return 0
-    #if type(x_name)!=type([]):
-    r = result.map(lambda x: np.sqrt(abs(x.rsquared)))
-
-    data = []
-    index = []
-    for i in result.items():
-        data.append(dict(i[1].params))
-        index.append(i[0])
-    params = pd.DataFrame(data, index=index)
-
-    if residual:
-        return pd.Series(df.groupby('date').apply(lambda x: x[y_name] - \
-                    (params.loc[x.index[0][0]][x_name]*x[x_name]).sum(axis=1) -\
-                        params.loc[x.index[0][0]]['const']).values, index=df.index)
-    else:
-        return params, r
+import pandas as pd
+import numpy as np
+from numpy_ext import rolling_apply
+from joblib import Parallel, delayed
+import copy, math
+
+# 关于pandas经常使用到的一些操作 以及对现有函数的改进
+
+# dataframe, 查找的列， 为value时删除，包括np.nan 
+# return 操作后df 与被删除的df
+def drop_row(df, col, value_list):
+    drop_all = pd.DataFrame(columns = df.columns)
+    for value in value_list:
+        # nan特殊处理
+        if type(value) == type(np.nan):
+            if np.isnan(value):
+                # 重新排序
+                df = df.reset_index(drop = True)
+                beishanchu = df[df[col].isnull() == True]
+                df = df.drop(df.index[df[col].isnull() == True].values)
+                df = df.reset_index(drop = True)
+        else:
+            df = df.reset_index(drop = True)
+            beishanchu = df[df[col] == value]
+            df = df.drop(df.index[df[col] == value].values)
+            df = df.reset_index(drop = True)
+        drop_all = pd.concat([drop_all, beishanchu], ignore_index=True)
+    return df, drop_all
+
+# merge的改进， 避免列被重新命名(新加的为a_，并且保持on的列不变
+def nmerge(df, df_add, on):
+    new_name = ['a_' + x for x in df_add.columns]
+    new_name = dict(zip(df_add.columns,new_name))
+    df_add = df_add.rename(columns = new_name)
+    # 将 on 列 改回
+    new_name = ['a_' + x for x in on]
+    new_name = dict(zip(new_name,on))
+    # on
+    df_add = df_add.rename(columns = new_name)
+
+    # merge
+    return df.merge(df_add, on=on)
+
+# 将df中所有行按照年份划分，返回一个列表包含各年度的行，从最早开始
+def divide_row(df):
+    first_year = df['date'].min().year
+    last_year = df['date'].max().year
+    result = []
+    for y in range(first_year, last_year+1):
+        select = list(map(lambda x: x.year==y, df['date']))
+        df_ = df[select]
+        result.append(df_)
+    return result
+
+# 按sortby排序，使用unique_id列第一次出现的行组成新的df
+def extract_first(df, unique_id = 'thscode', sortby = 'date'):
+    df_result = pd.DataFrame(columns = df.columns)
+    df = df.sort_values(by = sortby)
+    for i in df[unique_id].unique():
+        # 默认按时间第一行
+        df_ = df[df[unique_id]==i].iloc[0]
+        df_ = df_.to_frame().T
+        df_result = pd.concat([df_result, df_], ignore_index = True)
+    
+    return df_result
+
+# 按unique_col将所有combine_col的值合并为所有values的list
+def combine_row(df, unique_col='date', combine_col='order_status'):
+    df_result = pd.DataFrame(columns = list(df.columns))
+    for date in list(df[unique_col].unique()):
+        list_status = list(df[df[unique_col] == date][combine_col].values)
+        df_ = pd.DataFrame({unique_col:date, combine_col:[list_status]})
+        df_result = pd.concat([df_result, df_])
+    return df_result
+
+# x, y 自变量与因变量的列名（单自变量）
+# 返回DataFrame  0，1分别为回归系数与截距
+def rolling_reg(df, x_name, y_name, n):
+    # 如果这一字段的df长度小于n，直接返回nan,对应index
+    if df.shape[0]<n:
+        result_nan = np.ones(df.shape[0])*np.nan
+        result = pd.Series(result_nan, df.index)
+        return result
+    # 回归的x和y
+    x = df[x_name]
+    y = df[y_name]
+#    def func(x, y):
+#        # 可能出现连续0值造成错误，这时使用np.nan填充
+#        try:
+#            result = np.polyfit(x, y, deg=1)
+#        except:
+#            # 一元回归情况
+#            result = np.ones(2)*np.nan
+#        return result
+    def func(x, y):
+        lxx = ((x-x.mean())**2).sum()
+        #lyy = ((y-y.mean())**2).sum()
+        lxy = ((x-x.mean())*(y-y.mean())).sum()
+    # 斜率与截距
+        beta = lxy/lxx
+        alpha = y.mean() - beta*x.mean()
+    # Sum of Reg/Error/Total  r2
+        #SSE2 = ((y-(alpha+x*beta))**2).sum()
+        #SSR2 = ((alpha+x*beta - y.mean())**2).sum()
+        #SST2 = SSR2 + SSE2
+        #r2 = SSR2/SST2 
+        r = x.corr(y)
+    # corr**2  = r2 一元线性回归
+        #corr = x.corr(y)
+        return beta, alpha, r 
+    result = rolling_apply(func, n, x, y)
+# 添加index
+    result = pd.DataFrame(result, index=df.index)
+    return result
+
+def rolling_corr(df, x_name, y_name, n):
+    # 如果这一字段的df长度小于n，直接返回nan,对应index
+    if df.shape[0]<n:
+        result_nan = np.ones(df.shape[0])*np.nan
+        result = pd.Series(result_nan, df.index)
+        return result
+    # 相关性的x和y
+    x = df[x_name]
+    y = df[y_name]
+    def func(x, y):
+        r = x.corr(y)
+        return r 
+    result = rolling_apply(func, n, x, y)
+# 添加index
+    result = pd.DataFrame(result, index=df.index)
+    return result
+
+# 并行计算df, func为对df/ser的操作,返回df/ser 可以保留顺序
+def parallel(df, func, n_core=12):
+    len_df = len(df)
+    sp = list(range(len_df)[::int(len_df/n_core+0.5)])[:-1] # 最后一个节点改为末尾
+    sp.append(len_df)
+    slc_gen = (slice(*idx) for idx in zip(sp[:-1],sp[1:]))
+    results = Parallel(n_jobs=n_core)(delayed(func)(df[slc]) for slc in slc_gen)
+    return pd.concat(results)
+
+# 并行group
+def parallel_group(df, func, n_core=12, sort_by='code'):
+    results = Parallel(n_jobs=n_core)(delayed(func)(group) for name, group in df.groupby(sort_by))
+    return pd.concat(results)
+
+# 行情数据的常用计算
+# 数据格式为 mutiindex (date,code)   close...
+
+# 输入series返回series
+# 有并行选项的函数默认并行
+# a 函数可选参数
+def cal_ts(ser, func_name='Max', period=20, a=1, parallel=True, n_core=12):
+    if func_name=='MA':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).mean()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='Max':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).max()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='Min':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).min()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='Std':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).std()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='Skew':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).skew()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='Kurt':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).kurt()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='Sum':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).sum()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name=='rank':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).rank()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
+    elif func_name=='quantile':
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).quantile(a)).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0] 
+    elif func_name=='Zscore':
+        MA = ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).mean()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+        Std = ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).std()).reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+        return ((ser-MA)/Std).fillna(0)
+    elif func_name=='HV':
+        returns = np.log(ser/ser.groupby(level='code').shift()).fillna(0)
+        return np.exp(returns.groupby(level='code').apply(lambda x: x.droplevel('code').rolling(\
+            period, min_periods=1).std()*np.sqrt(250)).reset_index().sort_values(\
+                by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0])-1
+    elif func_name in ['WMA']:
+        if parallel:
+            def func(ser):
+                return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+                    period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2)))
+            result = parallel_group(ser, func, n_core=n_core)
+            return result.reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).apply(lambda x: x[::-1].cumsum().sum()/(period*(1+period)/2))).reset_index().sort_values(by='date').set_index(\
+                ['date', 'code']).loc[ser.index].iloc[:,0]
+    elif func_name in ['argmin', 'argmax', 'prod']:
+        if parallel:
+            def func(ser):
+                return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+                    period, min_periods=1).apply(getattr(np, func_name)))
+            result = parallel_group(ser, func, n_core=n_core)
+            return result.reset_index().sort_values(by='date').set_index(['date', 'code']).loc[ser.index].iloc[:,0]
+        return ser.groupby(level='code').apply(lambda x: x.droplevel( 'code').rolling(\
+            period, min_periods=1).apply(getattr(np, func_name))).reset_index().sort_values(by='date').set_index(\
+                ['date', 'code']).loc[ser.index].iloc[:,0]
+
+# 按照look列的阈值筛选得到cal列，求和
+def cal_select_sum(df, key, threshold_left, threshold_right, sum, n, n_core=12):
+    # 按条件筛选滚动求和
+    def rolling_select_sum(df, key, threshold_left, threshold_right, sum, n):
+        # 如果这一字段的df长度小于n，直接返回nan,对应index
+        if df.shape[0]<n:
+            result_nan = np.ones(df.shape[0])*np.nan
+            result = pd.Series(result_nan, df.index)
+            return result
+        # 相关性的x和y
+        x = df[key]
+        tl = df[threshold_left]
+        tr = df[threshold_right]
+        y = df[sum]
+        def func(x, tl, tr, y):
+            return ((x>=tl.iloc[-1])*(x<=tr.iloc[-1])*y).sum()
+        result = rolling_apply(func, n, x, tl, tr, y)
+# 添加  index
+        result = pd.DataFrame(result, index=df.index)
+        return result
+    # 按代码并行
+    df = copy.deepcopy(df)
+    # inde必须为 'code'和'date'，并且code内部的date排序
+    df = df.reset_index()
+    df = df.sort_values(by='code')
+    df = df.set_index(['code','date'])
+    df = df.sort_index(level=['code','date'])
+    # 命名规则
+    name_r = str(sum) + '_' + 'Sum' + str(n) + '-' + str(key) + ',' + str(threshold_left) + ';' + str(threshold_right)
+    def func(df):
+        return rolling_select_sum(df.reset_index('code'), key, threshold_left, threshold_right, sum, n)
+    df[[name_r]] =  parallel_group(df, func, n_core=n_core).values
+    # 将index变回 date code
+    df = df.reset_index()
+    df = df.sort_values(by='date')
+    df = df.set_index(['date','code'])
+    df = df.sort_index(level=['date','code'])
+    return df[name_r]
+
+
+# 获得df中x_name列为自变量 y_name列为因变量的线性回归结果 
+def cal_reg(df, x_name, y_name, n, parallel=True, n_core=12):
+    df = copy.deepcopy(df)
+    # inde必须为 'code'和'date'，并且code内部的date排序
+    df = df.reset_index()
+    df = df.sort_values(by='code')
+    df = df.set_index(['code','date'])
+    df = df.sort_index(level=['code','date'])
+    # 命名规则
+    name_beta = str(x_name) + '-' + str(y_name) + '--beta' +str(n)
+    name_alpha = str(x_name) + '-' + str(y_name) + '--alpha'+str(n)
+    name_r = str(x_name) + '-' + str(y_name) + '--r'+str(n)
+    if parallel:
+        def func(df):
+            return rolling_reg(df.reset_index('code'), x_name, y_name, n)
+        df[[name_beta, name_alpha, name_r]] =  parallel_group(df, func, n_core=n_core).values
+    else:
+        # 回归    去掉二级index中的code
+        df_reg = df.groupby('code', sort=False).apply(lambda df: rolling_reg(df.reset_index('code'), x_name, y_name, n))
+        df[[name_beta,name_alpha, name_r]] = df_reg
+    # 将index变回 date code
+    df = df.reset_index()
+    df = df.sort_values(by='date')
+    df = df.set_index(['date','code'])
+    df = df.sort_index(level=['date','code']) 
+    return df
+
+def cal_corr(df, x_name, y_name, n, parallel=True, n_core=12):
+    df = copy.deepcopy(df)
+    # inde必须为 'code'和'date'，并且code内部的date排序
+    df = df.reset_index()
+    df = df.sort_values(by='code')
+    df = df.set_index(['code','date'])
+    df = df.sort_index(level=['code','date'])
+    # 命名规则
+    name_r = str(x_name) + '-' + str(y_name) + '--r'+str(n)
+    if parallel:
+        def func(df):
+            return rolling_corr(df.reset_index('code'), x_name, y_name, n)
+        df[[name_r]] =  parallel_group(df, func, n_core=n_core).values
+    else:
+        # 回归    去掉二级index中的code
+        df_reg = df.groupby('code', sort=False).apply(lambda df: \
+                        rolling_corr(df.reset_index('code'), x_name, y_name, n))
+        df[[name_r]] = df_reg
+    # 将index变回 date code
+    df = df.reset_index()
+    df = df.sort_values(by='date')
+    df = df.set_index(['date','code'])
+    df = df.sort_index(level=['date','code']) 
+    return df
+
+
+# x_name list, y_nmae column
+# 截面多元线性回归
+def cal_CrossReg(df, x_name, y_name, residual=False):
+    import statsmodels.api as sm
+    # 使用sm模块
+    result = df.groupby('date', sort=False).apply(lambda d:\
+                 sm.OLS(d[y_name], sm.add_constant(d[x_name])).fit())
+    
+    # 如果d[x_name]中所有数相同为C且不为零，这时params中没有const，x_name为d[y_name].mean()/C
+    # rsquared为0
+    # 当d[x_name]全为0时，params['const']为0，params[x_name]为d[y_name].mean()
+    # rsquared可能为极小的负数
+    def func(x, name):
+        try:
+            return x.params[name]
+        except:
+            print('sm reg warning')
+            return 0
+    #if type(x_name)!=type([]):
+    r = result.map(lambda x: np.sqrt(abs(x.rsquared)))
+
+    data = []
+    index = []
+    for i in result.items():
+        data.append(dict(i[1].params))
+        index.append(i[0])
+    params = pd.DataFrame(data, index=index)
+
+    if residual:
+        return pd.Series(df.groupby('date').apply(lambda x: x[y_name] - \
+                    (params.loc[x.index[0][0]][x_name]*x[x_name]).sum(axis=1) -\
+                        params.loc[x.index[0][0]]['const']).values, index=df.index)
+    else:
+        return params, r
```

### Comparing `FreeBack-3.0.1a0/FreeBack/post.py` & `FreeBack-4.1.0a0/FreeBack/post.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,769 +1,632 @@
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-import datetime
-import statsmodels.api as sm
-from plottable import ColumnDefinition, ColDef, Table
-from matplotlib.colors import LinearSegmentedColormap
-from FreeBack.display import *
-import os
-  
-
-'''
-# matplot绘图
-def matplot(r=1, c=1, sharex=False, sharey=False, w=8, d=5):
-    # don't use sns style
-    sns.reset_orig()
-    #plot
-    #run configuration 
-    plt.rcParams['font.size']=14
-    plt.rcParams['font.family'] = 'KaiTi'
-    #plt.rcParams['font.family'] = 'Arial'
-    plt.rcParams['font.sans-serif']=['Microsoft YaHei']
-    plt.rcParams["axes.unicode_minus"]=False #该语句解决图像中的“-”负号的乱码问题
-    plt.rcParams['axes.linewidth']=1
-    plt.rcParams['axes.grid']=True
-    plt.rcParams['grid.linestyle']='--'
-    plt.rcParams['grid.linewidth']=0.2
-    plt.rcParams["savefig.transparent"]='True'
-    plt.rcParams['lines.linewidth']=0.8
-    plt.rcParams['lines.markersize'] = 1
-    
-    #保证图片完全展示
-    plt.tight_layout()
-        
-    #subplot
-    fig,ax = plt.subplots(r,c,sharex=sharex, sharey=sharey,figsize=(w,d))
-    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, hspace = None, wspace=0.5)
-        
-    plt.gcf().autofmt_xdate()
-
-    return plt, fig, ax
-
-# 月度数据热力图  
-# period_value格式为 index month ‘2023-7-1’  value  0: ***
-# color_threshold 为红绿色分界点
-def month_thermal(period_value, color_threshold=0):   
-    # 数值>0红色，<0为绿色。转化为颜色[R,G,B]
-    def color_map(x, max_r):
-        if x>0:
-            return [1,1-x/max_r,1-x/max_r]
-        elif x == 0:
-            return [1,1,1]
-        else:
-            return [1+x/max_r,1,1+x/max_r]
-    # i 年份序号（纵坐标）  j 月份序号（横坐标） calendar是值， plot是颜色
-    def calendar_array(dates, data):
-    #    i, j = zip(*[d.isocalendar()[1:] for d in dates])
-    # 年份  月份 array
-        i, j = zip(*[(d.year,d.month) for d in dates])
-        i = np.array(i) - min(i)
-        j = np.array(j) - 1
-    # 总年份
-        ni = max(i) + 1
-    # 12个月
-    # 值 矩阵
-        calendar = np.nan * np.zeros((ni, 12))
-    # 颜色值 矩阵 默认白色[1,1,1]
-        plot =   np.ones((ni, 12, 3))
-        calendar[i, j] = data
-    # 绝对值最大为纯红（绿）
-        max_r = np.abs(data).max().max()
-        mat_color = [color_map(i-color_threshold,max_r) for i in data]
-        plot[i,j] = np.array(mat_color)
-        return i, j, plot, calendar
-
-    # 纵坐标为年份，横坐标为月份, 填充值
-    dates, data = list(period_value.index), period_value.iloc[:,0].values
-    i, j, plot, calendar = calendar_array(dates, data)
-    # 绘制热力图
-    plt, fig, ax = matplot()
-    ax.imshow(plot, aspect='auto')
-    # 设置纵坐标 年份
-    i = np.array(list(set(i)))
-    i.sort()
-    ax.set(yticks=i)
-    # 年份
-    years = list(set([i.year for i in period_value.index]))
-    ax.set_yticklabels(years)
-    # 设置横坐标 月份
-    j = np.array(list(set(j)))
-    j.sort()
-    ax.set(xticks=j)
-    ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
-                                'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
-    # 关闭网格
-    ax.grid(False)
-    # 显示数值
-    for i_ in i:
-        for j_ in j:
-            if not np.isnan(calendar[i_][j_]):
-                ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
-    return plt, fig, ax
-
-# 月度收益热力图    输入对数收益率的series 
-def plot_thermal(df_returns):
-    # 先转化为对数收益率
-    #df_lr = df_returns.apply(lambda x: np.log(x+1))
-    df_lr = df_returns.reset_index()
-    # 筛出同月数据
-    df_lr['month'] = df_lr['date'].apply(lambda x: x - datetime.timedelta(x.day-1))
-    df_lr = df_lr[['month', df_returns.name]]
-    df_lr = df_lr.set_index('month')
-    # 月度收益 %
-    period_return = (np.exp(df_lr.groupby('month').sum()) - 1)*100
-    # 收益率转化为颜色[R,G,B]
-    def color_map(x,max_r):
-        if x>0:
-            return [1,1-x/max_r,1-x/max_r]
-        elif x == 0:
-            return [1,1,1]
-        else:
-            return [1+x/max_r,1,1+x/max_r]
-    # i 年份序号（纵坐标）  j 月份序号（横坐标） calendar是值， plot是颜色
-    def calendar_array(dates, data):
-    #    i, j = zip(*[d.isocalendar()[1:] for d in dates])
-    # 年份  月份 array
-        i, j = zip(*[(d.year,d.month) for d in dates])
-        i = np.array(i) - min(i)
-        j = np.array(j) - 1
-    # 总年份
-        ni = max(i) + 1
-    # 12个月
-    # 收益率 矩阵
-        calendar = np.nan * np.zeros((ni, 12))
-    # 颜色值 矩阵 默认白色[1,1,1]
-        plot =   np.ones((ni, 12, 3))
-        calendar[i, j] = data
-    # 正最大收益为纯红 负最大收益为纯绿
-        max_r = np.abs(data).max().max()
-        mat_color = [color_map(i,max_r) for i in data]
-        plot[i,j] = np.array(mat_color)
-        return i, j, plot, calendar
-
-    # 纵坐标为年份，横坐标为月份, 填充值
-    dates, data = list(period_return.index), period_return.iloc[:,0].values
-    i, j, plot, calendar = calendar_array(dates, data)
-    # 绘制热力图
-    plt, fig, ax = matplot()
-    ax.imshow(plot, aspect='auto')
-    # 设置纵坐标 年份
-    i = np.array(list(set(i)))
-    i.sort()
-    ax.set(yticks=i)
-    # 年份
-    years = list(set([i.year for i in df_returns.index]))
-    ax.set_yticklabels(years)
-    # 设置横坐标 月份
-    j = np.array(list(set(j)))
-    j.sort()
-    ax.set(xticks=j)
-    ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
-                                'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
-    # 关闭网格
-    ax.grid(False)
-    # 显示数值
-    for i_ in i:
-        for j_ in j:
-            if not np.isnan(calendar[i_][j_]):
-                ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
-
-    return plt, fig, ax
-'''
-
-# 仅处理收益率序列（简单收益率，非对数收益率）结果
-class SeriesPost():
-    def __init__(self, returns, benchmark=None, stratname='策略'):
-        self.stratname = stratname
-        self.returns = returns
-        self.net = (1+returns).cumprod()
-        # 无风险利率
-        self.rf = 0.03
-        # 基准
-        if type(benchmark) == type(None):
-            benchmark = pd.DataFrame(index = returns.index)
-            benchmark['zero'] = 0
-            self.benchmark = benchmark
-        self.benchmark = benchmark.loc[returns.index].fillna(0)
-        # 基准波动率
-        self.sigma_benchmark = np.exp(np.log(self.benchmark[\
-            self.benchmark.columns[0]]+1).std())-1
-        # 计算复杂指标
-        # 净值曲线
-        self.lr = np.log(self.returns + 1)
-        # 超额收益 默认第一个benchmark
-        self.excess_lr = self.lr-np.log(self.benchmark[self.benchmark.columns[0]]+1)
-        self.returns.index.name = 'date'
-        
-        # 评价指标
-        # 年化收益率（+1）
-        self.years = (returns.index[-1]-returns.index[0]).days/365  
-        self.return_total = (returns+1).prod()                             
-        self.return_annual = self.return_total**(1/self.years)-1    
-        excess_total = np.exp(self.excess_lr.sum())                  # 超额收益
-        self.excess_return_annual = excess_total**(1/self.years)-1
-        # 年化波动率 shrpe
-        self.sigma = np.exp(self.lr.std())-1
-        self.sharpe = (self.return_annual - self.rf)/(self.sigma*np.sqrt(250))
-        # 超额年化波动率 shrpe
-        self.excess_sigma = np.exp(self.excess_lr.std())-1
-        self.excess_sharpe = (self.excess_return_annual - self.rf)/(self.excess_sigma*np.sqrt(250))
-        # 回撤
-        a = np.maximum.accumulate(self.net)
-        self.drawdown = (a-self.net)/a
-    def cal_complex(self):
-        # 复杂指标 
-        win = self.lr[self.lr>0]
-        loss = self.lr[self.lr<0]
-        excesswin = self.excess_lr[self.excess_lr>0]
-        excessloss = self.excess_lr[self.excess_lr<0]
-        # 下行波动率
-        self.sigma_down = np.exp((self.lr-\
-                            self.lr.mean()).apply(lambda x: min(x,0)).std())-1
-        # 跟踪误差
-        self.sigma_alpha = np.exp(np.std(self.lr-\
-                             np.log(self.benchmark[self.benchmark.columns[0]]+1)))-1
-        # 超额回撤
-        excess_net = np.exp(self.excess_lr.fillna(0).cumsum())
-        a = np.maximum.accumulate(excess_net)
-        self.excess_drawdown = (a-excess_net)/a
-        # CAPM (无风险收益为0)
-        y = self.returns.fillna(0)
-        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
-        x = sm.add_constant(x)
-        model = sm.OLS(y, x).fit()
-        # T-M 模型(无风险收益为0)
-        y = self.returns.fillna(0)
-        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
-        x = sm.add_constant(x)
-        model = sm.OLS(y, x).fit()
-        # 市场风险暴露
-        self.beta = model.params[self.benchmark.columns[0]]
-        # 市场波动无法解释的截距项
-        self.alpha = model.params['const'] 
-        #model.summary()
-        ## 索提诺比率   单位下行风险的超额收益
-        #self.sortino = (self.return_annual - self.rf)/(self.sigma_down*np.sqrt(250))
-        # 特雷诺指数  单位beta的超额收益
-        self.treynor  = (self.return_annual - self.rf)/self.beta 
-# 净值曲线
-# 时间起止（默认全部），是否显示细节,是否自定义输出图片名称，是否显示对数，是否显示超额
-    def pnl(self, timerange=None, detail=True, filename=None, log=False, excess=False):
-        plt, fig, ax = matplot(w=10)
-        # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
-        if type(timerange) != type(None):
-            # 时间段内净值与基准
-            net = self.net.loc[timerange[0]:timerange[1]]
-            returns = self.returns.loc[timerange[0]:timerange[1]]
-            # 计算夏普
-            years = (pd.to_datetime(timerange[1])-pd.to_datetime(timerange[0])).days/365
-            return_annual = (net[-1]/net[0])**(1/years)-1
-            std_annual = returns.std()*np.sqrt(250)
-            sharpe = (return_annual - self.rf)/std_annual
-            if detail:
-                # 回撤
-                a = np.maximum.accumulate(net)
-                drawdown = (a-net)/a 
-                ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
-                    round(100*return_annual,2), round(sharpe,2), 
-                        round(100*max(drawdown),2)), transform=ax.transAxes)
-                # 回撤
-                ax2 = ax.twinx()
-                ax2.fill_between(drawdown.index,-100*drawdown, 0, color='C1', alpha=0.1)
-                if excess:
-                    ax.plot(np.exp(self.excess_lr.loc[timerange[0]:timerange[1]].cumsum()), 
-                            c='C3', label='超额收益')
-            else:
-                ax.text(0.7,0.05,'Sharpe:  {}'.format(round(sharpe,2)), transform=ax.transAxes)
-            ax.plot(net/net[0], c='C0', label='p&l')
-            if type(self.benchmark) != type(None):
-                benchmark = self.benchmark.loc[timerange[0]:timerange[1]].copy()
-                benchmark.iloc[0] = 0
-        # colors of benchmark
-                colors_list = ['C4','C5','C6','C7']
-                for i in range(len(benchmark.columns)):
-                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), 
-                            c=colors_list[i], label=benchmark.columns[i])
-            if log:
-                # 对数坐标显示
-                ax.set_yscale("log")
-            ax.set_xlim(returns.index[0], returns.index[-1])
-            plt.gcf().autofmt_xdate()
-        else:
-    #评价指标
-            ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
-            round(100*self.return_annual,2), round(self.sharpe,2), 
-            round(100*max(self.drawdown),2)), transform=ax.transAxes)
-        # 净值与基准
-            ax.plot(self.net, c='C0', label=self.stratname)
-            if not (self.benchmark==0).any().values[0]:
-                # benchmark 匹配回测时间段, 基准从0开始
-                # 如果基准是0就不绘制了
-                benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
-                benchmark.loc[self.net.index[0]] = 0
-                # colors of benchmark
-                colors_list = ['C4','C5','C6','C7']
-                for i in range(len(benchmark.columns)):
-                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), \
-                            c=colors_list[i], label=benchmark.columns[i])
-                if excess:
-                    ax.plot(np.exp(self.excess_lr.cumsum()), c='C3', label='超额收益')
-                plt.legend(loc='upper left')
-            if log:
-                # 对数坐标显示
-                ax.set_yscale("log")
-            # 回撤
-            ax2 = ax.twinx()
-            ax2.fill_between(self.drawdown.index,-100*self.drawdown, 0, color='C1', alpha=0.1)
-            ax.set_ylabel('累计净值')
-            ax.set_xlabel('日期')
-            ax2.set_ylabel('回撤 (%)')
-            ax.set_xlim(self.net.index[0], self.net.index[-1])
-            plt.gcf().autofmt_xdate()
-        if 'output' in os.listdir():
-            pass
-        else:
-            os.mkdir('output')
-        if type(filename) == type(None):
-            plt.savefig('./output/pnl.png')
-        else:
-            plt.savefig('./output/'+filename)
-        plt.show()
-
-
-
-# 传入barbybar运行完毕的world对象
-class Post():
-    # benchmark为收益率（非对数收益率）
-    def __init__(self, world, benchmark=None, stratname='策略'):
-        # world
-        self.world = world
-        # 策略名
-        self.stratname = stratname
-        # 无风险利率
-        self.rf = 0.03
-        # 基准
-        if type(benchmark) == type(None):
-            benchmark = pd.DataFrame(index = world.series_net.index)
-            benchmark['zero'] = 0
-            self.benchmark = benchmark
-        self.benchmark = benchmark.loc[world.series_net.index].fillna(0)
-        self.sigma_benchmark = np.exp(np.log(self.benchmark[\
-            self.benchmark.columns[0]]+1).std())-1
-        self.details()
-
-# 策略详细评价指标
-    def details(self):
-        # 净值曲线
-        self.abs_net = self.world.series_net
-        self.net = self.world.series_net/self.world.series_net.iloc[0]
-        self.returns = self.net/self.net.shift() - 1
-        self.lr = np.log(self.returns + 1)
-        # 超额收益 默认第一个benchmark
-        self.excess_lr = self.lr  - np.log(self.benchmark[self.benchmark.columns[0]]+1)
-        self.returns.index.name = 'date'
-        # 评价指标
-        # 年化收益率
-        self.years = (self.net.index[-1]-self.net.index[0]).days/365
-        self.return_total = self.net[-1]/self.net[0]
-        self.return_annual = self.return_total**(1/self.years)-1
-        excess_total = np.exp(self.excess_lr.sum())
-        self.excess_return_annual = excess_total**(1/self.years)-1
-        # 年化波动率 shrpe
-        self.sigma = np.exp(self.lr.std())-1
-        self.sharpe = (self.return_annual - self.rf)/(self.sigma*np.sqrt(250))
-        # 超额年化波动率 shrpe
-        self.excess_sigma = np.exp(self.excess_lr.std())-1
-        self.excess_sharpe = (self.excess_return_annual - self.rf)/(self.excess_sigma*np.sqrt(250))
-        # 回撤
-        a = np.maximum.accumulate(self.net)
-        self.drawdown = (a-self.net)/a
-        # 持仓标的
-        self.df_hold = self.world.df_hold
-        held = self.world.df_hold.reset_index().melt(id_vars=['date']).set_index(['date', 'code'])
-        held = held['value'] * self.world.market['close']
-        self.held = held[(held != 0)&~np.isnan(held)]
-        # 现金
-        self.cash = self.world.series_cash
-        # 交割单
-        self.excute = self.world.df_excute.reset_index().set_index(['date', 'code', 'unique'])
-        # 换手率
-        occurance_amount = abs(self.excute['occurance_amount']).groupby('date').sum()
-        #turnover = (occurance_amount/(self.net*self.cash.iloc[0])).fillna(0)
-        turnover = (occurance_amount/self.world.series_net).fillna(0)
-        self.turnover = turnover.mean()*250
-
-        # 逐笔交易信息
-        self.trade()
-
-        # details 表格
-        win = self.lr[self.lr>0]
-        loss = self.lr[self.lr<0]
-        excesswin = self.excess_lr[self.excess_lr>0]
-        excessloss = self.excess_lr[self.excess_lr<0]
-        # 下行波动率
-        self.sigma_down = np.exp((self.lr-self.lr.mean()).apply(lambda x: min(x,0)).std())-1
-        # 跟踪误差
-        sigma_alpha = np.exp(np.std(self.lr-np.log(self.benchmark[self.benchmark.columns[0]]+1)))-1
-        # 超额回撤
-        excess_net = np.exp(self.excess_lr.fillna(0).cumsum())
-        a = np.maximum.accumulate(excess_net)
-        self.excess_drawdown = (a-excess_net)/a
-        # CAPM (无风险收益为0)
-        y = self.returns.fillna(0)
-        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
-        x = sm.add_constant(x)
-        model = sm.OLS(y, x).fit()
-        # T-M 模型(无风险收益为0)
-        y = self.returns.fillna(0)
-        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
-        x = sm.add_constant(x)
-        model = sm.OLS(y, x).fit()
-        # 市场风险暴露
-        self.beta = model.params[self.benchmark.columns[0]]
-        # 市场波动无法解释的截距项
-        self.alpha = model.params['const'] 
-        #model.summary()
-        ## 索提诺比率   单位下行风险的超额收益
-        #self.sortino = (self.return_annual - self.rf)/(self.sigma_down*np.sqrt(250))
-        # 特雷诺指数  单位beta的超额收益
-        self.treynor  = (self.return_annual - self.rf)/self.beta
-
-        col0 = pd.DataFrame(columns=['col0'])
-        col0.loc[0] = '运行时间（年, 日）'
-        col0.loc[1] = '%s, %s'%(round(self.years,1), len(self.net))
-        col0.loc[2] = '盈利次数（日）'
-        col0.loc[3] = len(win)
-        col0.loc[4] = '超额次数（日）'
-        col0.loc[5] = len(excesswin)
-        col0.loc[6] = '空仓次数（日）' 
-        col0.loc[7] = len(self.net)-len(win)-len(loss) 
-        col1 = pd.DataFrame(columns=['col1'])
-        col1.loc[0] = '年化收益率（%）'
-        col1.loc[1] = round(self.return_annual*100,1)
-        col1.loc[2] = '年化超额收益率（%）'
-        col1.loc[3] = round(self.excess_return_annual*100,1)
-        col1.loc[4] = '累计收益（%）'
-        col1.loc[5] = round((self.return_total-1)*100,1)
-        col1.loc[6] = '累计超额收益（%）'
-        col1.loc[7] = round((excess_total-1)*100,1)
-        col2 = pd.DataFrame(columns=['col2'])
-        col2.loc[0] = '日胜率（%）'
-        col2.loc[1] = round(100*len(win)/(len(win)+len(loss)),1) 
-        col2.loc[2] = '超额日胜率（%）'
-        col2.loc[3] = round(100*len(excesswin)/(len(excesswin)+\
-                                len(excessloss)),1) 
-        col2.loc[4] = '日盈亏比'
-        col2.loc[5] = round(win.mean()/abs(loss.mean()),2) 
-        col2.loc[6] = '亏损日平均亏损（万）'
-        col2.loc[7] = round(abs(loss.mean())*10000,1) 
-        col3 = pd.DataFrame(columns=['col3'])
-        col3.loc[0] = '最大回撤（%）'
-        col3.loc[1] = round(max(self.drawdown)*100, 1)
-        col3.loc[2] = '超额最大回撤（%）'
-        col3.loc[3] = round(max(self.excess_drawdown)*100, 1)
-        col3.loc[4] = '波动率（%）'
-        col3.loc[5] = round(self.sigma*np.sqrt(250)*100, 1)
-        col3.loc[6] = '基准波动率（%）'
-        col3.loc[7] = round(self.sigma_benchmark*np.sqrt(250)*100, 1)
-        col4 = pd.DataFrame(columns=['col4'])
-        col4.loc[0] = '下行波动率（%）'
-        col4.loc[1] = round(self.sigma_down*np.sqrt(250)*100, 1)
-        col4.loc[2] = 'beta系数'
-        col4.loc[3] = round(self.beta,2) 
-        col4.loc[4] = '跟踪误差（%）'
-        col4.loc[5] = round(sigma_alpha*np.sqrt(250)*100, 1)
-        col4.loc[6] = '年化换手' 
-        col4.loc[7] = round(self.turnover,1)
-        col5 = pd.DataFrame(columns=['col5'])
-        col5.loc[0] = '夏普比率'
-        col5.loc[1] = round(self.sharpe,2)
-        col5.loc[2] = '超额夏普' 
-        col5.loc[3] = round(self.excess_sharpe,2)
-        col5.loc[4] = '卡玛比率'
-        col5.loc[5] = round(self.return_annual/max(self.drawdown),2)
-        col5.loc[6] = '无风险收益率（%）' 
-        col5.loc[7] = self.rf*100 
-        col6 = pd.DataFrame(columns=['col6'])
-        col6.loc[0] = '詹森指数（alpha）'
-        #col6.loc[0] = '詹森指数'
-        col6.loc[1] = round(self.alpha*250*100,1) 
-        col6.loc[2] = '特雷诺指数'  # 单位beta的超额收益 
-        col6.loc[3] =  round(self.treynor, 2)
-        col6.loc[4] = '信息比率'   # 超额收益的夏普
-        col6.loc[5] = round(self.alpha*np.sqrt(250)/sigma_alpha,2) 
-        col6.loc[6] = '' 
-        col6.loc[7] = '' 
-        col7 = pd.DataFrame(columns=['col7'])
-        col7.loc[0] = 'Hurst指数' 
-        col7.loc[1] = '' 
-        col7.loc[2] = 'T-M模型' 
-        col7.loc[3] = '' 
-        col7.loc[4] = '' 
-        col7.loc[5] = '' 
-        col7.loc[6] = '' 
-        col7.loc[7] = '' 
-        df_details = pd.concat([col0, col1, col2, col3, \
-                col4, col5, col6, col7], axis=1)
-
-        plt, fig, ax = matplot(w=22)
-        column_definitions = [ColumnDefinition(name='col0', group="收益能力"), \
-                              ColumnDefinition(name='col1', group="收益能力"), \
-                            ColumnDefinition(name='col2', group='收益能力'), \
-                            ColumnDefinition(name='col3', group='风险水平'), \
-                            ColumnDefinition(name="col4", group='风险水平'), \
-                            ColumnDefinition(name="col5", group='风险调整'), \
-                            ColumnDefinition(name="col6", group='风险调整'),
-                            ColumnDefinition(name="col7", group='业绩持续性分析')] +\
-                            [ColDef("index", title="", width=1.5, textprops={"ha":"right"})]
-        tab = Table(df_details, row_dividers=False, col_label_divider=False, 
-                    column_definitions=column_definitions,
-                    odd_row_color="#e0f6ff", even_row_color="#f0f0f0", 
-                    textprops={"ha": "center"})
-        #ax.set_xlim(2,5)
-        # 设置列标题文字和背景颜色(隐藏表头名)
-        tab.col_label_row.set_facecolor("white")
-        tab.col_label_row.set_fontcolor("white")
-        # 设置行标题文字和背景颜色
-        tab.columns["index"].set_facecolor("white")
-        tab.columns["index"].set_fontcolor("white")
-        tab.columns["index"].set_linewidth(0)
-        plt.savefig('details.png')
-        plt.show()
-# 净值曲线
-    def pnl(self, timerange=None, detail=False, filename=None, log=False, excess=True):
-        plt, fig, ax = matplot(w=10)
-        # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
-        if type(timerange) != type(None):
-            # 时间段内净值与基准
-            net = self.net.loc[timerange[0]:timerange[1]]
-            returns = self.returns.loc[timerange[0]:timerange[1]]
-            # 计算夏普
-            years = (pd.to_datetime(timerange[1])-pd.to_datetime(timerange[0])).days/365
-            return_annual = (net[-1]/net[0])**(1/years)-1
-            std_annual = returns.std()*np.sqrt(250)
-            sharpe = (return_annual - self.rf)/std_annual
-            if detail:
-                # 回撤
-                a = np.maximum.accumulate(net)
-                drawdown = (a-net)/a 
-                ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
-                    round(100*return_annual,2), round(sharpe,2), 
-                        round(100*max(drawdown),2)), transform=ax.transAxes)
-                # 回撤
-                ax2 = ax.twinx()
-                ax2.fill_between(drawdown.index,-100*drawdown, 0, color='C1', alpha=0.1)
-                if excess:
-                    ax.plot(np.exp(self.excess_lr.loc[timerange[0]:timerange[1]].cumsum()), 
-                            c='C3', label='超额收益')
-            else:
-                ax.text(0.7,0.05,'Sharpe:  {}'.format(round(sharpe,2)), transform=ax.transAxes)
-            ax.plot(net/net[0], c='C0', label='p&l')
-            if type(self.benchmark) != type(None):
-                benchmark = self.benchmark.loc[timerange[0]:timerange[1]].copy()
-                benchmark.iloc[0] = 0
-        # colors of benchmark
-                colors_list = ['C4','C5','C6','C7']
-                for i in range(len(benchmark.columns)):
-                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), 
-                            c=colors_list[i], label=benchmark.columns[i])
-            if log:
-                # 对数坐标显示
-                ax.set_yscale("log")
-            ax.set_xlim(returns.index[0], returns.index[-1])
-            plt.gcf().autofmt_xdate()
-        else: 
-    #评价指标
-            ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
-            round(100*self.return_annual,2), round(self.sharpe,2), 
-            round(100*max(self.drawdown),2)), transform=ax.transAxes)
-        # 净值与基准
-            ax.plot(self.net, c='C0', label=self.stratname)
-            if type(self.benchmark) != type(None):
-                # benchmark 匹配回测时间段, 基准从0开始
-                benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
-                benchmark.loc[self.net.index[0]] = 0
-                # colors of benchmark
-                colors_list = ['C4','C5','C6','C7']
-                for i in range(len(benchmark.columns)):
-                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(),  c=colors_list[i], label=benchmark.columns[i])
-                if excess:
-                    ax.plot(np.exp(self.excess_lr.cumsum()), c='C3', label='超额收益')
-                plt.legend(loc='upper left')
-            if log:
-                # 对数坐标显示
-                ax.set_yscale("log")
-            # 回撤
-            ax2 = ax.twinx()
-            ax2.fill_between(self.drawdown.index,-100*self.drawdown, 0, color='C1', alpha=0.1)
-            ax.set_ylabel('累计净值')
-            ax.set_xlabel('日期')
-            ax2.set_ylabel('回撤 (%)')
-            ax.set_xlim(self.net.index[0], self.net.index[-1])
-            plt.gcf().autofmt_xdate()
-        if type(filename) == type(None):
-            plt.savefig('pnl.png')
-        else:
-            plt.savefig(filename)
-        plt.show()
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
-# 交易分析
-    def trade(self):
-        self.CashFlow = self.excute.apply(lambda x: x['occurance_amount'] - x['comm'] if x['BuyOrSell']=='Sell' else -x['occurance_amount'] - x['comm'], axis=1)
-        # 获取持仓卖出变为0时的订单unique，记为一次交易结束(有可能会出现同时两个卖出订单误判为两次交易)
-        completes = list(self.excute[(self.excute['remain_vol'] == 0)&(self.excute['BuyOrSell']=='Sell')].reset_index()['unique'])
-        # 对每个标的的累积现金流
-        CumCashFlow = self.CashFlow.groupby('code').cumsum()
-        # 截取交易结束节点
-        Close_amount = CumCashFlow.reset_index().set_index('unique').loc[completes]
-        Close_amount = Close_amount.reset_index().set_index(['date', 'code', 'unique'])[0]
-        # 每次交易盈亏（当前交易结束的现金流-上一次交易结束的现金流 ）
-        self.Close_amount = Close_amount - Close_amount.groupby('code').shift().fillna(0)
-        trade_pnl = self.Close_amount.reset_index()[['date', 'code', 0]].set_index([\
-                                'date', 'code'])[0]
-        self.trade_pnl = trade_pnl.sort_values()/self.abs_net
-        # 筛出同月数据
-        trades = self.Close_amount.reset_index()
-        trades['month'] = trades['date'].apply(lambda x: x - datetime.timedelta(x.day-1)) 
-        trades = trades[['month', 0]]
-        self.trades = trades.set_index('month')
-
-        # 总体数据
-        self.trades_win = self.trades > 0
-        self.trades_loss = self.trades < 0
-        self.winrate = self.trades_win.sum().values[0]/len(self.trades)
-        self.odds = -(self.trades[self.trades_win[0]].mean()/self.trades[self.trades_loss[0]].mean()).values[0]
-    def trade_plot(self):
-        # 交易次数
-        Close_count = self.Close_amount.reset_index()[['date',0]].set_index('date')
-        Close_count = Close_count.groupby('date').count().cumsum()
-        # 画图
-        plt, fig, ax = matplot()
-        ax.plot(Close_count, label='累积交易次数 胜率：%s 盈亏比：%s'%(round(self.winrate, 2), round(self.odds, 2)))
-        ax.set_xlim(self.net.index[0], self.net.index[-1])
-        ax.legend()
-        plt.gcf().autofmt_xdate()
-        plt.savefig('trade.png')
-        plt.show()
-    def trade_monthly(self):
-        # 月度盈利（亏损）交易的次数与平均盈利（亏损）。
-        count_win = self.trades_win.groupby('month').sum()
-        count_loss = self.trades_loss.groupby('month').sum()
-#        mean_win = trades[trades_win[0]].groupby('month').mean()
-#        mean_loss = trades[trades_loss[0]].groupby('month').mean()
-        # 月度胜率和盈亏比
-        self.month_winrate = count_win/(count_win + count_loss)
-#        self.month_odds = -mean_win/mean_loss
-        plt,fig,ax = month_thermal(self.month_winrate, 0.5)
-        plt.savefig('trade_monthly.png') 
-        plt.show()
-# 仓位分析
-    def position(self):
-        plt, fig, ax = matplot()
-        held_amount = self.held.groupby('date').sum()
-        # 0是资产 1是现金
-        df_total = pd.concat([self.held.groupby('date').sum(), self.cash], axis=1).fillna(0)
-        df_max = pd.concat([self.held.groupby('date').max(), self.cash], axis=1).fillna(0)
-        df_count = pd.concat([self.held.groupby('date').count(), self.cash], axis=1).fillna(0)
-        ax.plot(df_total[0]/df_total.sum(axis=1), label='非现金仓位')
-        ax.set_xlim(self.held.index[0][0], self.held.index[-1][0])
-        ax.legend(loc = 'upper left')
-        ax2 = ax.twinx()
-        #ax2.plot(self.held.groupby('date').count(), c="C2", label='持有标的数量')
-        # 如果不是单品种策略
-        if self.world.market.index[0][1] != 'onlyone':
-            ax.plot(df_max[0]/df_total.sum(axis=1), label='第一大持仓仓位')
-            ax2.plot(df_count[0], c="C2", label='持有标的数量')
-            ax2.legend(loc = 'upper right')
-        plt.gcf().autofmt_xdate()
-        plt.savefig('position.png')
-        plt.show()
-
-
-
-
-
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
+import datetime
+import statsmodels.api as sm
+from plottable import ColumnDefinition, ColDef, Table
+from matplotlib.colors import LinearSegmentedColormap
+from FreeBack.display import *
+import os
+# 该模块处理策略的后处理(业绩评价、归因）工作，主要包含：
+# 1. ReturnsPost 收益率序列后处理
+# 2. HoldPost 持仓矩阵后处理
+# 3. WorldPost barbybar模块World对象后处理
+
+
+############################################################################################
+####################### 处理收益率序列（简单收益率，非对数收益率） ###########################
+############################################################################################
+class ReturnsPost():
+    # benchmark dataframe 收益率序列
+    def __init__(self, returns, benchmark=0, stratname='策略'):
+        self.stratname = stratname
+        self.returns = returns
+        self.net = (1+returns).cumprod()
+        # 无风险利率
+        self.rf = 0.03
+        # 基准
+        if benchmark==0:
+            benchmark = pd.DataFrame(index = returns.index)
+            benchmark['zero'] = 0
+            self.benchmark = benchmark
+        self.benchmark = benchmark.loc[returns.index].fillna(0)
+        # 基准波动率
+        self.sigma_benchmark = np.exp(np.log(self.benchmark[\
+            self.benchmark.columns[0]]+1).std())-1
+        # 净值曲线
+        self.lr = np.log(self.returns + 1)
+        # 超额收益 默认第一个benchmark
+        self.excess_lr = self.lr-np.log(self.benchmark[self.benchmark.columns[0]]+1)
+        self.returns.index.name = 'date'
+        # 评价指标
+        # 年化收益率（+1）
+        self.years = (returns.index[-1]-returns.index[0]).days/365  
+        self.return_total = (returns+1).prod()                             
+        self.return_annual = self.return_total**(1/self.years)-1    
+        excess_total = np.exp(self.excess_lr.sum())                  # 超额收益
+        self.excess_return_annual = excess_total**(1/self.years)-1
+        # 年化波动率 shrpe
+        self.sigma = np.exp(self.lr.std())-1
+        self.sharpe = (self.return_annual - self.rf)/(self.sigma*np.sqrt(250))
+        # 超额年化波动率 shrpe
+        self.excess_sigma = np.exp(self.excess_lr.std())-1
+        self.excess_sharpe = (self.excess_return_annual - self.rf)/(self.excess_sigma*np.sqrt(250))
+        # 回撤
+        a = np.maximum.accumulate(self.net)
+        self.drawdown = (a-self.net)/a
+    def cal_complex(self):
+        # 复杂指标 
+        win = self.lr[self.lr>0]
+        loss = self.lr[self.lr<0]
+        excesswin = self.excess_lr[self.excess_lr>0]
+        excessloss = self.excess_lr[self.excess_lr<0]
+        # 下行波动率
+        self.sigma_down = np.exp((self.lr-\
+                            self.lr.mean()).apply(lambda x: min(x,0)).std())-1
+        # 跟踪误差
+        self.sigma_alpha = np.exp(np.std(self.lr-\
+                             np.log(self.benchmark[self.benchmark.columns[0]]+1)))-1
+        # 超额回撤
+        excess_net = np.exp(self.excess_lr.fillna(0).cumsum())
+        a = np.maximum.accumulate(excess_net)
+        self.excess_drawdown = (a-excess_net)/a
+        # CAPM (无风险收益为0)
+        y = self.returns.fillna(0)
+        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
+        x = sm.add_constant(x)
+        model = sm.OLS(y, x).fit()
+        # T-M 模型(无风险收益为0)
+        y = self.returns.fillna(0)
+        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
+        x = sm.add_constant(x)
+        model = sm.OLS(y, x).fit()
+        # 市场风险暴露
+        self.beta = model.params[self.benchmark.columns[0]]
+        # 市场波动无法解释的截距项
+        self.alpha = model.params['const'] 
+        #model.summary()
+        ## 索提诺比率   单位下行风险的超额收益
+        #self.sortino = (self.return_annual - self.rf)/(self.sigma_down*np.sqrt(250))
+        # 特雷诺指数  单位beta的超额收益
+        self.treynor  = (self.return_annual - self.rf)/self.beta 
+# 净值曲线
+# 时间起止（默认全部），是否显示细节,是否自定义输出图片名称，是否显示对数，是否显示超额
+    def pnl(self, timerange=None, detail=True, filename=None, log=False, excess=False):
+        plt, fig, ax = matplot()
+        # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
+        if type(timerange) != type(None):
+            # 时间段内净值与基准
+            net = self.net.loc[timerange[0]:timerange[1]]
+            returns = self.returns.loc[timerange[0]:timerange[1]]
+            # 计算夏普
+            years = (pd.to_datetime(timerange[1])-pd.to_datetime(timerange[0])).days/365
+            return_annual = (net[-1]/net[0])**(1/years)-1
+            std_annual = returns.std()*np.sqrt(250)
+            sharpe = (return_annual - self.rf)/std_annual
+            if detail:
+                # 回撤
+                a = np.maximum.accumulate(net)
+                drawdown = (a-net)/a 
+                ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
+                    round(100*return_annual,2), round(sharpe,2), 
+                        round(100*max(drawdown),2)), transform=ax.transAxes)
+                # 回撤
+                ax2 = ax.twinx()
+                ax2.fill_between(drawdown.index,-100*drawdown, 0, color='C1', alpha=0.1)
+                if excess:
+                    ax.plot(np.exp(self.excess_lr.loc[timerange[0]:timerange[1]].cumsum()), 
+                            c='C3', label='超额收益')
+            else:
+                ax.text(0.7,0.05,'Sharpe:  {}'.format(round(sharpe,2)), transform=ax.transAxes)
+            ax.plot(net/net[0], c='C0', label='p&l')
+            # 如果基准是0就不绘制了
+            if not (self.benchmark==0).any().values[0]:
+                # benchmark 匹配回测时间段, 基准从0开始
+                benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
+                benchmark.loc[self.net.index[0]] = 0
+                # colors of benchmark
+                colors_list = ['C4','C5','C6','C7']
+                for i in range(len(benchmark.columns)):
+                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), \
+                            c=colors_list[i], label=benchmark.columns[i])
+                if excess:
+                    ax.plot(np.exp(self.excess_lr.cumsum()), c='C3', label='超额收益')
+                plt.legend(loc='upper left')
+            if log:
+                # 对数坐标显示
+                ax.set_yscale("log")
+            ax.set_xlim(returns.index[0], returns.index[-1])
+            plt.gcf().autofmt_xdate()
+        else:
+    #评价指标
+            ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
+            round(100*self.return_annual,2), round(self.sharpe,2), 
+            round(100*max(self.drawdown),2)), transform=ax.transAxes)
+        # 净值与基准
+            ax.plot(self.net, c='C0', label=self.stratname)
+            # 如果基准是0就不绘制了
+            if not (self.benchmark==0).any().values[0]:
+                # benchmark 匹配回测时间段, 基准从0开始
+                benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
+                benchmark.loc[self.net.index[0]] = 0
+                # colors of benchmark
+                colors_list = ['C4','C5','C6','C7']
+                for i in range(len(benchmark.columns)):
+                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), \
+                            c=colors_list[i], label=benchmark.columns[i])
+                if excess:
+                    ax.plot(np.exp(self.excess_lr.cumsum()), c='C3', label='超额收益')
+                plt.legend(loc='upper left')
+            if log:
+                # 对数坐标显示
+                ax.set_yscale("log")
+            # 回撤
+            ax2 = ax.twinx()
+            ax2.fill_between(self.drawdown.index,-100*self.drawdown, 0, color='C1', alpha=0.1)
+            ax.set_ylabel('累计净值')
+            ax.set_xlabel('日期')
+            ax2.set_ylabel('回撤 (%)')
+            ax.set_xlim(self.net.index[0], self.net.index[-1])
+            plt.gcf().autofmt_xdate()
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        if type(filename) == type(None):
+            plt.savefig('./output/pnl.png')
+        else:
+            plt.savefig('./output/'+filename)
+        plt.show()
+
+
+
+############################################################################################
+################################### 处理持仓表 ##############################################
+############################################################################################
+class HoldPost(ReturnsPost):
+    def __init__(self, df_hold, market=None, \
+                 benchmark=0, stratname='策略'):
+        returns = df_hold.groupby('date')['next_returns'].mean()
+        super(HoldPost, self).__init__(returns, benchmark=benchmark, stratname=stratname) 
+
+
+
+########################################################################################################
+####################################  barbybar.world  ##################################################
+########################################################################################################
+
+# 传入barbybar运行完毕的world对象
+class WorldPost():
+    # benchmark为收益率（非对数收益率）
+    def __init__(self, world, benchmark=None, stratname='策略'):
+        # world
+        self.world = world
+        # 策略名
+        self.stratname = stratname
+        # 无风险利率
+        self.rf = 0.03
+        # 基准
+        if type(benchmark) == type(None):
+            benchmark = pd.DataFrame(index = world.series_net.index)
+            benchmark['zero'] = 0
+            self.benchmark = benchmark
+        self.benchmark = benchmark.loc[world.series_net.index].fillna(0)
+        self.sigma_benchmark = np.exp(np.log(self.benchmark[\
+            self.benchmark.columns[0]]+1).std())-1
+        self.details()
+
+# 策略详细评价指标
+    def details(self):
+        # 净值曲线
+        self.abs_net = self.world.series_net
+        self.net = self.world.series_net/self.world.series_net.iloc[0]
+        self.returns = self.net/self.net.shift() - 1
+        self.lr = np.log(self.returns + 1)
+        # 超额收益 默认第一个benchmark
+        self.excess_lr = self.lr  - np.log(self.benchmark[self.benchmark.columns[0]]+1)
+        self.returns.index.name = 'date'
+        # 评价指标
+        # 年化收益率
+        self.years = (self.net.index[-1]-self.net.index[0]).days/365
+        self.return_total = self.net[-1]/self.net[0]
+        self.return_annual = self.return_total**(1/self.years)-1
+        excess_total = np.exp(self.excess_lr.sum())
+        self.excess_return_annual = excess_total**(1/self.years)-1
+        # 年化波动率 shrpe
+        self.sigma = np.exp(self.lr.std())-1
+        self.sharpe = (self.return_annual - self.rf)/(self.sigma*np.sqrt(250))
+        # 超额年化波动率 shrpe
+        self.excess_sigma = np.exp(self.excess_lr.std())-1
+        self.excess_sharpe = (self.excess_return_annual - self.rf)/(self.excess_sigma*np.sqrt(250))
+        # 回撤
+        a = np.maximum.accumulate(self.net)
+        self.drawdown = (a-self.net)/a
+        # 持仓标的
+        self.df_hold = self.world.df_hold
+        held = self.world.df_hold.reset_index().melt(id_vars=['date']).set_index(['date', 'code'])
+        held = held['value'] * self.world.market['close']
+        self.held = held[(held != 0)&~np.isnan(held)]
+        # 现金
+        self.cash = self.world.series_cash
+        # 交割单
+        self.excute = self.world.df_excute.reset_index().set_index(['date', 'code', 'unique'])
+        # 换手率
+        occurance_amount = abs(self.excute['occurance_amount']).groupby('date').sum()
+        #turnover = (occurance_amount/(self.net*self.cash.iloc[0])).fillna(0)
+        turnover = (occurance_amount/self.world.series_net).fillna(0)
+        self.turnover = turnover.mean()*250
+
+        # 逐笔交易信息
+        self.trade()
+
+        # details 表格
+        win = self.lr[self.lr>0]
+        loss = self.lr[self.lr<0]
+        excesswin = self.excess_lr[self.excess_lr>0]
+        excessloss = self.excess_lr[self.excess_lr<0]
+        # 下行波动率
+        self.sigma_down = np.exp((self.lr-self.lr.mean()).apply(lambda x: min(x,0)).std())-1
+        # 跟踪误差
+        sigma_alpha = np.exp(np.std(self.lr-np.log(self.benchmark[self.benchmark.columns[0]]+1)))-1
+        # 超额回撤
+        excess_net = np.exp(self.excess_lr.fillna(0).cumsum())
+        a = np.maximum.accumulate(excess_net)
+        self.excess_drawdown = (a-excess_net)/a
+        # CAPM (无风险收益为0)
+        y = self.returns.fillna(0)
+        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
+        x = sm.add_constant(x)
+        model = sm.OLS(y, x).fit()
+        # T-M 模型(无风险收益为0)
+        y = self.returns.fillna(0)
+        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
+        x = sm.add_constant(x)
+        model = sm.OLS(y, x).fit()
+        # 市场风险暴露
+        self.beta = model.params[self.benchmark.columns[0]]
+        # 市场波动无法解释的截距项
+        self.alpha = model.params['const'] 
+        #model.summary()
+        ## 索提诺比率   单位下行风险的超额收益
+        #self.sortino = (self.return_annual - self.rf)/(self.sigma_down*np.sqrt(250))
+        # 特雷诺指数  单位beta的超额收益
+        self.treynor  = (self.return_annual - self.rf)/self.beta
+
+        col0 = pd.DataFrame(columns=['col0'])
+        col0.loc[0] = '运行时间（年, 日）'
+        col0.loc[1] = '%s, %s'%(round(self.years,1), len(self.net))
+        col0.loc[2] = '盈利次数（日）'
+        col0.loc[3] = len(win)
+        col0.loc[4] = '超额次数（日）'
+        col0.loc[5] = len(excesswin)
+        col0.loc[6] = '空仓次数（日）' 
+        col0.loc[7] = len(self.net)-len(win)-len(loss) 
+        col1 = pd.DataFrame(columns=['col1'])
+        col1.loc[0] = '年化收益率（%）'
+        col1.loc[1] = round(self.return_annual*100,1)
+        col1.loc[2] = '年化超额收益率（%）'
+        col1.loc[3] = round(self.excess_return_annual*100,1)
+        col1.loc[4] = '累计收益（%）'
+        col1.loc[5] = round((self.return_total-1)*100,1)
+        col1.loc[6] = '累计超额收益（%）'
+        col1.loc[7] = round((excess_total-1)*100,1)
+        col2 = pd.DataFrame(columns=['col2'])
+        col2.loc[0] = '日胜率（%）'
+        col2.loc[1] = round(100*len(win)/(len(win)+len(loss)),1) 
+        col2.loc[2] = '超额日胜率（%）'
+        col2.loc[3] = round(100*len(excesswin)/(len(excesswin)+\
+                                len(excessloss)),1) 
+        col2.loc[4] = '日盈亏比'
+        col2.loc[5] = round(win.mean()/abs(loss.mean()),2) 
+        col2.loc[6] = '亏损日平均亏损（万）'
+        col2.loc[7] = round(abs(loss.mean())*10000,1) 
+        col3 = pd.DataFrame(columns=['col3'])
+        col3.loc[0] = '最大回撤（%）'
+        col3.loc[1] = round(max(self.drawdown)*100, 1)
+        col3.loc[2] = '超额最大回撤（%）'
+        col3.loc[3] = round(max(self.excess_drawdown)*100, 1)
+        col3.loc[4] = '波动率（%）'
+        col3.loc[5] = round(self.sigma*np.sqrt(250)*100, 1)
+        col3.loc[6] = '基准波动率（%）'
+        col3.loc[7] = round(self.sigma_benchmark*np.sqrt(250)*100, 1)
+        col4 = pd.DataFrame(columns=['col4'])
+        col4.loc[0] = '下行波动率（%）'
+        col4.loc[1] = round(self.sigma_down*np.sqrt(250)*100, 1)
+        col4.loc[2] = 'beta系数'
+        col4.loc[3] = round(self.beta,2) 
+        col4.loc[4] = '跟踪误差（%）'
+        col4.loc[5] = round(sigma_alpha*np.sqrt(250)*100, 1)
+        col4.loc[6] = '年化换手' 
+        col4.loc[7] = round(self.turnover,1)
+        col5 = pd.DataFrame(columns=['col5'])
+        col5.loc[0] = '夏普比率'
+        col5.loc[1] = round(self.sharpe,2)
+        col5.loc[2] = '超额夏普' 
+        col5.loc[3] = round(self.excess_sharpe,2)
+        col5.loc[4] = '卡玛比率'
+        col5.loc[5] = round(self.return_annual/max(self.drawdown),2)
+        col5.loc[6] = '无风险收益率（%）' 
+        col5.loc[7] = self.rf*100 
+        col6 = pd.DataFrame(columns=['col6'])
+        col6.loc[0] = '詹森指数（alpha）'
+        #col6.loc[0] = '詹森指数'
+        col6.loc[1] = round(self.alpha*250*100,1) 
+        col6.loc[2] = '特雷诺指数'  # 单位beta的超额收益 
+        col6.loc[3] =  round(self.treynor, 2)
+        col6.loc[4] = '信息比率'   # 超额收益的夏普
+        col6.loc[5] = round(self.alpha*np.sqrt(250)/sigma_alpha,2) 
+        col6.loc[6] = '' 
+        col6.loc[7] = '' 
+        col7 = pd.DataFrame(columns=['col7'])
+        col7.loc[0] = 'Hurst指数' 
+        col7.loc[1] = '' 
+        col7.loc[2] = 'T-M模型' 
+        col7.loc[3] = '' 
+        col7.loc[4] = '' 
+        col7.loc[5] = '' 
+        col7.loc[6] = '' 
+        col7.loc[7] = '' 
+        df_details = pd.concat([col0, col1, col2, col3, \
+                col4, col5, col6, col7], axis=1)
+
+        plt, fig, ax = matplot(w=22)
+        column_definitions = [ColumnDefinition(name='col0', group="收益能力"), \
+                              ColumnDefinition(name='col1', group="收益能力"), \
+                            ColumnDefinition(name='col2', group='收益能力'), \
+                            ColumnDefinition(name='col3', group='风险水平'), \
+                            ColumnDefinition(name="col4", group='风险水平'), \
+                            ColumnDefinition(name="col5", group='风险调整'), \
+                            ColumnDefinition(name="col6", group='风险调整'),
+                            ColumnDefinition(name="col7", group='业绩持续性分析')] +\
+                            [ColDef("index", title="", width=1.5, textprops={"ha":"right"})]
+        tab = Table(df_details, row_dividers=False, col_label_divider=False, 
+                    column_definitions=column_definitions,
+                    odd_row_color="#e0f6ff", even_row_color="#f0f0f0", 
+                    textprops={"ha": "center"})
+        #ax.set_xlim(2,5)
+        # 设置列标题文字和背景颜色(隐藏表头名)
+        tab.col_label_row.set_facecolor("white")
+        tab.col_label_row.set_fontcolor("white")
+        # 设置行标题文字和背景颜色
+        tab.columns["index"].set_facecolor("white")
+        tab.columns["index"].set_fontcolor("white")
+        tab.columns["index"].set_linewidth(0)
+        plt.savefig('details.png')
+        plt.show()
+# 净值曲线
+    def pnl(self, timerange=None, detail=False, filename=None, log=False, excess=True):
+        plt, fig, ax = matplot(w=10)
+        # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
+        if type(timerange) != type(None):
+            # 时间段内净值与基准
+            net = self.net.loc[timerange[0]:timerange[1]]
+            returns = self.returns.loc[timerange[0]:timerange[1]]
+            # 计算夏普
+            years = (pd.to_datetime(timerange[1])-pd.to_datetime(timerange[0])).days/365
+            return_annual = (net[-1]/net[0])**(1/years)-1
+            std_annual = returns.std()*np.sqrt(250)
+            sharpe = (return_annual - self.rf)/std_annual
+            if detail:
+                # 回撤
+                a = np.maximum.accumulate(net)
+                drawdown = (a-net)/a 
+                ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
+                    round(100*return_annual,2), round(sharpe,2), 
+                        round(100*max(drawdown),2)), transform=ax.transAxes)
+                # 回撤
+                ax2 = ax.twinx()
+                ax2.fill_between(drawdown.index,-100*drawdown, 0, color='C1', alpha=0.1)
+                if excess:
+                    ax.plot(np.exp(self.excess_lr.loc[timerange[0]:timerange[1]].cumsum()), 
+                            c='C3', label='超额收益')
+            else:
+                ax.text(0.7,0.05,'Sharpe:  {}'.format(round(sharpe,2)), transform=ax.transAxes)
+            ax.plot(net/net[0], c='C0', label='p&l')
+            if type(self.benchmark) != type(None):
+                benchmark = self.benchmark.loc[timerange[0]:timerange[1]].copy()
+                benchmark.iloc[0] = 0
+        # colors of benchmark
+                colors_list = ['C4','C5','C6','C7']
+                for i in range(len(benchmark.columns)):
+                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), 
+                            c=colors_list[i], label=benchmark.columns[i])
+            if log:
+                # 对数坐标显示
+                ax.set_yscale("log")
+            ax.set_xlim(returns.index[0], returns.index[-1])
+            plt.gcf().autofmt_xdate()
+        else: 
+    #评价指标
+            ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
+            round(100*self.return_annual,2), round(self.sharpe,2), 
+            round(100*max(self.drawdown),2)), transform=ax.transAxes)
+        # 净值与基准
+            ax.plot(self.net, c='C0', label=self.stratname)
+            if type(self.benchmark) != type(None):
+                # benchmark 匹配回测时间段, 基准从0开始
+                benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
+                benchmark.loc[self.net.index[0]] = 0
+                # colors of benchmark
+                colors_list = ['C4','C5','C6','C7']
+                for i in range(len(benchmark.columns)):
+                    ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(),  c=colors_list[i], label=benchmark.columns[i])
+                if excess:
+                    ax.plot(np.exp(self.excess_lr.cumsum()), c='C3', label='超额收益')
+                plt.legend(loc='upper left')
+            if log:
+                # 对数坐标显示
+                ax.set_yscale("log")
+            # 回撤
+            ax2 = ax.twinx()
+            ax2.fill_between(self.drawdown.index,-100*self.drawdown, 0, color='C1', alpha=0.1)
+            ax.set_ylabel('累计净值')
+            ax.set_xlabel('日期')
+            ax2.set_ylabel('回撤 (%)')
+            ax.set_xlim(self.net.index[0], self.net.index[-1])
+            plt.gcf().autofmt_xdate()
+        if type(filename) == type(None):
+            plt.savefig('pnl.png')
+        else:
+            plt.savefig(filename)
+        plt.show()
+# 滚动收益
+    def rolling_return(self):
+        plt, fig, ax = matplot()
+        ax.plot((self.net/self.net.shift(120)-1)*100, c='C0', label='滚动半年收益')
+        #ax.plot((post0.net/post0.net.shift(60)-1)*4, c='C1', label='quarter return')
+        #ax.plot((post0.net/post0.net.shift(120)-1)*2, c='C3', label='half year return')
+        ax2 = ax.twinx()
+        ax2.plot((self.net/self.net.shift(250)-1)*100, c='C3', label='滚动年度收益')
+        ax.legend(loc='upper left')
+        ax2.legend(loc='upper right')
+        ax.set_ylabel(' (%)')
+        ax2.set_ylabel('(%)')
+        ax.set_xlim(self.returns.index[0], self.returns.index[-1])
+        plt.gcf().autofmt_xdate()
+        plt.savefig('rolling_return.png')
+        plt.show()
+# 滚动sharpe
+    def rolling_sharpe(self):
+        plt, fig, ax = matplot()
+        halfyearly_sharpe = (np.exp(self.lr.rolling(120).mean()*250)-1)/\
+            ((np.exp(self.lr.rolling(120).std())-1)*np.sqrt(250))
+        yearly_sharpe = (np.exp(self.lr.rolling(250).mean()*250)-1)/\
+            ((np.exp(self.lr.rolling(250).std())-1)*np.sqrt(250))
+        ax.plot(halfyearly_sharpe, c='C0', label='滚动半年sharpe')
+        ax2 = ax.twinx()
+        ax2.plot(yearly_sharpe, c='C3', label='滚动年度sharpe')
+        ax.legend(loc='upper left')
+        ax2.legend(loc='upper right')
+        ax.set_ylim(-3, 10)
+        ax.set_xlim(self.returns.index[0], self.returns.index[-1])
+        plt.gcf().autofmt_xdate()
+        plt.savefig('rolling_sharpe.png')
+# 月度收益
+    def pnl_monthly(self):
+        plt,fig,ax = plot_thermal(self.lr)
+        plt.savefig('pnl_monthly.png')
+        plt.show()
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
+        plt, fig, ax = matplot()
+
+        len_years = len(yearly_returns)
+        plot_x = range(len_years)
+        plot_index = yearly_returns.index
+        plot_height = yearly_returns['lr'].values
+        plot_height1 = yearly_returns['bench'].values
+
+        ax.bar([i-0.225  for i in plot_x], plot_height, width=0.45, color='C0', label='策略')
+        ax.bar([i+0.225  for i in plot_x], plot_height1, width=0.45, color='C4', label=self.benchmark.columns[0])
+
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
+        plt.ylabel('(%)')
+        plt.savefig('pnl_yearly.png')
+        plt.show()
+# 月度超额收益
+    def pnl_excess_monthly(self):
+        plt,fig,ax = plot_thermal(self.excess_lr)
+        plt.savefig('pnl_excess_monthly.png')
+        plt.show()
+# 交易分析
+    def trade(self):
+        self.CashFlow = self.excute.apply(lambda x: x['occurance_amount'] - x['comm'] if x['BuyOrSell']=='Sell' else -x['occurance_amount'] - x['comm'], axis=1)
+        # 获取持仓卖出变为0时的订单unique，记为一次交易结束(有可能会出现同时两个卖出订单误判为两次交易)
+        completes = list(self.excute[(self.excute['remain_vol'] == 0)&(self.excute['BuyOrSell']=='Sell')].reset_index()['unique'])
+        # 对每个标的的累积现金流
+        CumCashFlow = self.CashFlow.groupby('code').cumsum()
+        # 截取交易结束节点
+        Close_amount = CumCashFlow.reset_index().set_index('unique').loc[completes]
+        Close_amount = Close_amount.reset_index().set_index(['date', 'code', 'unique'])[0]
+        # 每次交易盈亏（当前交易结束的现金流-上一次交易结束的现金流 ）
+        self.Close_amount = Close_amount - Close_amount.groupby('code').shift().fillna(0)
+        trade_pnl = self.Close_amount.reset_index()[['date', 'code', 0]].set_index([\
+                                'date', 'code'])[0]
+        self.trade_pnl = trade_pnl.sort_values()/self.abs_net
+        # 筛出同月数据
+        trades = self.Close_amount.reset_index()
+        trades['month'] = trades['date'].apply(lambda x: x - datetime.timedelta(x.day-1)) 
+        trades = trades[['month', 0]]
+        self.trades = trades.set_index('month')
+
+        # 总体数据
+        self.trades_win = self.trades > 0
+        self.trades_loss = self.trades < 0
+        self.winrate = self.trades_win.sum().values[0]/len(self.trades)
+        self.odds = -(self.trades[self.trades_win[0]].mean()/self.trades[self.trades_loss[0]].mean()).values[0]
+    def trade_plot(self):
+        # 交易次数
+        Close_count = self.Close_amount.reset_index()[['date',0]].set_index('date')
+        Close_count = Close_count.groupby('date').count().cumsum()
+        # 画图
+        plt, fig, ax = matplot()
+        ax.plot(Close_count, label='累积交易次数 胜率：%s 盈亏比：%s'%(round(self.winrate, 2), round(self.odds, 2)))
+        ax.set_xlim(self.net.index[0], self.net.index[-1])
+        ax.legend()
+        plt.gcf().autofmt_xdate()
+        plt.savefig('trade.png')
+        plt.show()
+    def trade_monthly(self):
+        # 月度盈利（亏损）交易的次数与平均盈利（亏损）。
+        count_win = self.trades_win.groupby('month').sum()
+        count_loss = self.trades_loss.groupby('month').sum()
+#        mean_win = trades[trades_win[0]].groupby('month').mean()
+#        mean_loss = trades[trades_loss[0]].groupby('month').mean()
+        # 月度胜率和盈亏比
+        self.month_winrate = count_win/(count_win + count_loss)
+#        self.month_odds = -mean_win/mean_loss
+        plt,fig,ax = month_thermal(self.month_winrate, 0.5)
+        plt.savefig('trade_monthly.png') 
+        plt.show()
+# 仓位分析
+    def position(self):
+        plt, fig, ax = matplot()
+        held_amount = self.held.groupby('date').sum()
+        # 0是资产 1是现金
+        df_total = pd.concat([self.held.groupby('date').sum(), self.cash], axis=1).fillna(0)
+        df_max = pd.concat([self.held.groupby('date').max(), self.cash], axis=1).fillna(0)
+        df_count = pd.concat([self.held.groupby('date').count(), self.cash], axis=1).fillna(0)
+        ax.plot(df_total[0]/df_total.sum(axis=1), label='非现金仓位')
+        ax.set_xlim(self.held.index[0][0], self.held.index[-1][0])
+        ax.legend(loc = 'upper left')
+        ax2 = ax.twinx()
+        #ax2.plot(self.held.groupby('date').count(), c="C2", label='持有标的数量')
+        # 如果不是单品种策略
+        if self.world.market.index[0][1] != 'onlyone':
+            ax.plot(df_max[0]/df_total.sum(axis=1), label='第一大持仓仓位')
+            ax2.plot(df_count[0], c="C2", label='持有标的数量')
+            ax2.legend(loc = 'upper right')
+        plt.gcf().autofmt_xdate()
+        plt.savefig('position.png')
+        plt.show()
+
+
+
+
+
```

### Comparing `FreeBack-3.0.1a0/LICENSE` & `FreeBack-4.1.0a0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `FreeBack-3.0.1a0/setup.py` & `FreeBack-4.1.0a0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from setuptools import setup, find_packages
-from codecs import open
-
-with open("README.md","r",encoding='utf-8') as fh:
-    long_description = fh.read()
-
-setup(
-    name="FreeBack",
-    # 版本号: 第几次模块增加，第几次函数增加，第几次函数功能修改
-    # (每次高级别序号增加后,低级别序号归0)
-    # alpha为调试版,beta为测试版,stable为稳定版 
-    version="3.0.1-alpha",
-    author="LH.Li,zzq",
-    author_email="lh98lee@zju.edu.cn",  
-    description='Package for backtest',
-    long_description=long_description, 
-    # 描述文件为md格式
-    long_description_content_type="text/markdown",
-    url="https://github.com/LHanLi/FreeBack",
-    packages=find_packages(),
-    install_requires = [
-        'pandas',
-        'scipy',
-        'statsmodels',
-        'seaborn',
-        'plottable',
-        'pyecharts',
-        'numpy_ext',
-    ],
-    classifiers=[
-         # 该软件包仅与Python3兼容
-        "Programming Language :: Python :: 3",
-        # 根据GPL 3.0许可证开源
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-        # 与操作系统无关
-        "Operating System :: OS Independent",
-    ],
-)
-
-# python3 setup.py install --u
+from setuptools import setup, find_packages
+from codecs import open
+
+with open("README.md","r",encoding='utf-8') as fh:
+    long_description = fh.read()
+
+setup(
+    name="FreeBack",
+    # 版本号: 第几次模块增加，第几次函数增加，第几次函数功能修改
+    # (每次高级别序号增加后,低级别序号归0)
+    # alpha为调试版,beta为测试版,stable为稳定版 
+    version="4.1.0-alpha",
+    author="LH.Li,zzq",
+    author_email="lh98lee@zju.edu.cn",  
+    description='Package for backtest',
+    long_description=long_description, 
+    # 描述文件为md格式
+    long_description_content_type="text/markdown",
+    url="https://github.com/LHanLi/FreeBack",
+    packages=find_packages(),
+    install_requires = [
+        'pandas',
+        'scipy',
+        'statsmodels',
+        'seaborn',
+        'plottable',
+        'pyecharts',
+        'numpy_ext',
+    ],
+    classifiers=[
+         # 该软件包仅与Python3兼容
+        "Programming Language :: Python :: 3",
+        # 根据GPL 3.0许可证开源
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        # 与操作系统无关
+        "Operating System :: OS Independent",
+    ],
+)
+
+# python3 setup.py install --u
```

