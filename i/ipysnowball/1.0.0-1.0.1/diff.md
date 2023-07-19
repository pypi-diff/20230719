# Comparing `tmp/ipysnowball-1.0.0.tar.gz` & `tmp/ipysnowball-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipysnowball-1.0.0.tar", last modified: Tue Jun  6 09:18:09 2023, max compression
+gzip compressed data, was "ipysnowball-1.0.1.tar", last modified: Wed Jul 19 08:22:36 2023, max compression
```

## Comparing `ipysnowball-1.0.0.tar` & `ipysnowball-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-06-06 09:18:09.338344 ipysnowball-1.0.0/
--rw-r--r--   0 issa       (501) staff       (20)    11357 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/LICENSE
--rw-r--r--   0 issa       (501) staff       (20)     2813 2023-06-06 09:18:09.336060 ipysnowball-1.0.0/PKG-INFO
--rw-r--r--   0 issa       (501) staff       (20)    69770 2023-06-06 09:12:04.000000 ipysnowball-1.0.0/README.md
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-06-06 09:18:09.297809 ipysnowball-1.0.0/ipysnowball.egg-info/
--rw-r--r--   0 issa       (501) staff       (20)     2813 2023-06-06 09:18:09.000000 ipysnowball-1.0.0/ipysnowball.egg-info/PKG-INFO
--rw-r--r--   0 issa       (501) staff       (20)      561 2023-06-06 09:18:09.000000 ipysnowball-1.0.0/ipysnowball.egg-info/SOURCES.txt
--rw-r--r--   0 issa       (501) staff       (20)        1 2023-06-06 09:18:09.000000 ipysnowball-1.0.0/ipysnowball.egg-info/dependency_links.txt
--rw-r--r--   0 issa       (501) staff       (20)       40 2023-06-06 09:18:09.000000 ipysnowball-1.0.0/ipysnowball.egg-info/requires.txt
--rw-r--r--   0 issa       (501) staff       (20)       17 2023-06-06 09:18:09.000000 ipysnowball-1.0.0/ipysnowball.egg-info/top_level.txt
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-06-06 09:18:09.332780 ipysnowball-1.0.0/pysnowball/
--rw-r--r--   0 issa       (501) staff       (20)     1281 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/__init__.py
--rw-r--r--   0 issa       (501) staff       (20)     4964 2023-06-06 09:00:22.000000 ipysnowball-1.0.0/pysnowball/api_ref.py
--rw-r--r--   0 issa       (501) staff       (20)      260 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/bond.py
--rw-r--r--   0 issa       (501) staff       (20)      826 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/capital.py
--rw-r--r--   0 issa       (501) staff       (20)       72 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/cons.py
--rw-r--r--   0 issa       (501) staff       (20)      381 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/cube.py
--rw-r--r--   0 issa       (501) staff       (20)     1338 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/f10.py
--rw-r--r--   0 issa       (501) staff       (20)     1209 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/finance.py
--rw-r--r--   0 issa       (501) staff       (20)     1045 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/fund.py
--rw-r--r--   0 issa       (501) staff       (20)     2737 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/hkex.py
--rw-r--r--   0 issa       (501) staff       (20)     1272 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/index.py
--rw-r--r--   0 issa       (501) staff       (20)      516 2023-06-06 09:07:03.000000 ipysnowball-1.0.0/pysnowball/realtime.py
--rw-r--r--   0 issa       (501) staff       (20)      311 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/report.py
--rw-r--r--   0 issa       (501) staff       (20)      302 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/token.py
--rw-r--r--   0 issa       (501) staff       (20)      222 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/user.py
--rw-r--r--   0 issa       (501) staff       (20)     4284 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/pysnowball/utls.py
--rw-r--r--   0 issa       (501) staff       (20)       38 2023-06-06 09:18:09.339357 ipysnowball-1.0.0/setup.cfg
--rw-r--r--   0 issa       (501) staff       (20)     3250 2023-06-06 09:14:37.000000 ipysnowball-1.0.0/setup.py
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-06-06 09:18:09.334775 ipysnowball-1.0.0/tests/
--rw-r--r--   0 issa       (501) staff       (20)        0 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/tests/__init__.py
--rw-r--r--   0 issa       (501) staff       (20)     1178 2023-06-06 08:57:00.000000 ipysnowball-1.0.0/tests/test_fund.py
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 08:22:36.754533 ipysnowball-1.0.1/
+-rw-r--r--   0 issa       (501) staff       (20)    11357 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/LICENSE
+-rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 08:22:36.753617 ipysnowball-1.0.1/PKG-INFO
+-rw-r--r--   0 issa       (501) staff       (20)    70302 2023-07-19 08:08:48.000000 ipysnowball-1.0.1/README.md
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 08:22:36.732545 ipysnowball-1.0.1/ipysnowball.egg-info/
+-rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 08:22:36.000000 ipysnowball-1.0.1/ipysnowball.egg-info/PKG-INFO
+-rw-r--r--   0 issa       (501) staff       (20)      580 2023-07-19 08:22:36.000000 ipysnowball-1.0.1/ipysnowball.egg-info/SOURCES.txt
+-rw-r--r--   0 issa       (501) staff       (20)        1 2023-07-19 08:22:36.000000 ipysnowball-1.0.1/ipysnowball.egg-info/dependency_links.txt
+-rw-r--r--   0 issa       (501) staff       (20)       40 2023-07-19 08:22:36.000000 ipysnowball-1.0.1/ipysnowball.egg-info/requires.txt
+-rw-r--r--   0 issa       (501) staff       (20)       17 2023-07-19 08:22:36.000000 ipysnowball-1.0.1/ipysnowball.egg-info/top_level.txt
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 08:22:36.750271 ipysnowball-1.0.1/pysnowball/
+-rw-r--r--   0 issa       (501) staff       (20)     1323 2023-07-19 08:08:16.000000 ipysnowball-1.0.1/pysnowball/__init__.py
+-rw-r--r--   0 issa       (501) staff       (20)     5133 2023-07-19 07:54:07.000000 ipysnowball-1.0.1/pysnowball/api_ref.py
+-rw-r--r--   0 issa       (501) staff       (20)      260 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/bond.py
+-rw-r--r--   0 issa       (501) staff       (20)      826 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/capital.py
+-rw-r--r--   0 issa       (501) staff       (20)       72 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/cons.py
+-rw-r--r--   0 issa       (501) staff       (20)      381 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/cube.py
+-rw-r--r--   0 issa       (501) staff       (20)     1338 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/f10.py
+-rw-r--r--   0 issa       (501) staff       (20)     1209 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/finance.py
+-rw-r--r--   0 issa       (501) staff       (20)     1045 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/fund.py
+-rw-r--r--   0 issa       (501) staff       (20)     2737 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/hkex.py
+-rw-r--r--   0 issa       (501) staff       (20)     1272 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/index.py
+-rw-r--r--   0 issa       (501) staff       (20)      516 2023-06-06 09:07:03.000000 ipysnowball-1.0.1/pysnowball/realtime.py
+-rw-r--r--   0 issa       (501) staff       (20)      311 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/report.py
+-rw-r--r--   0 issa       (501) staff       (20)      298 2023-07-19 07:54:01.000000 ipysnowball-1.0.1/pysnowball/scan.py
+-rw-r--r--   0 issa       (501) staff       (20)      302 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/token.py
+-rw-r--r--   0 issa       (501) staff       (20)      222 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/user.py
+-rw-r--r--   0 issa       (501) staff       (20)     4284 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/pysnowball/utls.py
+-rw-r--r--   0 issa       (501) staff       (20)       38 2023-07-19 08:22:36.754733 ipysnowball-1.0.1/setup.cfg
+-rw-r--r--   0 issa       (501) staff       (20)     3253 2023-07-19 08:09:08.000000 ipysnowball-1.0.1/setup.py
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 08:22:36.752617 ipysnowball-1.0.1/tests/
+-rw-r--r--   0 issa       (501) staff       (20)        0 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/tests/__init__.py
+-rw-r--r--   0 issa       (501) staff       (20)     1178 2023-06-06 08:57:00.000000 ipysnowball-1.0.1/tests/test_fund.py
```

### Comparing `ipysnowball-1.0.0/LICENSE` & `ipysnowball-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/PKG-INFO` & `ipysnowball-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: ipysnowball
-Version: 1.0.0
-Summary: xueqiu api python client | 集成雪球API
+Version: 1.0.1
+Summary: 原版雪球Python API pysnowball 的修改
 Home-page: https://github.com/issaTan/pysnowball
 Author: IssaTan
 Author-email: tanxinhao.1990@gmail.com
