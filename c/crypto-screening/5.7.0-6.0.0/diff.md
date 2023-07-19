# Comparing `tmp/crypto-screening-5.7.0.tar.gz` & `tmp/crypto-screening-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.7.0.tar", last modified: Tue Jul 18 22:08:43 2023, max compression
+gzip compressed data, was "crypto-screening-6.0.0.tar", last modified: Wed Jul 19 00:03:01 2023, max compression
```

## Comparing `crypto-screening-5.7.0.tar` & `crypto-screening-6.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.800255 crypto-screening-5.7.0/
--rw-rw-rw-   0        0        0       98 2023-07-18 22:08:42.000000 crypto-screening-5.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-18 22:08:43.800255 crypto-screening-5.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.7.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.7.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.727247 crypto-screening-5.7.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.754247 crypto-screening-5.7.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.7.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.7.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.767247 crypto-screening-5.7.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.7.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-5.7.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.7.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-5.7.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.773247 crypto-screening-5.7.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24747 2023-07-18 21:10:08.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21735 2023-07-18 21:10:09.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-5.7.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16703 2023-07-18 21:41:58.000000 crypto-screening-5.7.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-5.7.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.7.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.7.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.7.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.775277 crypto-screening-5.7.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-5.7.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.777248 crypto-screening-5.7.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.783247 crypto-screening-5.7.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11429 2023-07-18 22:07:23.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13670 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/container.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.799248 crypto-screening-5.7.0/crypto_screening/market/screeners/database/
--rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/database/__init__.py
--rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/database/data.py
--rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/database/execution.py
--rw-rw-rw-   0        0        0    38366 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19721 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    19217 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    21485 2023-07-18 21:41:58.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    19249 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-5.7.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.7.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-5.7.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-5.7.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.741277 crypto-screening-5.7.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-18 22:08:42.000000 crypto-screening-5.7.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-5.7.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-5.7.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 22:08:43.800255 crypto-screening-5.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-18 22:08:32.000000 crypto-screening-5.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.497197 crypto-screening-6.0.0/
+-rw-rw-rw-   0        0        0       98 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-19 00:03:01.496197 crypto-screening-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-6.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-6.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.462198 crypto-screening-6.0.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.477197 crypto-screening-6.0.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-6.0.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-6.0.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.481197 crypto-screening-6.0.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-6.0.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-6.0.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-6.0.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-6.0.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.483197 crypto-screening-6.0.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24747 2023-07-18 21:10:08.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21735 2023-07-18 21:10:09.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-6.0.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16703 2023-07-18 21:41:58.000000 crypto-screening-6.0.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-6.0.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-6.0.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-6.0.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-6.0.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.485196 crypto-screening-6.0.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-6.0.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.487197 crypto-screening-6.0.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.494197 crypto-screening-6.0.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11429 2023-07-18 22:07:23.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13801 2023-07-18 23:55:50.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/container.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.496197 crypto-screening-6.0.0/crypto_screening/market/screeners/database/
+-rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/database/__init__.py
+-rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/database/data.py
+-rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/database/execution.py
+-rw-rw-rw-   0        0        0    38581 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    20374 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    19870 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    27176 2023-07-18 23:59:47.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    19944 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-6.0.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-6.0.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-6.0.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-6.0.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.474238 crypto-screening-6.0.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-6.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-6.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 00:03:01.497197 crypto-screening-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-19 00:02:57.000000 crypto-screening-6.0.0/setup.py
```

### Comparing `crypto-screening-5.7.0/PKG-INFO` & `crypto-screening-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.7.0
+Version: 6.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.7.0/README.md` & `crypto-screening-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/build.py` & `crypto-screening-6.0.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/assets.py` & `crypto-screening-6.0.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/exchanges.py` & `crypto-screening-6.0.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/orders.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/market/trades.py` & `crypto-screening-6.0.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/screeners.py` & `crypto-screening-6.0.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/collect/symbols.py` & `crypto-screening-6.0.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/dataset.py` & `crypto-screening-6.0.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/interval.py` & `crypto-screening-6.0.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/dynamic.py` & `crypto-screening-6.0.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/foundation/data.py` & `crypto-screening-6.0.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-6.0.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/foundation/state.py` & `crypto-screening-6.0.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-6.0.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/base.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/combined.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 from crypto_screening.market.screeners.orders import (
     orders_market_screener, OrdersScreener,
     OrdersMarketRecorder
 )
 from crypto_screening.market.screeners.database.data import (
     validate_database_engines
 )
