# Comparing `tmp/stock-open-api-0.0.3.tar.gz` & `tmp/stock-open-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.3.tar", last modified: Tue Jul 18 14:41:57 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.4.tar", last modified: Wed Jul 19 07:49:30 2023, max compression
```

## Comparing `stock-open-api-0.0.3.tar` & `stock-open-api-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/api/sse/sh_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 07:49:15.000000 stock-open-api-0.0.4/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-19 07:49:29.000000 stock-open-api-0.0.4/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-19 07:49:30.000000 stock-open-api-0.0.4/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:49:29.000000 stock-open-api-0.0.4/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 07:49:29.000000 stock-open-api-0.0.4/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 07:49:29.000000 stock-open-api-0.0.4/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:49:29.000000 stock-open-api-0.0.4/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.3/PKG-INFO` & `stock-open-api-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
         
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domain-admin)](https://pypi.org/project/domain-admin)
-        [![PyPI](https://img.shields.io/pypi/v/domain-admin.svg)](https://pypi.org/project/domain-admin)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/domain-admin?label=pypi%20downloads)](https://pypi.org/project/domain-admin)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stock-open-api)](https://pypi.org/project/stock-open-api)
+        [![PyPI](https://img.shields.io/pypi/v/stock-open-api.svg)](https://pypi.org/project/stock-open-api)
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/stock-open-api?label=pypi%20downloads)](https://pypi.org/project/stock-open-api)
+        [![Documentation Status](https://readthedocs.org/projects/stock-open-api/badge/?version=latest)](https://stock-open-api.readthedocs.io/zh_CN/latest/?badge=latest)
         
         股票数据接口
         
         数据来自网上公开数据，仅做学习交流使用，不可用于商业用途
         
         - github: [https://github.com/mouday/stock-open-api](https://github.com/mouday/stock-open-api)
         - pypi: [https://pypi.org/project/stock-open-api/](https://pypi.org/project/stock-open-api/)
+        - 项目文档：[https://stock-open-api.readthedocs.io/zh_CN/latest/](https://stock-open-api.readthedocs.io/zh_CN/latest/stock_open_api.html#module-stock_open_api)
+        - 项目主页：[https://mouday.github.io/stock-open-api/](https://mouday.github.io/stock-open-api/)
         
         ## 安装
         
         ```bash
         pip install stock-open-api
         ```
         
@@ -107,14 +110,23 @@
         | [科创板-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/kcb_stock.get_company_info |
         | [新三板-列表](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list |
         | [新三板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list_iter |
         | [新三板-公司资料+证券资料](http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html) | api/eastmoney/neeq_stock.get_company_info |
         | [A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/company.get_company_info |
         | [深圳A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sz_stock.get_company_info |
         
+        ## 升级记录 
+         
+        [CHANGELOG.md](https://github.com/mouday/stock-open-api/blob/master/CHANGELOG.md)
+        
+        ## 其他相关库
+        
+        - AKShare 开源财经数据接口库 [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)
+        - Tushare 免费提供各类数据 , 助力行业和量化研究。 [https://github.com/waditu/tushare](https://github.com/waditu/tushare)
+        
 Keywords: stock,api
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `stock-open-api-0.0.3/README.md` & `stock-open-api-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Stock Open Api
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domain-admin)](https://pypi.org/project/domain-admin)
-[![PyPI](https://img.shields.io/pypi/v/domain-admin.svg)](https://pypi.org/project/domain-admin)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/domain-admin?label=pypi%20downloads)](https://pypi.org/project/domain-admin)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stock-open-api)](https://pypi.org/project/stock-open-api)
+[![PyPI](https://img.shields.io/pypi/v/stock-open-api.svg)](https://pypi.org/project/stock-open-api)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/stock-open-api?label=pypi%20downloads)](https://pypi.org/project/stock-open-api)
+[![Documentation Status](https://readthedocs.org/projects/stock-open-api/badge/?version=latest)](https://stock-open-api.readthedocs.io/zh_CN/latest/?badge=latest)
 
 股票数据接口
 
 数据来自网上公开数据，仅做学习交流使用，不可用于商业用途
 
 - github: [https://github.com/mouday/stock-open-api](https://github.com/mouday/stock-open-api)
 - pypi: [https://pypi.org/project/stock-open-api/](https://pypi.org/project/stock-open-api/)
+- 项目文档：[https://stock-open-api.readthedocs.io/zh_CN/latest/](https://stock-open-api.readthedocs.io/zh_CN/latest/stock_open_api.html#module-stock_open_api)
+- 项目主页：[https://mouday.github.io/stock-open-api/](https://mouday.github.io/stock-open-api/)
 
 ## 安装
 
 ```bash
 pip install stock-open-api
 ```
 
@@ -98,7 +101,16 @@
 | [科创板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list_iter |
 | [科创板-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/kcb_stock.get_company_info |
 | [新三板-列表](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list |
 | [新三板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list_iter |
 | [新三板-公司资料+证券资料](http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html) | api/eastmoney/neeq_stock.get_company_info |
 | [A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/company.get_company_info |
 | [深圳A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sz_stock.get_company_info |
+
+## 升级记录 
+ 
+[CHANGELOG.md](https://github.com/mouday/stock-open-api/blob/master/CHANGELOG.md)
+
+## 其他相关库
+
+- AKShare 开源财经数据接口库 [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)
+- Tushare 免费提供各类数据 , 助力行业和量化研究。 [https://github.com/waditu/tushare](https://github.com/waditu/tushare)
```

### Comparing `stock-open-api-0.0.3/setup.py` & `stock-open-api-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/company.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,81 @@
 # -*- coding: utf-8 -*-
 """
-@File    : company.py
+@File    : sz_stock.py
 @Date    : 2023-07-18
+深圳证券交易所
 """
-import json
 
-from stock_open_api.api.eastmoney import company_config
-from stock_open_api.utils import request_util
+from stock_open_api.api.eastmoney import company
+from stock_open_api.utils import json_util
 
 
 def get_company_info(code):
     """
-    公司 基本资料 | 发行相关
+    深圳证券交易所 公司 基本资料 | 发行相关
     http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801
 
-    :param code: str eg:
-        深圳证券交易所 SZ301398 或者 sz301398
-        上海证券交易所 SH688627 或者 sh688627
+    :param code: str eg: 688627
 
     :return:
-    {
-      "公司名称": "志邦家居股份有限公司",
-      "英文名称": "Zbom Home Collection Co.,Ltd",
-      "A股代码": "603801",
-      "A股简称": "志邦家居",
-      "A股扩位简称": null,
-      "曾用名": "志邦股份",
-      "B股代码": null,
-      "B股简称": null,
-      "H股代码": null,
-      "H股简称": null,
-      "证券类别": "上交所主板A股",
-      "上市交易所": "上海证券交易所",
-      "所属东财行业": "轻工制造-家具-家具制造",
-      "所属证监会行业": "鲁昌华,张京跃,王文兵",
-      "总经理": "许帮顺",
-      "法人代表": "孙志勇",
-      "董秘": "孙娟",
-      "董事长": "孙志勇",
-      "证券事务代表": "臧晶晶",
-      "独立董事": "鲁昌华,张京跃,王文兵",
-      "联系电话": "0551-67186564",
-      "电子信箱": "zbom@zbom.com",
-      "传真": "0551-65203999",
-      "公司网址": "www.zbom.com",
-      "办公地址": "安徽省合肥市庐阳工业区连水路19号",
-      "注册地址": "安徽省合肥市庐阳工业区连水路19号",
-      "区域": "安徽",
-      "邮政编码": "230061",
-      "注册资本(元)": 43654.7813,
-      "工商登记": "91340100772816763N",
-      "雇员人数": 5151,
-      "管理人员人数": 16,
-      "律师事务所": "安徽天禾律师事务所",
-      "会计师事务所": "大华会计师事务所(特殊普通合伙)",
-      "公司介绍": "志邦家居股份有限公司创立于1998年,是中国厨柜行业的先行者。现在,志邦专注于整家定制家居的研发、设计、生产与销售。从“更懂生活”的品牌理念出发,以整家生活的定制设计和服务为优势,为亿万家庭提供从厨房到全屋的整家解决方案。作为整家定制领域的专业家居品牌,志邦家居为人们提供整体厨房、全屋定制、木门墙板、成品家配为核心的整家一体化设计、制造、交付业务,在全国拥有六大生产基地,引进国外智能化制造设备,整合优质供应链,确保产品从设计、生产、安装到服务的每一个环节都以人为尺度、以生活为核心,为全球家庭创造理想的家居良品。凭借卓越的品质和口碑,志邦家居获得“中国环境标志认证”“FSC国际森林认证”等60余项国内外权威认证,同时成为国内诸多知名地产商的重要战略合作伙伴;志邦家居的产品远销海外,出口至澳洲、北美、东南亚、中东等国家和地区,是丽思卡尔顿、瑰丽酒店等国际五星级酒店优质供应商,在东南亚开设多家品牌专营店,品牌享誉全球。自2009年起,志邦家居与央视等主流媒体达成战略合作,并于2016年强势进驻纽约时代广场。同年签约前世界跳水冠军郭晶晶女士为品牌形象代言人,并先后联手郎平、杜丽等世界冠军和蔡康永、陈小春、罗嘉良、许茹芸、杨烁、孙杨、吴莫愁、王耀庆、钟汉良、张智霖、李晨等众多明星共同为美好生活赋义。2017年6月30日,志邦家居在上交所A股上市,2019年1月,正式签约世界著名音乐人周杰伦先生为品牌全新形象代言人。未来,我们将以专业的整家定制服务,发现和满足人们对生活空间的需求;以前沿的产品设计,引领和启发人们对生活品质的向往;以稳健的成长,为社会的良性发展创造更多真实的价值。志邦家居致力成为中国家居行业的一流企业、全球家居行业的领先企业,为现实现人们对家的美好想象奋力前行。",
-      "经营范围": "家具制造;家具零配件生产;家具零配件销售;家具销售;家具安装和维修服务;地板制造;地板销售;门窗制造加工;门窗销售;金属门窗工程施工;楼梯制造;楼梯销售;家居用品制造;家居用品销售;建筑装饰材料销售;木材加工;家用电器研发;家用电器制造;家用电器销售;家用电器零配件销售;家用电器安装服务;家用纺织制成品制造;非电力家用器具制造;非电力家用器具销售;卫生洁具研发;卫生洁具制造;卫生洁具销售;厨具卫具及日用杂品研发;厨具卫具及日用杂品批发;厨具卫具及日用杂品零售;日用品销售;灯具销售;互联网销售(除销售需要许可的商品);五金产品批发;五金产品零售;燃气器具生产;电子产品销售;第一类医疗器械销售;第二类医疗器械销售;普通货物仓储服务(不含危险化学品等需许可审批的项目);装卸搬运;会议及展览服务;供应链管理服务;专业设计服务;工业设计服务;咨询策划服务;住房租赁;非居住房地产租赁;货物进出口。",
-      "成立日期": "2005-04-04",
-      "上市日期": "2017-06-30",
-      "发行市盈率(倍)": 22.92,
-      "网上发行日期": "2017-06-20",
-      "发行方式": "网上定价发行,网下询价配售,市值申购",
-      "每股面值(元)": 1,
-      "发行量(股)": 40000000,
-      "每股发行价(元)": 23.47,
-      "发行费用(元)": 89434000,
-      "发行总市值(元)": 938800000,
-      "募集资金净额(元)": 849366000,
-      "首日开盘价(元)": 33.8,
-      "首日收盘价(元)": 33.8,
-      "首日换手率": 0.0914,
-      "首日最高价(元)": 33.8,
-      "网下配售中签率": 0.02743221,
-      "定价中签率": 0.03205759
-    }
+        {
+          "公司名称": "志邦家居股份有限公司",
+          "英文名称": "Zbom Home Collection Co.,Ltd",
+          "A股代码": "603801",
+          "A股简称": "志邦家居",
+          "A股扩位简称": null,
+          "曾用名": "志邦股份",
+          "B股代码": null,
+          "B股简称": null,
+          "H股代码": null,
+          "H股简称": null,
+          "证券类别": "上交所主板A股",
+          "上市交易所": "上海证券交易所",
+          "所属东财行业": "轻工制造-家具-家具制造",
+          "所属证监会行业": "鲁昌华,张京跃,王文兵",
+          "总经理": "许帮顺",
+          "法人代表": "孙志勇",
+          "董秘": "孙娟",
+          "董事长": "孙志勇",
+          "证券事务代表": "臧晶晶",
+          "独立董事": "鲁昌华,张京跃,王文兵",
+          "联系电话": "0551-67186564",
+          "电子信箱": "zbom@zbom.com",
+          "传真": "0551-65203999",
+          "公司网址": "www.zbom.com",
+          "办公地址": "安徽省合肥市庐阳工业区连水路19号",
+          "注册地址": "安徽省合肥市庐阳工业区连水路19号",
+          "区域": "安徽",
+          "邮政编码": "230061",
+          "注册资本(元)": 43654.7813,
+          "工商登记": "91340100772816763N",
+          "雇员人数": 5151,
+          "管理人员人数": 16,
+          "律师事务所": "安徽天禾律师事务所",
+          "会计师事务所": "大华会计师事务所(特殊普通合伙)",
+          "公司介绍": "志邦家居股份有限公司创立于1998年,是中国厨柜行业的先行者。现在,志邦专注于整家定制家居的研发、设计、生产与销售。从“更懂生活”的品牌理念出发,以整家生活的定制设计和服务为优势,为亿万家庭提供从厨房到全屋的整家解决方案。作为整家定制领域的专业家居品牌,志邦家居为人们提供整体厨房、全屋定制、木门墙板、成品家配为核心的整家一体化设计、制造、交付业务,在全国拥有六大生产基地,引进国外智能化制造设备,整合优质供应链,确保产品从设计、生产、安装到服务的每一个环节都以人为尺度、以生活为核心,为全球家庭创造理想的家居良品。凭借卓越的品质和口碑,志邦家居获得“中国环境标志认证”“FSC国际森林认证”等60余项国内外权威认证,同时成为国内诸多知名地产商的重要战略合作伙伴;志邦家居的产品远销海外,出口至澳洲、北美、东南亚、中东等国家和地区,是丽思卡尔顿、瑰丽酒店等国际五星级酒店优质供应商,在东南亚开设多家品牌专营店,品牌享誉全球。自2009年起,志邦家居与央视等主流媒体达成战略合作,并于2016年强势进驻纽约时代广场。同年签约前世界跳水冠军郭晶晶女士为品牌形象代言人,并先后联手郎平、杜丽等世界冠军和蔡康永、陈小春、罗嘉良、许茹芸、杨烁、孙杨、吴莫愁、王耀庆、钟汉良、张智霖、李晨等众多明星共同为美好生活赋义。2017年6月30日,志邦家居在上交所A股上市,2019年1月,正式签约世界著名音乐人周杰伦先生为品牌全新形象代言人。未来,我们将以专业的整家定制服务,发现和满足人们对生活空间的需求;以前沿的产品设计,引领和启发人们对生活品质的向往;以稳健的成长,为社会的良性发展创造更多真实的价值。志邦家居致力成为中国家居行业的一流企业、全球家居行业的领先企业,为现实现人们对家的美好想象奋力前行。",
+          "经营范围": "家具制造;家具零配件生产;家具零配件销售;家具销售;家具安装和维修服务;地板制造;地板销售;门窗制造加工;门窗销售;金属门窗工程施工;楼梯制造;楼梯销售;家居用品制造;家居用品销售;建筑装饰材料销售;木材加工;家用电器研发;家用电器制造;家用电器销售;家用电器零配件销售;家用电器安装服务;家用纺织制成品制造;非电力家用器具制造;非电力家用器具销售;卫生洁具研发;卫生洁具制造;卫生洁具销售;厨具卫具及日用杂品研发;厨具卫具及日用杂品批发;厨具卫具及日用杂品零售;日用品销售;灯具销售;互联网销售(除销售需要许可的商品);五金产品批发;五金产品零售;燃气器具生产;电子产品销售;第一类医疗器械销售;第二类医疗器械销售;普通货物仓储服务(不含危险化学品等需许可审批的项目);装卸搬运;会议及展览服务;供应链管理服务;专业设计服务;工业设计服务;咨询策划服务;住房租赁;非居住房地产租赁;货物进出口。",
+          "成立日期": "2005-04-04",
+          "上市日期": "2017-06-30",
+          "发行市盈率(倍)": 22.92,
+          "网上发行日期": "2017-06-20",
+          "发行方式": "网上定价发行,网下询价配售,市值申购",
+          "每股面值(元)": 1,
+          "发行量(股)": 40000000,
+          "每股发行价(元)": 23.47,
+          "发行费用(元)": 89434000,
+          "发行总市值(元)": 938800000,
+          "募集资金净额(元)": 849366000,
+          "首日开盘价(元)": 33.8,
+          "首日收盘价(元)": 33.8,
+          "首日换手率": 0.0914,
+          "首日最高价(元)": 33.8,
+          "网下配售中签率": 0.02743221,
+          "定价中签率": 0.03205759
+        }
 
     """
-    url = 'http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/PageAjax'
-
-    params = {
-        'code': code
-    }
-
-    res = request_util.get(url, params)
-
-    company_info = res.json()['jbzl'][0]
-    security_info = res.json()['fxxg'][0]
-
-    company_info.update(security_info)
-
-    item = {}
-    for row in company_config.company_key_map:
-        value = company_info.get(row['key'])
-        if isinstance(value, str):
-            value = value.strip()
-
-        # 上市日期 成立日期 网上发行日期
-        if row['key'] in ['LISTING_DATE', 'FOUND_DATE', 'ONLINE_ISSUE_DATE']:
-            value = value.split(' ')[0]
-
-        item[row['title']] = value
-
-    return item
+    return company.get_company_info("SZ{}".format(code))
 
 
 if __name__ == '__main__':
-    print(json.dumps(get_company_info('sh603801'), indent=2, ensure_ascii=False))
+    print(json_util.encode_json(get_company_info('301398')))
```

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/company_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # -*- coding: utf-8 -*-
 """
 @File    : hk_stock.py
 @Date    : 2023-07-17
+
 港股相关接口
 """
+
 import json
 
 from stock_open_api.api.eastmoney import hk_stock_config
 from stock_open_api.items.list_item import ListItem
 from stock_open_api.utils import time_util, request_util
 
 
 def get_list(page=1, size=20):
-    """
-    港股列表
+    """港股行情列表
+
     东方财富网 > 行情中心 > 港股市场 > 全部港股
     http://quote.eastmoney.com/center/gridlist.html#hk_stocks
 
-    :param page: int
-    :param size: int
+    :param page: 分页
+    :type page: int
+    :param size: 分页大小
+    :type size: int
 
-    :return: ListItem
+    :return: 港股行情列表
+    :rtype: ListItem
+
+    >>> get_list()
     {
       "total": 4587,
       "items": [
         {
           "代码": "00491",
           "名称": "英皇文化产业",
           "最新价": 0.075,
@@ -78,35 +85,18 @@
 
         items.append(item)
 
     list_item.items = items
     return list_item
 
 
-def get_list_iter(size=100):
-    """
-    列表迭代器
-    :param size: int
-    :return:
-    """
-    page = 0
-
-    while True:
-        page += 1
-
-        data = get_list(page, size)
-        if len(data.items) == 0:
-            break
-
-        yield data
-
-
 def get_org_profile(code):
     """
     公司资料
+
     http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile
 
     :param code: str eg: 00491
 
     :return:
     {
       "证券代码": "00491.HK",
```

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,32 +88,14 @@
 
         items.append(item)
 
     list_item.items = items
     return list_item
 
 
-def get_list_iter(size=100):
-    """
-    科创板 列表迭代器
-    :param size: int
-    :return:
-    """
-    page = 0
-
-    while True:
-        page += 1
-
-        data = get_list(page, size)
-        if len(data.items) == 0:
-            break
-
-        yield data
-
-
 def get_company_info(code):
     """
     科创板 公司 基本资料 | 发行相关
     http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801
 
     :param code: str eg: 688627
```

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,32 +81,14 @@
 
         items.append(item)
 
     list_item.items = items
     return list_item
 
 
-def get_list_iter(size=100):
-    """
-    新三板 列表迭代器
-    :param size: int
-    :return:
-    """
-    page = 0
-
-    while True:
-        page += 1
-
-        data = get_list(page, size)
-        if len(data.items) == 0:
-            break
-
-        yield data
-
-
 def get_company_info(code):
     """
     新三板 公司资料+证券资料
     eg: http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html
 
     :param code: str eg: 839499
```

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @Date    : 2023-07-17
 中国概念股相关接口
 """
 import json
 
 from stock_open_api.api.eastmoney import us_chinese_stock_config
 from stock_open_api.items.list_item import ListItem
+from stock_open_api.log import logger
 from stock_open_api.utils import time_util, request_util
 
 
 def get_list(page=1, size=20):
     """
     中国概念股 列表
     东方财富网 > 行情中心 > 美股市场 > 中国概念股
@@ -78,32 +79,14 @@
 
         items.append(item)
 
     list_item.items = items
     return list_item
 
 
-def get_list_iter(size=100):
-    """
-    列表迭代器
-    :param size: int
-    :return:
-    """
-    page = 0
-
-    while True:
-        page += 1
-
-        data = get_list(page, size)
-        if len(data.items) == 0:
-            break
-
-        yield data
-
-
 def get_org_profile(code):
     """
     中国概念股 公司资料
     http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/gszl
 
     :param code: str eg: PWM
 
@@ -121,14 +104,17 @@
       "公司网址": "www.prestigewealthinc.com",
       "E-MAIL": null,
       "电话号码": "+852 2122-8560",
       "传真号码": "+852 2122 8589",
       "公司介绍": "盛德财富有限公司是一家在开曼群岛注册成立的境外控股母公司,主要由其境内实体子公司Prestige Financial Holdings Group Limited运营。盛德财富有限公司(“PWI”,或“公司”)是一家于2018年10月25日根据开曼群岛法律成立的有限公司。该公司通过其子公司向高净值和超高净值个人和企业提供私人财富管理服务和资产管理。"
     }
     """
+    detail_url = 'http://emweb.eastmoney.com/PC_USF10/pages/index.html?code={}&type=web&color=w#/gsgk/gszl'.format(code)
+    logger.debug(detail_url)
+
     url = 'https://datacenter.eastmoney.com/securities/api/data/v1/get'
 
     params = {
         'reportName': 'RPT_USF10_INFO_ORGPROFILE',
         'columns': 'SECUCODE,SECURITY_CODE,ORG_CODE,SECURITY_INNER_CODE,ORG_NAME,ORG_EN_ABBR,BELONG_INDUSTRY,FOUND_DATE,CHAIRMAN,REG_PLACE,ADDRESS,EMP_NUM,ORG_TEL,ORG_FAX,ORG_EMAIL,ORG_WEB,ORG_PROFILE',
         'quoteColumns': '',
         'filter': '(SECURITY_CODE="{}")'.format(code),
```

### Comparing `stock-open-api-0.0.3/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-0.0.4/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-0.0.4/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-0.0.4/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api/utils/request_util.py` & `stock-open-api-0.0.4/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.3/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-0.0.4/stock_open_api.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
         
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domain-admin)](https://pypi.org/project/domain-admin)
-        [![PyPI](https://img.shields.io/pypi/v/domain-admin.svg)](https://pypi.org/project/domain-admin)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/domain-admin?label=pypi%20downloads)](https://pypi.org/project/domain-admin)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stock-open-api)](https://pypi.org/project/stock-open-api)
+        [![PyPI](https://img.shields.io/pypi/v/stock-open-api.svg)](https://pypi.org/project/stock-open-api)
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/stock-open-api?label=pypi%20downloads)](https://pypi.org/project/stock-open-api)
+        [![Documentation Status](https://readthedocs.org/projects/stock-open-api/badge/?version=latest)](https://stock-open-api.readthedocs.io/zh_CN/latest/?badge=latest)
         
         股票数据接口
         
         数据来自网上公开数据，仅做学习交流使用，不可用于商业用途
         
         - github: [https://github.com/mouday/stock-open-api](https://github.com/mouday/stock-open-api)
         - pypi: [https://pypi.org/project/stock-open-api/](https://pypi.org/project/stock-open-api/)
+        - 项目文档：[https://stock-open-api.readthedocs.io/zh_CN/latest/](https://stock-open-api.readthedocs.io/zh_CN/latest/stock_open_api.html#module-stock_open_api)
+        - 项目主页：[https://mouday.github.io/stock-open-api/](https://mouday.github.io/stock-open-api/)
         
         ## 安装
         
         ```bash
         pip install stock-open-api
         ```
         
@@ -107,14 +110,23 @@
         | [科创板-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/kcb_stock.get_company_info |
         | [新三板-列表](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list |
         | [新三板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list_iter |
         | [新三板-公司资料+证券资料](http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html) | api/eastmoney/neeq_stock.get_company_info |
         | [A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/company.get_company_info |
         | [深圳A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sz_stock.get_company_info |
         
+        ## 升级记录 
+         
+        [CHANGELOG.md](https://github.com/mouday/stock-open-api/blob/master/CHANGELOG.md)
+        
+        ## 其他相关库
+        
+        - AKShare 开源财经数据接口库 [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)
+        - Tushare 免费提供各类数据 , 助力行业和量化研究。 [https://github.com/waditu/tushare](https://github.com/waditu/tushare)
+        
 Keywords: stock,api
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `stock-open-api-0.0.3/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-0.0.4/stock_open_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,11 +26,12 @@
 stock_open_api/api/eastmoney/us_chinese_stock_config.py
 stock_open_api/api/sse/__init__.py
 stock_open_api/api/sse/sh_stock.py
 stock_open_api/api/sse/sh_stock_config.py
 stock_open_api/items/__init__.py
 stock_open_api/items/list_item.py
 stock_open_api/utils/__init__.py
+stock_open_api/utils/iterator_util.py
 stock_open_api/utils/json_util.py
 stock_open_api/utils/request_util.py
 stock_open_api/utils/time_util.py
 stock_open_api/utils/ua_util.py
```

