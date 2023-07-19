# Comparing `tmp/stock-open-api-0.0.5.tar.gz` & `tmp/stock-open-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.5.tar", last modified: Wed Jul 19 09:45:46 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.6.tar", last modified: Wed Jul 19 09:50:44 2023, max compression
```

## Comparing `stock-open-api-0.0.5.tar` & `stock-open-api-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/api/sse/sh_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/utils/iterator_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 09:45:31.000000 stock-open-api-0.0.5/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:45:45.000000 stock-open-api-0.0.5/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-19 09:45:46.000000 stock-open-api-0.0.5/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:45:45.000000 stock-open-api-0.0.5/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:45:45.000000 stock-open-api-0.0.5/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 09:45:45.000000 stock-open-api-0.0.5/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:45:45.000000 stock-open-api-0.0.5/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.5/PKG-INFO` & `stock-open-api-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-0.0.5/README.md` & `stock-open-api-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/setup.py` & `stock-open-api-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/company.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/company.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/company_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/sz_stock.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/log.py` & `stock-open-api-0.0.6/stock_open_api/log.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/utils/iterator_util.py` & `stock-open-api-0.0.6/stock_open_api/utils/iterator_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api/utils/request_util.py` & `stock-open-api-0.0.6/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.5/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-0.0.6/stock_open_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-0.0.5/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-0.0.6/stock_open_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

