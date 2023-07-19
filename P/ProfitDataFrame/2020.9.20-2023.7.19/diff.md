# Comparing `tmp/ProfitDataFrame-2020.9.20.tar.gz` & `tmp/ProfitDataFrame-2023.7.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ProfitDataFrame-2020.9.20.tar", last modified: Sun Sep 20 12:13:20 2020, max compression
+gzip compressed data, was "dist\ProfitDataFrame-2023.7.19.tar", last modified: Wed Jul 19 09:47:35 2023, max compression
```

## Comparing `ProfitDataFrame-2020.9.20.tar` & `ProfitDataFrame-2023.7.19.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/
--rw-rw-rw-   0        0        0      425 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/PKG-INFO
--rw-rw-rw-   0        0        0       42 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/setup.cfg
--rw-rw-rw-   0        0        0      935 2020-09-20 12:12:10.000000 ProfitDataFrame-2020.9.20/setup.py
-drwxrwxrwx   0        0        0        0 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/
-drwxrwxrwx   0        0        0        0 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame/
--rw-rw-rw-   0        0        0     6710 2020-09-20 10:22:23.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame/ProfitDataFrame.py
--rw-rw-rw-   0        0        0      118 2020-09-20 12:11:43.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame/__init__.py
-drwxrwxrwx   0        0        0        0 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame.egg-info/
--rw-rw-rw-   0        0        0      425 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2020-09-20 12:13:20.000000 ProfitDataFrame-2020.9.20/src/ProfitDataFrame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 09:47:35.250372 ProfitDataFrame-2023.7.19/
+-rw-rw-rw-   0        0        0      425 2023-07-19 09:47:35.250372 ProfitDataFrame-2023.7.19/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-19 09:47:35.250372 ProfitDataFrame-2023.7.19/setup.cfg
+-rw-rw-rw-   0        0        0      965 2023-07-19 09:47:19.000000 ProfitDataFrame-2023.7.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:47:35.241879 ProfitDataFrame-2023.7.19/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 09:47:35.243873 ProfitDataFrame-2023.7.19/src/ProfitDataFrame/
+-rw-rw-rw-   0        0        0     7901 2023-07-19 09:46:22.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame/ProfitDataFrame.py
+-rw-rw-rw-   0        0        0      118 2023-07-19 09:46:46.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:47:35.249342 ProfitDataFrame-2023.7.19/src/ProfitDataFrame.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-07-19 09:47:35.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-07-19 09:47:35.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 09:47:35.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-19 09:47:35.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 09:47:35.000000 ProfitDataFrame-2023.7.19/src/ProfitDataFrame.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ProfitDataFrame-2020.9.20/setup.py` & `ProfitDataFrame-2023.7.19/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-from distutils.core import setup
-from setuptools import find_packages
-
-name = 'ProfitDataFrame'
-version = '2020.9.20'
-author = 'Zhang Chuanpeng'
-author_email = 'yz7zzxj001@qq.com'
-description = '''This is a package for myself to make data analysis easily, it includes some functions 
-which only work with pandas.DataFrame.\n
-'''
-long_description = 'This is a package for myself to make data analysis easily'
-install_requires = ['pandas','numpy','matplotlib','seaborn','sklearn']
-
-setup(name = name
-        , version = version
-        ,long_description = long_description
-        ,author = author
-        ,author_email = author_email
-        ,description = description
-        ,install_requires = install_requires
-        ,keywords='data analysis tools'
-        ,packages = find_packages('src')
-        ,package_dir = {'':'src'}
-        ,include_package_data = True
-        ,url = ''
-        )  
-
+#!/usr/bin/env python
+# coding: utf-8
+
+from distutils.core import setup
+from setuptools import find_packages
+
+name = 'ProfitDataFrame'
+version = '2023.7.19'
+author = 'Zhang Chuanpeng'
+author_email = 'yz7zzxj001@qq.com'
+description = '''This is a package for myself to make data analysis easily, it includes some functions 
+which only work with pandas.DataFrame.\n
+'''
+long_description = 'This is a package for myself to make data analysis easily'
+install_requires = ['pandas','numpy','matplotlib','seaborn','sklearn']
+
+setup(name = name
+        , version = version
+        ,long_description = long_description
+        ,author = author
+        ,author_email = author_email
+        ,description = description
+        ,install_requires = install_requires
+        ,keywords='data analysis tools'
+        ,packages = find_packages('src')
+        ,package_dir = {'':'src'}
+        ,include_package_data = True
+        ,url = ''
+        )  
+
```

### Comparing `ProfitDataFrame-2020.9.20/src/ProfitDataFrame/ProfitDataFrame.py` & `ProfitDataFrame-2023.7.19/src/ProfitDataFrame/ProfitDataFrame.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 # coding: utf-8
 #author : Zhang Chuanpeng 张传鹏 
 #nickname :Zhang Xuanjin 张玄瑾 / yz7zzxj001