-License: UNKNOWN
 Keywords: Financial Data,XueQiu,Snow Ball,雪球,Python Api
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# pysnowball
+# ipysnowball
 ===============
 
 ## quick start
 
 ```python
->>> import pysnowball as ball
+>>> import ipysnowball as ball
 >>> ball.set_token('xq_a_token=651af***************031c96a315c;')
 'xq_a_token=651af***************031c96a315c;'
 >>> ball.cash_flow('SH600000')
 ```
 
 ```json
 {
@@ -69,9 +67,7 @@
                     'ncf_from_fa ': [-18376000000.0, -1.6123496284447998]
                 }
             ]}, 
             'error_code ': 0, 
             'error_description': ''
         }
 ```
-
-
```

### Comparing `ipysnowball-1.0.0/README.md` & `ipysnowball-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,34 @@
 ball.kline('SZ002027')
 ball.kline('SZ002027', 300)
 ball.kline('SZ002027', 300, 'week')
 ```
 
 [结果显示](APIs/realtime_kline.md)
 
+
+### 筛选股票
+
+目前仅支持通过**当前价**和**本日成交量**筛选股票，第一参数为当前价格，第二参数为本日成交量。需要根据返回的`count`自行更新`page`。
+第三参数是市场，分别是：`US-美股、HK-港股、CN-沪深`
+第四参数为排序字段，第五参数为排序方向。
+
+参数如下：
+```
+screener(current, volume, category='US', order_by='current', order='desc', page='1', size='30')
+```
+
+
+```python
+import ipysnowball as ball
+ball.screener('15', 2000000)
+```
+
+
+
 ### 业绩预告
 
 按年度获取业绩预告数据
 
 ```python
 import ipysnowball as ball
 ball.earningforecast('SZ002027')