-from crypto_screening.market.screeners.recorder import MarketScreener
+from crypto_screening.market.screeners.recorder import (
+    MarketScreener, Callback
+)
 
 __all__ = [
     "CombinedMarketRecorder",
     "CombinedMarketScreener",
     "combined_market_screener",
     "CATEGORIES",
     "RECORDERS",
@@ -293,22 +295,22 @@
     """
 
     recorder: CombinedMarketRecorder
 
     def __init__(
             self,
             markets: Iterable[MarketScreener],
+            recorder: CombinedMarketRecorder,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
-            recorder: Optional[CombinedMarketRecorder] = None
+            amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param markets: The market screeners.
         :param delay: The delay for the process.
@@ -324,17 +326,15 @@
 
         for market in markets:
             screeners.extend(market.screeners)
         # end for
 
         super().__init__(
             location=location, cancel=cancel,
-            delay=delay, recorder=recorder or CombinedMarketRecorder(
-                recorders=[market.recorder for market in markets]
-            ),
+            delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
         self.markets = list(markets)
         self.screeners = list(screeners)
     # end __init__
@@ -411,22 +411,23 @@
     OrdersCategory: orders_market_screener
 }
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
 
 def combined_market_screener(
         data: Dict[str, Iterable[str]],
-        databases: Optional[Databases] = None,
         categories: Optional[Type[CategoryBase]] = None,
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         amount: Optional[int] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
+        databases: Optional[Databases] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrderbookMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> CombinedMarketScreener:
     """
     Creates the market screener object for the data.
@@ -440,34 +441,37 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param databases: The paths to the databases.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
+    :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
     if categories is None:
         categories = CATEGORIES
     # end if
 
     markets = [
         CATEGORY_RECORDER_CONSTRUCTOR_MATCHES[category](
             recorder=recorder, handler=handler, data=data,
             location=location, amount=amount, cancel=cancel,
             delay=delay, limited=limited, refresh=refresh,
-            fixed=fixed, parameters=parameters, databases=databases
+            fixed=fixed, parameters=parameters, databases=databases,
+            callbacks=callbacks
         ) for category in set(categories)
     ]
 
     screener = CombinedMarketScreener(
-        markets=markets, recorder=recorder, handler=handler,
-        location=location, amount=amount, cancel=cancel,
+        markets=markets, recorder=recorder or CombinedMarketRecorder(
+            recorders=[market.recorder for market in markets]
+        ), handler=handler, location=location, amount=amount, cancel=cancel,
         delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
         fixed=fixed, parameters=parameters
     )
```

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/container.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/database/data.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/database/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/database/execution.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/database/execution.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,21 @@
     OHLCV_COLUMNS, VOLUME, BIDS, BIDS_VOLUME,
     load_dataset, save_dataset, OHLC_COLUMNS, create_market_dataframe
 )
 from crypto_screening.validate import validate_interval
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
-    structure_screener_datasets, MarketRecorder, validate_market
+    MarketRecorder, validate_market, Callback
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.orderbook import (
     create_orderbook_dataframe, OrderbookScreener, record_orderbook,
-    OrderbookMarketScreener, create_orderbook_market, OrderbookMarketRecorder
+    OrderbookMarketScreener, create_orderbook_market,
+    OrderbookMarketRecorder
 )
 
 __all__ = [
     "OHLCVMarketScreener",
     "OHLCVMarketRecorder",
     "OHLCVScreener",
     "create_ohlcv_market",
@@ -517,30 +518,33 @@
 
 def record_ohlcv(
         market: Market,
         ohlcv_market: OHLCVMarket,
         indexes: Indexes,
         data: OrderBook,
         timestamp: float,
-        databases: Optional[Dict[str, Engine]] = None
+        databases: Optional[Dict[str, Engine]] = None,
+        callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param ohlcv_market: The OHLCV market structure.
     :param indexes: The indexes of the OHLCV market.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
     :param databases: The database engines.
+    :param callbacks: The callbacks for the service.
+
+    :return: The validation value.
     """
 
     if not record_orderbook(
-        market=market, data=data,
-        timestamp=timestamp, databases=databases
+        market=market, data=data, timestamp=timestamp
     ):
         return False
     # end if
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
@@ -568,28 +572,42 @@
             adjuster = f'{interval_total_minutes}Min'
 
             ohlcv: pd.DataFrame = spread[BIDS].resample(adjuster).ohlc()
             ohlcv.columns = list(OHLC_COLUMNS)
             volume: pd.DataFrame = spread[BIDS_VOLUME].resample(adjuster).ohlc()
             ohlcv[VOLUME] = volume[list(volume.columns)[-1]]
 
+            data = []
+
             for index, row in ohlcv.iterrows():
                 ohlcv_dataset.loc[index] = row
+
+                data.append(row.to_dict())
             # end for
 
             indexes[exchange][symbol][interval] += 1
         # end for
 
         if databases:
             insert_database_record(
                 exchange=exchange, symbol=symbol,
                 name=OHLCVScreener.NAME, interval=interval,
                 dataset=ohlcv_dataset, databases=databases
             )
-    # end if
+        # end if
+
+        for callback in callbacks or []:
+            data = {
+                'data': data,
+                'exchange': exchange,
+                'symbol': symbol
+            }
+
+            callback.record(data, timestamp, name=OHLCVScreener.NAME)
+        # end if
     # end for
 
     return True
 # end record_ohlcv
 
 RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 Databases = Union[Iterable[str], Dict[str, Engine]]
@@ -638,34 +656,36 @@
     INTERVAL = OHLCVScreener.INTERVAL
 
     def __init__(
             self,
             intervals: Optional[Intervals] = None,
             market: Optional[Market] = None,
             ohlcv_market: Optional[OHLCVMarket] = None,
-            databases: Optional[Databases] = None
+            databases: Optional[Databases] = None,
+            callbacks: Optional[Iterable[Callback]] = None,
     ) -> None:
         """
         Defines the class attributes.
 
         :param market: The object to fill with the crypto feed record.
         :param intervals: The intervals for the datasets.
         :param ohlcv_market: The OHLCV market structure.
         :param databases: The paths to the databases.
+        :param callbacks: The callbacks for the service.
         """
 
         data = create_ohlcv_market_recorder_initializers(
             market=market, ohlcv_market=ohlcv_market, intervals=intervals
         )
 
         market = data["market"]
         intervals = data["intervals"]
         ohlcv_market = data["ohlcv_market"]
 
-        super().__init__(market=market, databases=databases)
+        super().__init__(market=market, databases=databases, callbacks=callbacks)
 
         self.intervals = self.validate_intervals(intervals)
         self.ohlcv_market = self.validate_ohlcv_market(ohlcv_market)
 
         self._indexes: Indexes = {}
     # end __init__
 
@@ -773,18 +793,24 @@
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
+        for callback in self.callbacks:
+            if callback.connectable and (not callback.connected):
+                await callback.connect()
+            # end if
+        # end for
+
         return record_ohlcv(
             market=self.market, ohlcv_market=self.ohlcv_market,
             indexes=self._indexes, data=data, timestamp=timestamp,
-            databases=self.databases
+            databases=self.databases, callbacks=self.callbacks
         )
     # end record
 # end MarketOHLCVRecorder
 
 def structure_screener_intervals(
         screeners: Iterable[OHLCVScreener]
 ) -> Dict[str, Dict[str, List[str]]]:
@@ -891,58 +917,42 @@
     recorder: OHLCVMarketRecorder
 
     COLUMNS = OHLCVMarketRecorder.COLUMNS
     INTERVAL = OHLCVMarketRecorder.INTERVAL
 
     def __init__(
             self,
-            intervals: Optional[Intervals] = None,
-            market: Optional[Market] = None,
-            ohlcv_market: Optional[OHLCVMarket] = None,
+            recorder: OHLCVMarketRecorder,
             screeners: Optional[Iterable[Union[OHLCVScreener, OrderbookScreener]]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
-            recorder: Optional[OHLCVMarketRecorder] = None
+            amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
-        :param intervals: The intervals for the datasets.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         :param limited: The value to limit the screeners to active only.
         :param refresh: The refresh time for rerunning.
         :param handler: The handler object for the market data.
         :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
         screeners = screeners or []
 
-        data = create_ohlcv_market_recorder_initializers(
-            market=market or structure_screener_datasets(screeners=screeners),
-            intervals=intervals or structure_screener_intervals(screeners=screeners),
-            ohlcv_market=ohlcv_market
-        )
-
-        market = data["market"]
-        intervals = data["intervals"]
-        ohlcv_market = data["ohlcv_market"]
-
         super().__init__(
             location=location, cancel=cancel,
-            delay=delay, recorder=recorder or OHLCVMarketRecorder(
-                market=market, intervals=intervals, ohlcv_market=ohlcv_market
-            ),
+            delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
         self.screeners[:] = screeners or self.create_ohlcv_screeners()
     # end __init__
 
@@ -1162,21 +1172,22 @@
 # end ohlcv_market_recorder
 
 def ohlcv_market_screener(
         data: Union[Intervals, Dict[str, Iterable[str]]],
         intervals: Optional[Intervals] = None,
         market: Optional[Market] = None,
         ohlcv_market: Optional[OHLCVMarket] = None,
-        databases: Optional[Databases] = None,
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         amount: Optional[int] = None,
+        databases: Optional[Databases] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OHLCVMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OHLCVMarketScreener:
     """
     Creates the market screener object for the data.
@@ -1192,29 +1203,31 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
+    :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
     try:
         intervals = validate_intervals(data)
 
     except ValueError:
         market = create_orderbook_market(data)
     # end try
 
     screener = OHLCVMarketScreener(
         recorder=recorder or OHLCVMarketRecorder(
             market=market, ohlcv_market=ohlcv_market,
-            intervals=intervals, databases=databases
+            intervals=intervals, databases=databases,
+            callbacks=callbacks
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
```

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, save_dataset,
     create_market_dataframe, ORDERBOOK_COLUMNS, load_dataset
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
-    MarketScreener, structure_screener_datasets, MarketRecorder
+    MarketScreener, MarketRecorder, Callback
 )
 
 __all__ = [
     "OrderbookMarketScreener",
     "OrderbookMarketRecorder",
     "OrderbookScreener",
     "create_orderbook_market",
@@ -174,23 +174,27 @@
     # end load_dataset
 # end OrderbookScreener
 
 def record_orderbook(
         market: Market,
         data: OrderBook,
         timestamp: float,
-        databases: Optional[Dict[str, Engine]] = None
+        databases: Optional[Dict[str, Engine]] = None,
+        callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
     :param databases: The database engines.
+    :param callbacks: The callbacks for the service.
+
+    :return: The validation value.
     """
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
         value=adjust_symbol(symbol=data.symbol),
@@ -203,28 +207,40 @@
         setdefault(symbol, create_orderbook_dataframe())
     )
 
     bids = data.book.bids.to_list()
     asks = data.book.asks.to_list()
 
     try:
-        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
+        data = {
             BIDS: float(bids[0][0]),
             ASKS: float(asks[0][0]),
             BIDS_VOLUME: float(bids[0][1]),
             ASKS_VOLUME: float(asks[0][1])
         }
 
+        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = data
+
         if databases:
             insert_database_record(
                 exchange=exchange, symbol=symbol, name=OrderbookScreener.NAME,
                 dataset=dataset, databases=databases
             )
         # end if
 
+        for callback in callbacks or []:
+            data = {
+                'data': [data],
+                'exchange': exchange,
+                'symbol': symbol
+            }
+
+            callback.record(data, timestamp, name=OrderbookScreener.NAME)
+        # end if
+
         return True
 
     except IndexError:
         return False
     # end try
 # end record_orderbook
 
@@ -318,16 +334,22 @@
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
+        for callback in self.callbacks:
+            if callback.connectable and (not callback.connected):
+                await callback.connect()
+            # end if
+        # end for
+
         return record_orderbook(
-            market=self.market, data=data,
+            market=self.market, data=data, callbacks=self.callbacks,
             timestamp=timestamp, databases=self.databases
         )
     # end record
 # end MarketOrderbookRecorder
 
 class OrderbookMarketScreener(MarketScreener):
     """
@@ -377,23 +399,23 @@
     screeners: List[OrderbookScreener]
     recorder: OrderbookMarketRecorder
 
     COLUMNS = OrderbookMarketRecorder.COLUMNS
 
     def __init__(
             self,
+            recorder: OrderbookMarketRecorder,
             screeners: Optional[Iterable[OrderbookScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
-            recorder: Optional[OrderbookMarketRecorder] = None
+            amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
@@ -402,17 +424,15 @@
         :param handler: The handler object for the market data.
         :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
         super().__init__(
             location=location, cancel=cancel,
-            delay=delay, recorder=recorder or OrderbookMarketRecorder(
-                market=structure_screener_datasets(screeners=screeners)
-            ),
+            delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
         self.screeners[:] = screeners or self.create_orderbook_screeners()
     # end __init__
 
@@ -578,21 +598,22 @@
         databases=databases
     )
 # end orderbook_market_recorder
 
 def orderbook_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
-        databases: Optional[Databases] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
+        databases: Optional[Databases] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrderbookMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OrderbookMarketScreener:
     """
     Creates the market screener object for the data.
@@ -606,22 +627,23 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
+    :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
     screener = OrderbookMarketScreener(
         recorder=recorder or OrderbookMarketRecorder(
             market=market or create_orderbook_market(data=data),
-            databases=databases
+            databases=databases, callbacks=callbacks
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
```

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from crypto_screening.dataset import (
     BIDS, ASKS, ORDERS_COLUMNS, create_market_dataframe,
     load_dataset, save_dataset
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
-    MarketScreener, structure_screener_datasets, MarketRecorder
+    MarketScreener, MarketRecorder, Callback
 )
 
 __all__ = [
     "OrdersMarketScreener",
     "OrdersMarketRecorder",
     "OrdersScreener",
     "create_orders_market",
@@ -174,23 +174,27 @@
     # end load_dataset
 # end OrdersScreener
 
 def record_orders(
         market: Market,
         data: Ticker,
         timestamp: float,
-        databases: Optional[Dict[str, Engine]] = None
+        databases: Optional[Dict[str, Engine]] = None,
+        callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
     :param databases: The database engines.
+    :param callbacks: The callbacks for the service.
+
+    :return: The validation value.
     """
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
         value=adjust_symbol(symbol=data.symbol),
@@ -200,26 +204,38 @@
     dataset = (
         market.
         setdefault(exchange, {}).
         setdefault(symbol, create_orders_dataframe())
     )
 
     try:
-        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
+        data = {
             BIDS: float(data.bid),
             ASKS: float(data.ask)
         }
 
+        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = data
+
         if databases:
             insert_database_record(
                 exchange=exchange, symbol=symbol, name=OrdersScreener.NAME,
                 dataset=dataset, databases=databases
             )
         # end if
 
+        for callback in callbacks or []:
+            data = {
+                'data': [data],
+                'exchange': exchange,
+                'symbol': symbol
+            }
+
+            callback.record(data, timestamp, name=OrdersScreener.NAME)
+        # end if
+
         return True
 
     except IndexError:
         return False
     # end try
 # end record_orders
 
@@ -313,17 +329,23 @@
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
+        for callback in self.callbacks:
+            if callback.connectable and (not callback.connected):
+                await callback.connect()
+            # end if
+        # end for
+
         return record_orders(
             market=self.market, data=data, timestamp=timestamp,
-            databases=self.databases
+            databases=self.databases, callbacks=self.callbacks
         )
     # end record
 # end MarketOrdersRecorder
 
 class OrdersMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
@@ -372,23 +394,23 @@
     screeners: List[OrdersScreener]
     recorder: OrdersMarketRecorder
 
     COLUMNS = OrdersMarketRecorder.COLUMNS
 
     def __init__(
             self,
+            recorder: OrdersMarketRecorder,
             screeners: Optional[Iterable[OrdersScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
-            recorder: Optional[OrdersMarketRecorder] = None
+            amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
@@ -397,17 +419,15 @@
         :param handler: The handler object for the market data.
         :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
         super().__init__(
             location=location, cancel=cancel,
-            delay=delay, recorder=recorder or OrdersMarketRecorder(
-                market=structure_screener_datasets(screeners=screeners)
-            ),
+            delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
         self.screeners[:] = screeners or self.create_orders_screeners()
     # end __init__
 
@@ -580,14 +600,15 @@
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         databases: Optional[Databases] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrdersMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OrdersMarketScreener:
     """
     Creates the market screener object for the data.
@@ -601,22 +622,23 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
+    :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
     screener = OrdersMarketScreener(
         recorder=recorder or OrdersMarketRecorder(
             market=market or create_orders_market(data=data),
-            databases=databases
+            databases=databases, callbacks=callbacks
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
```

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/recorder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # recorder.py
 
 import warnings
+import json
 import threading
 import time
 import datetime as dt
 from typing import (
     Optional, Dict, Any, List,
     Iterable, Type, Union
 )
 from functools import partial
 import asyncio
+from textwrap import wrap
 
 import pandas as pd
 
 from sqlalchemy import Engine
 
 from represent import Modifiers, represent
 
-
 from cryptofeed import FeedHandler
 from cryptofeed.feed import Feed
+from cryptofeed.backends.socket import UDPProtocol
 
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.database.data import validate_database_engines
 from crypto_screening.market.screeners.base import BaseMarketScreener, BaseScreener
@@ -33,15 +35,17 @@
     "ExchangeFeed",
     "FEED_GROUP_SIZE",
     "add_feeds",
     "MarketScreener",
     "structure_screeners_datasets",
     "structure_screener_datasets",
     "MarketRecorder",
-    "validate_market"
+    "validate_market",
+    "Callback",
+    "SocketCallback"
 ]
 
 class MarketHandler(FeedHandler):
     """A class to handle the market data feed."""
 
     def __init__(self) -> None:
         """Defines the class attributes."""
@@ -124,27 +128,25 @@
         packets = []
 
         for i in range(0, int(len(symbols) / amount) + len(symbols) % amount, amount):
             packets.append(symbols[i:])
         # end for
 
         for symbols_packet in packets:
-            feed = EXCHANGES[exchange](
-                symbols=symbols_packet,
-                **(
-                    parameters[exchange]
-                    if (
-                        (exchange in parameters) and
-                        isinstance(parameters[exchange], dict) and
-                        all(isinstance(key, str) for key in parameters)
-
-                    ) else {}
-                )
+            exchange_parameters = (
+                parameters[exchange]
+                if (
+                    (exchange in parameters) and
+                    isinstance(parameters[exchange], dict) and
+                    all(isinstance(key, str) for key in parameters)
+                ) else {}
             )
 
+            feed = EXCHANGES[exchange](symbols=symbols_packet, **exchange_parameters)
+
             feed.start = partial(ExchangeFeed.start, feed)
             feed.stop = partial(ExchangeFeed.stop, feed)
             feed.handler = handler
             feed.running = False
 
             handler.add_feed(feed)
         # end for
@@ -189,14 +191,215 @@
     # end try
 
     return data
 # end validate_market
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
 
+class Callback:
+    """A class to represent a callback."""
+
+    NAME: str = None
+    CONNECTABLE: bool = False
+    ADJUSTABLE: bool = True
+
+    def __init__(self, name: Optional[Any] = None) -> None:
+        """
+        Defines the class attributes.
+
+        :param name: The key od the data.
+        """
+
+        self.name = name if name else self.NAME
+    # end __init__
+
+    def record(self, data: Any, timestamp: float, name: Optional[Any] = None) -> bool:
+        """
+        Records the data from the crypto feed into the dataset.
+
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
+        :param name: The key for the data type.
+
+        :return: The validation value.
+        """
+    # end record
+
+    @property
+    def connectable(self) -> bool:
+        """
+        Checks if the connection was created.
+
+        :return: The existence of a connection.
+        """
+
+        return self.CONNECTABLE
+    # end connectable
+
+    @property
+    def adjustable(self) -> bool:
+        """
+        Checks if the connection was created.
+
+        :return: The existence of a connection.
+        """
+
+        return self.ADJUSTABLE
+    # end adjustable
+
+    async def connect(self) -> None:
+        """Connects to the socket service."""
+    # end connect
+# end Callback
+
+class SocketCallback(Callback):
+    """A class to represent a socket callback."""
+
+    BUFFER = 1024
+
+    PROTOCOLS = ('tcp://', 'udp://')
+
+    CONNECTABLE = True
+
+    def __init__(
+            self,
+            address: str,
+            port: int,
+            name: Optional[Any] = None,
+            buffer: Optional[int] = None
+    ) -> None:
+        """
+        Defines the class attributes.
+
+        :param address: The address of the socket.
+        :param port: The port of the socket.
+        :param name: The key od the data.
+        :param buffer: The buffer size.
+        """
+
+        super().__init__(name=name)
+
+        buffer = buffer or self.BUFFER
+
+        protocol = address[:6]
+
+        if protocol not in self.PROTOCOLS:
+            raise ValueError(
+                f"Invalid protocol: {protocol}. "
+                f"Protocol must be one of: {', '.join(self.PROTOCOLS)}"
+            )
+        # end if
+
+        self.connection = None
+        self.protocol = protocol
+        self.address = address[6:]
+        self.port = port
+        self.buffer = buffer
+
+        self.running = False
+    # end __init__
+
+    @property
+    def connected(self) -> bool:
+        """
+        Checks if the connection was created.
+
+        :return: The existence of a connection.
+        """
+
+        return self.connection is not None
+    # end connected
+
+    # noinspection PyTypeChecker
+    async def connect(self) -> None:
+        """Connects to the socket service."""
+
+        if self.connection is not None:
+            warnings.warn(f"{repr(self)} callback is already connected.")
+
+            return
+        # end if
+
+        try:
+            if self.protocol == 'udp://':
+                loop = asyncio.get_event_loop()
+                self.connection, self.protocol = (
+                    await loop.create_datagram_endpoint(
+                        lambda: UDPProtocol(loop),
+                        remote_addr=(self.address, self.port)
+                    )
+                )
+
+            elif self.protocol == 'tcp://':
+                _, self.connection = await asyncio.open_connection(
+                    host=self.address, port=self.port
+                )
+            # end if
+
+            self.running = True
+
+        except Exception as e:
+            if self.adjustable:
+                warnings.warn(f"{type(e)}: {str(e)}")
+
+            else:
+                raise e
+            # end if
+        # end try
+    # end connect
+
+    def record(self, data: Any, timestamp: float, name: Optional[Any] = None) -> bool:
+        """
+        Records the data from the crypto feed into the dataset.
+
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
+        :param name: The key for the data type.
+
+        :return: The validation value.
+        """
+
+        if not (self.running and self.connected):
+            return False
+        # end if
+
+        data = json.dumps({'name': self.name or name, 'data': data})
+
+        if self.protocol == 'udp://':
+            if len(data) > self.buffer:
+                chunks = wrap(data, self.buffer)
+
+                for chunk in chunks:
+                    message = json.dumps(
+                        {
+                            'type': 'chunked',
+                            'chunks': len(chunks),
+                            'data': chunk,
+                            'timestamp': float(timestamp)
+                        }
+                    ).encode()
+
+                    self.connection.sendto(message)
+                # end for
+
+                return True
+            # end if
+        # end if
+
+        self.connection.write(
+            json.dumps(
+                {'data': data, 'timestamp': float(timestamp)}
+            ).encode()
+        )
+
+        return True
+    # end writer
+# end SocketCallback
+
+Callbacks = Iterable[Callback]
 
 @represent
 class MarketRecorder:
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
@@ -219,27 +422,34 @@
     >>> recorder = MarketRecorder(data=market)
 
     """
 
     __modifiers__ = Modifiers()
     __modifiers__.hidden.append("market")
 
-    __slots__ = "market", "databases"
+    __slots__ = "market", "databases", 'callbacks'
 
-    def __init__(self, market: Market, databases: Optional[Databases] = None) -> None:
+    def __init__(
+            self,
+            market: Market,
+            databases: Optional[Databases] = None,
+            callbacks: Optional[Callbacks] = None
+    ) -> None:
         """
         Defines the class attributes.
 
         :param market: The object to fill with the crypto feed record.
         :param databases: The paths to the databases.
+        :param callbacks: The callbacks for the service.
         """
 
         self.market = self.validate_market(data=market)
+        self.databases = self.validate_database_engines(data=databases)
 
-        self.databases = self.validate_database_engines(databases)
+        self.callbacks = callbacks or []
     # end __init__
 
     @staticmethod
     def validate_market(data: Any) -> Market:
         """
         Validates the data.
 
@@ -410,23 +620,23 @@
     DELAY = 1
     AMOUNT = FEED_GROUP_SIZE
 
     REFRESH = dt.timedelta(minutes=5)
 
     def __init__(
             self,
+            recorder: Union[MarketRecorder, Any],
             screeners: Optional[Iterable[BaseScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
-            recorder: Optional[MarketRecorder] = None
+            amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
```

### Comparing `crypto-screening-5.7.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-6.0.0/crypto_screening/market/screeners/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from crypto_screening.dataset import (
     TRADES_COLUMNS, create_market_dataframe,
     AMOUNT, PRICE, SIDE, load_dataset, save_dataset
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
-    MarketScreener, structure_screener_datasets, MarketRecorder
+    MarketScreener, MarketRecorder, Callback
 )
 
 __all__ = [
     "TradesMarketScreener",
     "TradesMarketRecorder",
     "TradesScreener",
     "create_trades_market",
@@ -174,23 +174,27 @@
     # end load_dataset
 # end TradesScreener
 
 def record_trades(
         market: Market,
         data: Trade,
         timestamp: float,
-        databases: Optional[Dict[str, Engine]] = None
+        databases: Optional[Dict[str, Engine]] = None,
+        callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
     :param databases: The database engines.
+    :param callbacks: The callbacks for the service.
+
+    :return: The validation value.
     """
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
         value=adjust_symbol(symbol=data.symbol),
@@ -200,27 +204,39 @@
     dataset = (
         market.
         setdefault(exchange, {}).
         setdefault(symbol, create_trades_dataframe())
     )
 
     try:
-        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
+        data = {
             AMOUNT: float(data.amount),
             PRICE: float(data.price),
             SIDE: data.side
         }
 
+        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = data
+
         if databases:
             insert_database_record(
                 exchange=exchange, symbol=symbol, name=TradesScreener.NAME,
                 dataset=dataset, databases=databases
             )
         # end if
 
+        for callback in callbacks or []:
+            data = {
+                'data': [data],
+                'exchange': exchange,
+                'symbol': symbol
+            }
+
+            callback.record(data, timestamp, name=TradesScreener.NAME)
+        # end if
+
         return True
 
     except IndexError:
         return False
     # end try
 # end record_trades
 
@@ -312,19 +328,27 @@
 
     async def record(self, data: Trade, timestamp: float) -> bool:
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
+
+        :return: The validation value.
         """
 
+        for callback in self.callbacks:
+            if callback.connectable and (not callback.connected):
+                await callback.connect()
+            # end if
+        # end for
+
         return record_trades(
             market=self.market, data=data, timestamp=timestamp,
-            databases=self.databases
+            databases=self.databases, callbacks=self.callbacks
         )
     # end record
 # end TradesRecorder
 
 class TradesMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
@@ -373,23 +397,23 @@
     screeners: List[TradesScreener]
     recorder: TradesMarketRecorder
 
     COLUMNS = TradesMarketRecorder.COLUMNS
 
     def __init__(
             self,
+            recorder: TradesMarketRecorder,
             screeners: Optional[Iterable[TradesScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
-            recorder: Optional[TradesMarketRecorder] = None
+            amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
@@ -398,17 +422,15 @@
         :param handler: The handler object for the market data.
         :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
         super().__init__(
             location=location, cancel=cancel,
-            delay=delay, recorder=recorder or TradesMarketRecorder(
-                market=structure_screener_datasets(screeners=screeners)
-            ),
+            delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
         self.screeners[:] = screeners or self.create_trades_screeners()
     # end __init__
 
@@ -581,14 +603,15 @@
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         databases: Optional[Databases] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[TradesMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> TradesMarketScreener:
     """
     Creates the market screener object for the data.
@@ -602,22 +625,23 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
+    :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
     screener = TradesMarketScreener(
         recorder=recorder or TradesMarketRecorder(
             market=market or create_trades_market(data=data),
-            databases=databases
+            databases=databases, callbacks=callbacks
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
```

### Comparing `crypto-screening-5.7.0/crypto_screening/market/waiting.py` & `crypto-screening-6.0.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/process.py` & `crypto-screening-6.0.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/symbols.py` & `crypto-screening-6.0.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening/validate.py` & `crypto-screening-6.0.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-6.0.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.7.0
+Version: 6.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.7.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-6.0.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.7.0/pyproject.toml` & `crypto-screening-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.7.0'
+version = '6.0.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.7.0/setup.py` & `crypto-screening-6.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.7.0',
+        version='6.0.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

