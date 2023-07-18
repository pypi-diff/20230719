# Comparing `tmp/crypto-screening-5.5.0.tar.gz` & `tmp/crypto-screening-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.5.0.tar", last modified: Mon Jul 17 10:00:42 2023, max compression
+gzip compressed data, was "crypto-screening-5.6.0.tar", last modified: Tue Jul 18 09:15:46 2023, max compression
```

## Comparing `crypto-screening-5.5.0.tar` & `crypto-screening-5.6.0.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:42.000748 crypto-screening-5.5.0/
--rw-rw-rw-   0        0        0       98 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-17 10:00:42.000209 crypto-screening-5.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.5.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.5.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.965625 crypto-screening-5.5.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.982982 crypto-screening-5.5.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.5.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.5.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.986614 crypto-screening-5.5.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.5.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19456 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12436 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.988088 crypto-screening-5.5.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24779 2023-07-17 09:51:27.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    14887 2023-07-17 10:00:22.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21766 2023-07-17 09:50:45.000000 crypto-screening-5.5.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    14999 2023-07-17 09:43:58.000000 crypto-screening-5.5.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16697 2023-07-17 09:46:37.000000 crypto-screening-5.5.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.5.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.5.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.5.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.5.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.990612 crypto-screening-5.5.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.5.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.993126 crypto-screening-5.5.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.5.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.998670 crypto-screening-5.5.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-16 14:17:05.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36682 2023-07-16 13:04:17.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-16 14:16:54.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18061 2023-07-16 14:05:40.000000 crypto-screening-5.5.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.5.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.5.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.5.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4233 2023-07-17 08:56:51.000000 crypto-screening-5.5.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:00:41.980462 crypto-screening-5.5.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1673 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-17 10:00:41.000000 crypto-screening-5.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 10:00:42.000748 crypto-screening-5.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-17 10:00:39.000000 crypto-screening-5.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.030021 crypto-screening-5.6.0/
+-rw-rw-rw-   0        0        0       98 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-18 09:15:46.030021 crypto-screening-5.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.6.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.6.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:45.997510 crypto-screening-5.6.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.009510 crypto-screening-5.6.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.6.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.6.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.013513 crypto-screening-5.6.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.6.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19456 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12436 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.016514 crypto-screening-5.6.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24779 2023-07-17 09:51:27.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    14887 2023-07-17 10:00:22.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21766 2023-07-17 09:50:45.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    14999 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16697 2023-07-17 09:46:37.000000 crypto-screening-5.6.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.6.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.6.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.6.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.6.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.018513 crypto-screening-5.6.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.6.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.020513 crypto-screening-5.6.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.027017 crypto-screening-5.6.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10987 2023-07-17 21:45:06.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13753 2023-07-18 09:13:48.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/container.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.029021 crypto-screening-5.6.0/crypto_screening/market/screeners/database/
+-rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/database/__init__.py
+-rw-rw-rw-   0        0        0     8835 2023-07-18 09:10:50.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/database/data.py
+-rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/database/execution.py
+-rw-rw-rw-   0        0        0    37739 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    19397 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18899 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    21401 2023-07-18 09:10:57.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18931 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.6.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.6.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.6.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4233 2023-07-17 08:56:51.000000 crypto-screening-5.6.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.006510 crypto-screening-5.6.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-18 08:49:04.000000 crypto-screening-5.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-5.6.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-5.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 09:15:46.030021 crypto-screening-5.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-18 08:48:48.000000 crypto-screening-5.6.0/setup.py
```

### Comparing `crypto-screening-5.5.0/PKG-INFO` & `crypto-screening-5.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.5.0
+Version: 5.6.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.5.0/README.md` & `crypto-screening-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/build.py` & `crypto-screening-5.6.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/assets.py` & `crypto-screening-5.6.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/exchanges.py` & `crypto-screening-5.6.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/orders.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/market/trades.py` & `crypto-screening-5.6.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/screeners.py` & `crypto-screening-5.6.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/collect/symbols.py` & `crypto-screening-5.6.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/dataset.py` & `crypto-screening-5.6.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/interval.py` & `crypto-screening-5.6.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/dynamic.py` & `crypto-screening-5.6.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/foundation/data.py` & `crypto-screening-5.6.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.6.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/foundation/state.py` & `crypto-screening-5.6.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.6.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/base.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("market")
 
     MINIMUM_DELAY = 1
 