```

### Comparing `ipysnowball-1.0.0/ipysnowball.egg-info/PKG-INFO` & `ipysnowball-1.0.1/ipysnowball.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: ipysnowball
-Version: 1.0.0
-Summary: xueqiu api python client | 集成雪球API
+Version: 1.0.1
+Summary: 原版雪球Python API pysnowball 的修改
 Home-page: https://github.com/issaTan/pysnowball
 Author: IssaTan
 Author-email: tanxinhao.1990@gmail.com
-License: UNKNOWN
 Keywords: Financial Data,XueQiu,Snow Ball,雪球,Python Api
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# pysnowball
+# ipysnowball
 ===============
 
 ## quick start
 
 ```python
->>> import pysnowball as ball
+>>> import ipysnowball as ball
 >>> ball.set_token('xq_a_token=651af***************031c96a315c;')
 'xq_a_token=651af***************031c96a315c;'
 >>> ball.cash_flow('SH600000')
 ```
 
 ```json
 {
@@ -69,9 +67,7 @@
                     'ncf_from_fa ': [-18376000000.0, -1.6123496284447998]
                 }
             ]}, 
             'error_code ': 0, 
             'error_description': ''
         }
 ```
-
-
```

### Comparing `ipysnowball-1.0.0/ipysnowball.egg-info/SOURCES.txt` & `ipysnowball-1.0.1/ipysnowball.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 pysnowball/f10.py
 pysnowball/finance.py
 pysnowball/fund.py
 pysnowball/hkex.py
 pysnowball/index.py
 pysnowball/realtime.py
 pysnowball/report.py
+pysnowball/scan.py
 pysnowball/token.py
 pysnowball/user.py
 pysnowball/utls.py
 tests/__init__.py
 tests/test_fund.py