-#updated in  2020年9月15日
+#updated in  2023年7月19日
 #2020/5/26 profit q_info to suit whose index does not begins with 0
 #2020/5/27 fixing the5th which it goes well on my pc ,but mistake on others
 #2020/9/15 add 3 fuctions: gap_statistic finds best K in kmeans
 #          dup_corr show the corr between duplications 
 #          sta_describe show the kde and joinplot of numberic and bar of object
 #          增加了三个函数：区间间隔统计法寻找最优K值，重复值相关性探究每列重复值之间得相关性，以及数据分布描述
+#          sankey_type_data(x,result_is_df = True) make a df pivot table into a df that suit sunkey plot
 
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 import seaborn as sns
 
@@ -90,14 +91,15 @@
         if code == 3:
             print(r".q_info() show the infos of dataframe",
                 r".q_view() show the scatter_matrix of dataframe",
                 r".q_tips(code = 0) show the menu of this module",
                 r"gap_statistic(X,B = 10,K=range(1,11)) find the best K by gap_statistic in KMeanns",
                 r"dup_corr(X,nodatetime) show the corr of duplications in X . nodatetime means datatimeindex not in dups",
                 r".sta_describe(y_colname=None) show the kde and joinplot of numberic and bar of object"
+                r"sankey_type_data(x,result_is_df = True) make a df pivot table into a df that suit sunkey plot"
                 ,sep = '\r\n')
 
 
 def short_pair_wise_D(each_cluster):
     mu = each_cluster.mean(axis=0)
     Dk = sum(sum((each_cluster-mu)**2))*2.0*each_cluster.shape[0]
     return Dk
@@ -144,24 +146,47 @@
     gapDiff = gaps[:-1] - gaps[1:] + sk[1:]
     plt.bar(np.arange(len(gapDiff))+1,gapDiff)
     plt.xlabel('k')
     plt.ylabel('gapdiff')
     plt.show()
 
 def dup_corr(x,nodatetime = True):
+    """检验重复值相关性以确定重复值原因"""
     """注意，这里只判断dtype为object的重复值情况，因为如int/period/float重复值是没啥意义的"""
     tempdf = pd.DataFrame()
     for i in x.columns:
         if nodatetime:
             if x.loc[:,i].dtype == 'object':
                 tempdf[i] = x.loc[:,i].duplicated()
         else:
             if (x.loc[:,i].dtype == 'object') or (x.loc[:,i].dtype == 'DatetimeIndex'):
                 tempdf[i] = x.loc[:,i].duplicated()
     plt.figure(figsize =(10,10))
     sns.heatmap(tempdf.corr(),annot = True)
 
 
-
+def sankey_type_data(x,result_is_df = True):
+    """将df转换为符合桑基图绘制形式的关系网络图数据集。要求输入数据是一个透视表"""
+    nodes =[]
+    columns = x.columns.tolist()
+    for column in columns[:-1]:
+        nodes =nodes + (x[column].tolist())
+    py_nodes =[] # 提取了node数值数据
+    for i in list(set(nodes)):
+        dic = {}
+        dic['name'] = i
+        py_nodes.append(dic)
+    links = pd.DataFrame(columns=['source', 'target', 'value'])
+    for i in range(len(columns)-2):
+        ass = x[columns[-1]].groupby([x[columns[i]],x[columns[i+1]]]).sum()
+        sublinks = pd.DataFrame(ass.reset_index())
+        sublinks.columns = ['source', 'target', 'value']
+        links=links.append(sublinks)
+    py_links = links.to_dict('records')
+    if result_is_df :
+        df_sankey = pd.DataFrame(py_links)
+        return df_sankey
+    or:
+        return py_links
```