+    NAME = "BASE"
+
     __slots__ = "symbol", "exchange", "market"
 
     def __init__(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/combined.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import (
     Dict, Optional, Iterable, Any,
     Union, List, Callable, Type
 )
 
 import pandas as pd
 
+from sqlalchemy import Engine
+
 from cryptofeed import FeedHandler
 
 from crypto_screening.market.screeners.orderbook import (
     orderbook_market_screener, OrderbookScreener,
     OrderbookMarketRecorder
 )
 from crypto_screening.market.screeners.ohlcv import (
@@ -22,14 +24,17 @@
     trades_market_screener, TradesScreener,
     TradesMarketRecorder
 )
 from crypto_screening.market.screeners.orders import (
     orders_market_screener, OrdersScreener,
     OrdersMarketRecorder
 )
+from crypto_screening.market.screeners.database.data import (
+    validate_database_engines
+)
 from crypto_screening.market.screeners.recorder import MarketScreener
 
 __all__ = [
     "CombinedMarketRecorder",
     "CombinedMarketScreener",
     "combined_market_screener",
     "CATEGORIES",
@@ -158,16 +163,49 @@
 
         for recorder in recorders:
             structure.update(recorder.structure())
         # end for
 
         self.recorders = list(recorders)
         self._structure = structure
+
+        self.databases = {}
+
+        for recorder in self.recorders:
+            self.databases.update(recorder.databases)
+        # end for
     # end __init__
 
+    @staticmethod
+    def validate_database_engines(data: Any) -> Dict[str, Engine]:
+        """
+        Validates the data.
+
+        :param data: The data to validate.
+
+        :return: The valid data.
+        """
+
+        return validate_database_engines(data)
+    # end validate_market
+
+    def generate_databases(self) -> Dict[str, Engine]:
+        """
+        Generates the list of databases.
+
+        :return: The database paths.
+        """
+
+        for recorder in self.recorders:
+            self.databases.update(recorder.generate_databases())
+        # end for
+
+        return self.databases
+    # end generate_databases
+
     def structure(self) -> Dict[str, List[str]]:
         """
         Returns the structure of the market data.
 
         :return: The structure of the market.
         """
 
@@ -362,16 +400,19 @@
 CATEGORY_RECORDER_CONSTRUCTOR_MATCHES = {
     OrderbookCategory: orderbook_market_screener,
     OHLCVCategory: ohlcv_market_screener,
     TradesCategory: trades_market_screener,
     OrdersCategory: orders_market_screener
 }
 
+Databases = Union[Iterable[str], Dict[str, Engine]]
+
 def combined_market_screener(
         data: Dict[str, Iterable[str]],
+        databases: Optional[Databases] = None,
         categories: Optional[Type[CategoryBase]] = None,
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         amount: Optional[int] = None,
@@ -389,14 +430,15 @@
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
     :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param separator: The separator of the assets.
+    :param databases: The paths to the databases.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
 
     :return: The market screener object.
     """
@@ -406,17 +448,17 @@
     # end if
 
     markets = [
         CATEGORY_RECORDER_CONSTRUCTOR_MATCHES[category](
             recorder=recorder, handler=handler, data=data,
             location=location, amount=amount, cancel=cancel,
             delay=delay, limited=limited, refresh=refresh,
-            fixed=fixed, separator=separator, parameters=parameters
-        )
-        for category in set(categories)
+            fixed=fixed, separator=separator, parameters=parameters,
+            databases=databases
+        ) for category in set(categories)
     ]
 
     screener = CombinedMarketScreener(
         markets=markets, recorder=recorder, handler=handler,
         location=location, amount=amount, cancel=cancel,
         delay=delay, limited=limited, refresh=refresh
     )
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/container.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
+from sqlalchemy import Engine
+
 from represent import Modifiers
 
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.process import find_string_value
@@ -21,14 +23,15 @@
 )
 from crypto_screening.validate import validate_interval
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
     structure_screener_datasets, MarketRecorder, validate_market
 )
+from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.orderbook import (
     create_orderbook_dataframe, OrderbookScreener, record_orderbook,
     OrderbookMarketScreener, create_orderbook_market, OrderbookMarketRecorder
 )
 
 __all__ = [
     "OHLCVMarketScreener",
@@ -118,14 +121,15 @@
         The dataset of the market data as OHLCV.
 
     - base_market:
         The dataset of the market data as BID/ASK spread.
     """
 
     INTERVAL = "1m"
+    NAME = "OHLCV"
 
     def __init__(
             self,
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
             location: Optional[str] = None,
@@ -188,15 +192,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-ORDERBOOK.csv")
+            replace(".csv", f"-{OrderbookScreener.NAME}.csv")
         )
     # end orderbook_dataset_path
 
     def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -218,15 +222,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-OHLCV-{self.interval}.csv")
+            replace(".csv", f"-{self.NAME}-{self.interval}.csv")
         )
     # end ohlcv_dataset_path
 
     def save_ohlcv_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -512,27 +516,32 @@
 # end create_ohlcv_market_recorder_initializers
 
 def record_ohlcv(
         market: Market,
         ohlcv_market: OHLCVMarket,
         indexes: Indexes,
         data: OrderBook,
-        timestamp: float
+        timestamp: float,
+        databases: Optional[Dict[str, Engine]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param ohlcv_market: The OHLCV market structure.
     :param indexes: The indexes of the OHLCV market.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
+    :param databases: The database engines.
     """
 
-    if not record_orderbook(market=market, data=data, timestamp=timestamp):
+    if not record_orderbook(
+        market=market, data=data,
+        timestamp=timestamp, databases=databases
+    ):
         return False
     # end if
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
@@ -565,20 +574,29 @@
 
             for index, row in ohlcv.iterrows():
                 ohlcv_dataset.loc[index] = row
             # end for
 
             indexes[exchange][symbol][interval] += 1
         # end for
+
+        if databases:
+            insert_database_record(
+                exchange=exchange, symbol=symbol,
+                name=OHLCVScreener.NAME, interval=interval,
+                dataset=ohlcv_dataset, databases=databases
+            )
+    # end if
     # end for
 
     return True
 # end record_ohlcv
 
 RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
+Databases = Union[Iterable[str], Dict[str, Engine]]
 
 class OHLCVMarketRecorder(OrderbookMarketRecorder):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
@@ -609,33 +627,35 @@
     COLUMNS = OHLCV_COLUMNS
     INTERVAL = OHLCVScreener.INTERVAL
 
     def __init__(
             self,
             intervals: Optional[Intervals] = None,
             market: Optional[Market] = None,
-            ohlcv_market: Optional[OHLCVMarket] = None
+            ohlcv_market: Optional[OHLCVMarket] = None,
+            databases: Optional[Databases] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param market: The object to fill with the crypto feed record.
         :param intervals: The intervals for the datasets.
         :param ohlcv_market: The OHLCV market structure.
+        :param databases: The paths to the databases.
         """
 
         data = create_ohlcv_market_recorder_initializers(
             market=market, ohlcv_market=ohlcv_market, intervals=intervals
         )
 
         market = data["market"]
         intervals = data["intervals"]
         ohlcv_market = data["ohlcv_market"]
 
-        super().__init__(market=market)
+        super().__init__(market=market, databases=databases)
 
         self.intervals = self.validate_intervals(intervals)
         self.ohlcv_market = self.validate_ohlcv_market(ohlcv_market)
 
         self._indexes: Indexes = {}
     # end __init__
 
@@ -745,15 +765,16 @@
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
         return record_ohlcv(
             market=self.market, ohlcv_market=self.ohlcv_market,
-            indexes=self._indexes, data=data, timestamp=timestamp
+            indexes=self._indexes, data=data, timestamp=timestamp,
+            databases=self.databases
         )
     # end record
 # end MarketOHLCVRecorder
 
 def structure_screener_intervals(
         screeners: Iterable[OHLCVScreener]
 ) -> Dict[str, Dict[str, List[str]]]:
@@ -1085,21 +1106,23 @@
 
         return screeners
     # end create_ohlcv_screeners
 # end MarketOHLCVRecorder
 
 def ohlcv_market_recorder(
         data: Union[Intervals, Dict[str, Iterable[str]]],
-        interval: Optional[str] = None
+        interval: Optional[str] = None,
+        databases: Optional[Databases] = None
 ) -> OHLCVMarketRecorder:
     """
     Creates the market recorder object for the data.
 
     :param data: The market data.
     :param interval: The interval for the structure.
+    :param databases: The paths to the databases.
 
     :return: The market recorder object.
     """
 
     try:
         intervals = validate_ohlcv_market(data)
 
@@ -1107,22 +1130,25 @@
         validate_market(data)
 
         intervals = datasets_to_intervals_datasets(
             data=data, interval=interval
         )
     # end try
 
-    return OHLCVMarketRecorder(intervals=intervals, market=data)
+    return OHLCVMarketRecorder(
+        intervals=intervals, market=data, databases=databases
+    )
 # end ohlcv_market_recorder
 
 def ohlcv_market_screener(
         data: Union[Intervals, Dict[str, Iterable[str]]],
         intervals: Optional[Intervals] = None,
         market: Optional[Market] = None,
         ohlcv_market: Optional[OHLCVMarket] = None,
+        databases: Optional[Databases] = None,
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         amount: Optional[int] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
@@ -1145,28 +1171,30 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
+    :param databases: The paths to the databases.
 
     :return: The market screener object.
     """
 
     try:
         intervals = validate_intervals(data)
 
     except ValueError:
         market = create_orderbook_market(data)
     # end try
 
     screener = OHLCVMarketScreener(
         recorder=recorder or OHLCVMarketRecorder(
-            market=market, ohlcv_market=ohlcv_market, intervals=intervals
+            market=market, ohlcv_market=ohlcv_market,
+            intervals=intervals, databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(), fixed=fixed,
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
+from sqlalchemy import Engine
+
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, save_dataset,
     create_market_dataframe, ORDERBOOK_COLUMNS, load_dataset
 )
+from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
     MarketScreener, structure_screener_datasets, MarketRecorder
 )
 
 __all__ = [
     "OrderbookMarketScreener",
@@ -89,14 +92,16 @@
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data as BID/ASK spread.
     """
 
+    NAME = "ORDERBOOK"
+
     @property
     def orderbook_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
@@ -111,15 +116,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-ORDERBOOK.csv")
+            replace(".csv", f"-{self.NAME}.csv")
         )
     # end orderbook_dataset_path
 
     def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -165,21 +170,27 @@
         :param location: The saving location of the dataset.
         """
 
         self.load_orderbook_dataset(location=location)
     # end load_dataset
 # end OrderbookScreener
 
-def record_orderbook(market: Market, data: OrderBook, timestamp: float) -> bool:
+def record_orderbook(
+        market: Market,
+        data: OrderBook,
+        timestamp: float,
+        databases: Optional[Dict[str, Engine]] = None
+) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
+    :param databases: The database engines.
     """
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
         value=adjust_symbol(symbol=data.symbol),
@@ -199,14 +210,21 @@
         dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
             BIDS: float(bids[0][0]),
             ASKS: float(asks[0][0]),
             BIDS_VOLUME: float(bids[0][1]),
             ASKS_VOLUME: float(asks[0][1])
         }
 
+        if databases:
+            insert_database_record(
+                exchange=exchange, symbol=symbol, name=OrderbookScreener.NAME,
+                dataset=dataset, databases=databases
+            )
+        # end if
+
         return True
 
     except IndexError:
         return False
     # end try
 # end record_orderbook
 
@@ -298,15 +316,16 @@
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
         return record_orderbook(
-            market=self.market, data=data, timestamp=timestamp
+            market=self.market, data=data,
+            timestamp=timestamp, databases=self.databases
         )
     # end record
 # end MarketOrderbookRecorder
 
 class OrderbookMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
@@ -520,31 +539,39 @@
             # end for
         # end for
 
         return screeners
     # end create_orderbook_screeners
 # end MarketOrderbookScreener
 
-def orderbook_market_recorder(data: Dict[str, Iterable[str]]) -> OrderbookMarketRecorder:
+Databases = Union[Iterable[str], Dict[str, Engine]]
+
+def orderbook_market_recorder(
+        data: Dict[str, Iterable[str]],
+        databases: Optional[Databases] = None
+) -> OrderbookMarketRecorder:
     """
     Creates the market recorder object for the data.
 
     :param data: The market data.
+    :param databases: The paths to the databases.
 
     :return: The market recorder object.
     """
 
     return OrderbookMarketRecorder(
-        market=create_orderbook_market(data=data)
+        market=create_orderbook_market(data=data),
+        databases=databases
     )
 # end orderbook_market_recorder
 
 def orderbook_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
+        databases: Optional[Databases] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
@@ -565,21 +592,23 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
+    :param databases: The paths to the databases.
 
     :return: The market screener object.
     """
 
     screener = OrderbookMarketScreener(
         recorder=recorder or OrderbookMarketRecorder(
-            market=market or create_orderbook_market(data=data)
+            market=market or create_orderbook_market(data=data),
+            databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(), fixed=fixed,
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
+from sqlalchemy import Engine
+
 from cryptofeed import FeedHandler
 from cryptofeed.types import Ticker
 from cryptofeed.defines import TICKER
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     BIDS, ASKS, ORDERS_COLUMNS, create_market_dataframe,
     load_dataset, save_dataset
 )
+from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
     MarketScreener, structure_screener_datasets, MarketRecorder
 )
 
 __all__ = [
     "OrdersMarketScreener",
@@ -89,14 +92,16 @@
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data as orders.
     """
 
+    NAME = "ORDERS"
+
     @property
     def orders_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
@@ -111,15 +116,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-ORDERS.csv")
+            replace(".csv", f"-{self.NAME}.csv")
         )
     # end orders_dataset_path
 
     def save_orders_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -165,21 +170,27 @@
         :param location: The saving location of the dataset.
         """
 
         self.load_orders_dataset(location=location)
     # end load_dataset
 # end OrdersScreener
 
-def record_orders(market: Market, data: Ticker, timestamp: float) -> bool:
+def record_orders(
+        market: Market,
+        data: Ticker,
+        timestamp: float,
+        databases: Optional[Dict[str, Engine]] = None
+) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
+    :param databases: The database engines.
     """
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
         value=adjust_symbol(symbol=data.symbol),
@@ -194,14 +205,21 @@
 
     try:
         dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
             BIDS: float(data.bid),
             ASKS: float(data.ask)
         }
 
+        if databases:
+            insert_database_record(
+                exchange=exchange, symbol=symbol, name=OrdersScreener.NAME,
+                dataset=dataset, databases=databases
+            )
+        # end if
+
         return True
 
     except IndexError:
         return False
     # end try
 # end record_orders
 
@@ -293,15 +311,16 @@
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
         return record_orders(
-            market=self.market, data=data, timestamp=timestamp
+            market=self.market, data=data, timestamp=timestamp,
+            databases=self.databases
         )
     # end record
 # end MarketOrdersRecorder
 
 class OrdersMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
@@ -515,37 +534,45 @@
             # end for
         # end for
 
         return screeners
     # end create_orders_screeners
 # end MarketOrderbookScreener
 
-def orders_market_recorder(data: Dict[str, Iterable[str]]) -> OrdersMarketRecorder:
+Databases = Union[Iterable[str], Dict[str, Engine]]
+
+def orders_market_recorder(
+        data: Dict[str, Iterable[str]],
+        databases: Optional[Databases] = None
+) -> OrdersMarketRecorder:
     """
     Creates the market recorder object for the data.
 
     :param data: The market data.
+    :param databases: The paths to the databases.
 
     :return: The market recorder object.
     """
 
     return OrdersMarketRecorder(
-        market=create_orders_market(data=data)
+        market=create_orders_market(data=data),
+        databases=databases
     )
 # end orders_market_recorder
 
 def orders_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
+        databases: Optional[Databases] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrdersMarketRecorder] = None,
         fixed: Optional[bool] = True,
         separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OrdersMarketScreener:
     """
@@ -560,21 +587,23 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
+    :param databases: The paths to the databases.
 
     :return: The market screener object.
     """
 
     screener = OrdersMarketScreener(
         recorder=recorder or OrdersMarketRecorder(
-            market=market or create_orders_market(data=data)
+            market=market or create_orders_market(data=data),
+            databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(), fixed=fixed,
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # recorder.py
 
 import warnings
 import threading
 import time
 import datetime as dt
 from typing import (
-    Optional, Dict, Any, List, Iterable, Type, Union
+    Optional, Dict, Any, List,
+    Iterable, Type, Union
 )
 from functools import partial
 import asyncio
 
 import pandas as pd
 
+from sqlalchemy import Engine
+
 from represent import Modifiers, represent
 
+
 from cryptofeed import FeedHandler
 from cryptofeed.feed import Feed
 
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import Separator
-from crypto_screening.market.screeners.base import (
-    BaseMultiScreener, BaseScreener
-)
+from crypto_screening.market.screeners.database.data import validate_database_engines
+from crypto_screening.market.screeners.base import BaseMultiScreener, BaseScreener
 
 __all__ = [
     "MarketHandler",
     "ExchangeFeed",
     "FEED_GROUP_SIZE",
     "add_feeds",
     "MarketScreener",
@@ -193,14 +196,17 @@
             f"Data must be of type {Market}, not: {data}."
         )
     # end try
 
     return data
 # end validate_market
 
+Databases = Union[Iterable[str], Dict[str, Engine]]
+
+
 @represent
 class MarketRecorder:
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
@@ -219,24 +225,27 @@
     >>> recorder = MarketRecorder(data=market)
 
     """
 
     __modifiers__ = Modifiers()
     __modifiers__.hidden.append("market")
 
-    __slots__ = "market",
+    __slots__ = "market", "databases"
 
-    def __init__(self, market: Market) -> None:
+    def __init__(self, market: Market, databases: Optional[Databases] = None) -> None:
         """
         Defines the class attributes.
 
         :param market: The object to fill with the crypto feed record.
+        :param databases: The paths to the databases.
         """
 
         self.market = self.validate_market(data=market)
+
+        self.databases = self.validate_database_engines(databases)
     # end __init__
 
     @staticmethod
     def validate_market(data: Any) -> Market:
         """
         Validates the data.
 
@@ -244,14 +253,46 @@
 
         :return: The valid data.
         """
 
         return validate_market(data=data)
     # end validate_market
 
+    @staticmethod
+    def validate_database_engines(data: Any) -> Dict[str, Engine]:
+        """
+        Validates the data.
+
+        :param data: The data to validate.
+
+        :return: The valid data.
+        """
+
+        return validate_database_engines(data)
+    # end validate_market
+
+    def generate_databases(self) -> Dict[str, Engine]:
+        """
+        Generates the list of databases.
+
+        :return: The database paths.
+        """
+
+        self.databases.update(
+            self.validate_database_engines(
+                [
+                    f'sqlite:///databases/{exchange}.sqlite'
+                    for exchange in self.structure()
+                ]
+            )
+        )
+
+        return self.databases
+    # end generate_databases
+
     def parameters(self) -> Dict[str, Any]:
         """
         Returns the order book parameters.
 
         :return: The order book parameters.
         """
 
@@ -346,17 +387,15 @@
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
     """
 
     __modifiers__ = Modifiers(**BaseMultiScreener.__modifiers__)
-    __modifiers__.excluded.extend(
-        ['_run_parameters', '_feeds_parameters', 'handler']
-    )
+    __modifiers__.excluded.append('handler')
 
     __slots__ = (
         "handler", 'amount', "loop", "limited", "_feeds_parameters",
         "_run_parameters", 'refresh'
     )
 
     screeners: List[BaseScreener]
@@ -586,18 +625,18 @@
                 ):
                     screener.stop()
                 # end if
             # end for
         # end for
     # end update
 
-    def stop(self) -> None:
-        """Stops the data handling loop."""
+    def stop_screening(self) -> None:
+        """Stops the screening process."""
 
-        super().stop()
+        super().stop_screening()
 
         self.loop: asyncio.AbstractEventLoop
 
         async def stop() -> None:
             """Stops the handler."""
 
             self.handler.stop(self.loop)
@@ -609,15 +648,15 @@
         for task in asyncio.all_tasks(self.loop):
             task.cancel()
         # end for
 
         self.loop = None
 
         self.handler.running = False
-    # end stop
+    # end stop_screening
 
     def start_screening(
             self,
             start: Optional[bool] = True,
             loop: Optional[asyncio.AbstractEventLoop] = None
     ) -> None:
         """
@@ -662,15 +701,15 @@
         :param loop: The event loop.
 
         :return: The start_timeout process.
         """
 
         self._run_parameters = dict(
             save=save, block=block, update=update, screen=screen,
-            loop=loop, wait=wait, timeout=timeout
+            loop=loop, wait=wait, timeout=timeout,
         )
 
         if not block:
             self.start_screening(loop=loop, start=screen)
         # end if
 
         super().run(
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.6.0/crypto_screening/market/screeners/trades.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
+from sqlalchemy import Engine
+
 from cryptofeed import FeedHandler
 from cryptofeed.types import Trade
 from cryptofeed.defines import TRADES
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     TRADES_COLUMNS, create_market_dataframe,
     AMOUNT, PRICE, SIDE, load_dataset, save_dataset
 )
+from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
     MarketScreener, structure_screener_datasets, MarketRecorder
 )
 
 __all__ = [
     "TradesMarketScreener",
@@ -89,14 +92,16 @@
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data as trades.
     """
 
+    NAME = "TRADES"
+
     @property
     def trades_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
@@ -111,15 +116,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-TRADES.csv")
+            replace(".csv", f"-{self.NAME}.csv")
         )
     # end trades_dataset_path
 
     def save_trades_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -165,21 +170,27 @@
         :param location: The saving location of the dataset.
         """
 
         self.load_trades_dataset(location=location)
     # end load_dataset
 # end TradesScreener
 
-def record_trades(market: Market, data: Trade, timestamp: float) -> bool:
+def record_trades(
+        market: Market,
+        data: Trade,
+        timestamp: float,
+        databases: Optional[Dict[str, Engine]] = None
+) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
+    :param databases: The database engines.
     """
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
     symbol = find_string_value(
         value=adjust_symbol(symbol=data.symbol),
@@ -195,14 +206,21 @@
     try:
         dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
             AMOUNT: float(data.amount),
             PRICE: float(data.price),
             SIDE: data.side
         }
 
+        if databases:
+            insert_database_record(
+                exchange=exchange, symbol=symbol, name=TradesScreener.NAME,
+                dataset=dataset, databases=databases
+            )
+        # end if
+
         return True
 
     except IndexError:
         return False
     # end try
 # end record_trades
 
@@ -294,15 +312,16 @@
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
         return record_trades(
-            market=self.market, data=data, timestamp=timestamp
+            market=self.market, data=data, timestamp=timestamp,
+            databases=self.databases
         )
     # end record
 # end TradesRecorder
 
 class TradesMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
@@ -516,37 +535,45 @@
             # end for
         # end for
 
         return screeners
     # end create_trades_screeners
 # end MarketOrderbookScreener
 
-def trades_market_recorder(data: Dict[str, Iterable[str]]) -> TradesMarketRecorder:
+Databases = Union[Iterable[str], Dict[str, Engine]]
+
+def trades_market_recorder(
+        data: Dict[str, Iterable[str]],
+        databases: Optional[Databases] = None
+) -> TradesMarketRecorder:
     """
     Creates the market recorder object for the data.
 
     :param data: The market data.
+    :param databases: The paths to the databases.
 
     :return: The market recorder object.
     """
 
     return TradesMarketRecorder(
-        market=create_trades_market(data=data)
+        market=create_trades_market(data=data),
+        databases=databases
     )
 # end trades_market_recorder
 
 def trades_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
+        databases: Optional[Databases] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[TradesMarketRecorder] = None,
         fixed: Optional[bool] = True,
         separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> TradesMarketScreener:
     """
@@ -561,21 +588,23 @@
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
+    :param databases: The paths to the databases.
 
     :return: The market screener object.
     """
 
     screener = TradesMarketScreener(
         recorder=recorder or TradesMarketRecorder(
-            market=market or create_trades_market(data=data)
+            market=market or create_trades_market(data=data),
+            databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(), fixed=fixed,
```

### Comparing `crypto-screening-5.5.0/crypto_screening/market/waiting.py` & `crypto-screening-5.6.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/process.py` & `crypto-screening-5.6.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/symbols.py` & `crypto-screening-5.6.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening/validate.py` & `crypto-screening-5.6.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.5.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.6.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.5.0
+Version: 5.6.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.5.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.6.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,8 +39,11 @@
 crypto_screening/market/screeners/base.py
 crypto_screening/market/screeners/combined.py
 crypto_screening/market/screeners/container.py
 crypto_screening/market/screeners/ohlcv.py
 crypto_screening/market/screeners/orderbook.py
 crypto_screening/market/screeners/orders.py
 crypto_screening/market/screeners/recorder.py
-crypto_screening/market/screeners/trades.py
+crypto_screening/market/screeners/trades.py
+crypto_screening/market/screeners/database/__init__.py
+crypto_screening/market/screeners/database/data.py
+crypto_screening/market/screeners/database/execution.py
```

### Comparing `crypto-screening-5.5.0/pyproject.toml` & `crypto-screening-5.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.5.0'
+version = '5.6.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.5.0/setup.py` & `crypto-screening-5.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.5.0',
+        version='5.6.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