```

### Comparing `ipysnowball-1.0.0/pysnowball/__init__.py` & `ipysnowball-1.0.1/pysnowball/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
-name = "pysnowball"
+name = "ipysnowball"
 
-__author__ = 'Yang Yu'
+__author__ = 'Issa Tan'
 
 
 from pysnowball.finance import (cash_flow, indicator, balance, income, business)
 
 from pysnowball.report import (report, earningforecast)
 
 from pysnowball.capital import(
@@ -32,7 +32,9 @@
 from pysnowball.hkex import(
     northbound_shareholding_sh, northbound_shareholding_sz)
 
 from pysnowball.fund import (fund_detail, fund_info, fund_growth,
                              fund_nav_history, fund_derived, fund_asset,
                              fund_manager, fund_achievement, fund_trade_date)
 
+
+from pysnowball.scan import (screener)
```

### Comparing `ipysnowball-1.0.0/pysnowball/api_ref.py` & `ipysnowball-1.0.1/pysnowball/api_ref.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 
 # real time
 realtime_quote = "https://stock.xueqiu.com/v5/stock/realtime/quotec.json?symbol="
 realtime_pankou = "https://stock.xueqiu.com/v5/stock/realtime/pankou.json?symbol="
 realtime_quote_detail = "https://stock.xueqiu.com/v5/stock/quote.json?extend=detail&symbol="
 
 # kline
-
 kline = "https://stock.xueqiu.com/v5/stock/chart/kline.json?symbol={}&begin={}&period={}&type=before&count=-{}&indicator=kline,pe,pb,ps,pcf,market_capital,agt,ggt,balance"
 
+# screener
+screener = 'https://xueqiu.com/service/screener/screen?category={}&indcode=&order_by={}&order={}&page={}&size={}&only_count=0&current={}&pct=&volume={}&_={}'
+
 # user
 watch_list = "https://stock.xueqiu.com/v5/stock/portfolio/list.json?system=true"
 watch_stock = "https://stock.xueqiu.com/v5/stock/portfolio/stock/list.json?size=1000&category=1&pid="
 
 # cube
 nav_daily = "https://xueqiu.com/cubes/nav_daily/all.json?cube_symbol="
 rebalancing_history = "https://xueqiu.com/cubes/rebalancing/history.json?cube_symbol="
```

### Comparing `ipysnowball-1.0.0/pysnowball/capital.py` & `ipysnowball-1.0.1/pysnowball/capital.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/f10.py` & `ipysnowball-1.0.1/pysnowball/f10.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/finance.py` & `ipysnowball-1.0.1/pysnowball/finance.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/fund.py` & `ipysnowball-1.0.1/pysnowball/fund.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/hkex.py` & `ipysnowball-1.0.1/pysnowball/hkex.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/index.py` & `ipysnowball-1.0.1/pysnowball/index.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/realtime.py` & `ipysnowball-1.0.1/pysnowball/realtime.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/pysnowball/utls.py` & `ipysnowball-1.0.1/pysnowball/utls.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.0/setup.py` & `ipysnowball-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 long_desc = """
-# pysnowball
+# ipysnowball
 ===============
 
 ## quick start
 
 ```python
->>> import pysnowball as ball
+>>> import ipysnowball as ball
 >>> ball.set_token('xq_a_token=651af***************031c96a315c;')
 'xq_a_token=651af***************031c96a315c;'
 >>> ball.cash_flow('SH600000')
 ```
 
 ```json
 {
@@ -72,18 +72,18 @@
         'requests >= 2.18.4',
         'beautifulsoup4 >= 4.10.0'
     ]
     return reqs
 
 setuptools.setup(
     name="ipysnowball",
-    version="1.0.0",
+    version="1.0.1",
     author="IssaTan",
     author_email="tanxinhao.1990@gmail.com",
-    description="xueqiu api python client | 集成雪球API",
+    description="原版雪球Python API pysnowball 的修改",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/issaTan/pysnowball",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ipysnowball-1.0.0/tests/test_fund.py` & `ipysnowball-1.0.1/tests/test_fund.py`

 * *Files identical despite different names*

