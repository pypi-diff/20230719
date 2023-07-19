# Comparing `tmp/crypto-screening-6.0.0.tar.gz` & `tmp/crypto-screening-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-6.0.0.tar", last modified: Wed Jul 19 00:03:01 2023, max compression
+gzip compressed data, was "crypto-screening-6.1.0.tar", last modified: Wed Jul 19 11:03:14 2023, max compression
```

## Comparing `crypto-screening-6.0.0.tar` & `crypto-screening-6.1.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.497197 crypto-screening-6.0.0/
--rw-rw-rw-   0        0        0       98 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-19 00:03:01.496197 crypto-screening-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-6.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-6.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.462198 crypto-screening-6.0.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.477197 crypto-screening-6.0.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-6.0.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-6.0.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.481197 crypto-screening-6.0.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-6.0.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-6.0.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-6.0.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-6.0.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.483197 crypto-screening-6.0.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24747 2023-07-18 21:10:08.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21735 2023-07-18 21:10:09.000000 crypto-screening-6.0.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-6.0.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16703 2023-07-18 21:41:58.000000 crypto-screening-6.0.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-6.0.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-6.0.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-6.0.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-6.0.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.485196 crypto-screening-6.0.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-6.0.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.487197 crypto-screening-6.0.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-6.0.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.494197 crypto-screening-6.0.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11429 2023-07-18 22:07:23.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13801 2023-07-18 23:55:50.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/container.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.496197 crypto-screening-6.0.0/crypto_screening/market/screeners/database/
--rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/database/__init__.py
--rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/database/data.py
--rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/database/execution.py
--rw-rw-rw-   0        0        0    38581 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    20374 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    19870 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    27176 2023-07-18 23:59:47.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    19944 2023-07-18 23:55:40.000000 crypto-screening-6.0.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-6.0.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-6.0.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-6.0.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-6.0.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:03:01.474238 crypto-screening-6.0.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-19 00:03:01.000000 crypto-screening-6.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-6.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-6.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 00:03:01.497197 crypto-screening-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-19 00:02:57.000000 crypto-screening-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.632928 crypto-screening-6.1.0/
+-rw-rw-rw-   0        0        0       98 2023-07-19 11:03:12.000000 crypto-screening-6.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-19 11:03:14.632928 crypto-screening-6.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-6.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-6.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.485437 crypto-screening-6.1.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.519747 crypto-screening-6.1.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-6.1.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-6.1.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.547550 crypto-screening-6.1.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-6.1.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-6.1.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-6.1.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-6.1.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.570699 crypto-screening-6.1.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-6.1.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24747 2023-07-18 21:10:08.000000 crypto-screening-6.1.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-6.1.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21735 2023-07-18 21:10:09.000000 crypto-screening-6.1.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-6.1.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16701 2023-07-19 10:06:31.000000 crypto-screening-6.1.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-6.1.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-6.1.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-6.1.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-6.1.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.581667 crypto-screening-6.1.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-6.1.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.596870 crypto-screening-6.1.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-6.1.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-6.1.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-6.1.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-6.1.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.608821 crypto-screening-6.1.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-19 09:07:33.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11400 2023-07-19 10:06:31.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     7812 2023-07-19 10:52:12.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/callbacks.py
+-rw-rw-rw-   0        0        0    13857 2023-07-19 08:52:21.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/container.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.631920 crypto-screening-6.1.0/crypto_screening/market/screeners/database/
+-rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/database/__init__.py
+-rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/database/data.py
+-rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/database/execution.py
+-rw-rw-rw-   0        0        0    38832 2023-07-19 10:19:04.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    20433 2023-07-19 10:19:04.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    19929 2023-07-19 10:19:04.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    21780 2023-07-19 10:06:31.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     6442 2023-07-19 10:55:51.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/sockets.py
+-rw-rw-rw-   0        0        0    20003 2023-07-19 10:19:04.000000 crypto-screening-6.1.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-6.1.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-6.1.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-6.1.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-6.1.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:03:14.502896 crypto-screening-6.1.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-19 11:03:14.000000 crypto-screening-6.1.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1927 2023-07-19 11:03:14.000000 crypto-screening-6.1.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 11:03:14.000000 crypto-screening-6.1.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-19 11:03:14.000000 crypto-screening-6.1.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 11:03:14.000000 crypto-screening-6.1.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-19 11:03:12.000000 crypto-screening-6.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-6.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-6.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 11:03:14.632928 crypto-screening-6.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-19 11:03:09.000000 crypto-screening-6.1.0/setup.py
```

### Comparing `crypto-screening-6.0.0/PKG-INFO` & `crypto-screening-6.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 6.0.0
+Version: 6.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-6.0.0/README.md` & `crypto-screening-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/build.py` & `crypto-screening-6.1.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/assets.py` & `crypto-screening-6.1.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/exchanges.py` & `crypto-screening-6.1.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/orders.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/market/trades.py` & `crypto-screening-6.1.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/screeners.py` & `crypto-screening-6.1.0/crypto_screening/collect/screeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,18 +228,18 @@
     return structure
 # end structure_screeners
 
 def find_screeners(
         screeners: Iterable[BaseScreener], exchange: str, symbol: str
 ) -> List[BaseScreener]:
     """
-    Finds all the screeners with the matching exchange and symbol name.
+    Finds all the screeners with the matching exchange and symbol key.
 
     :param screeners: The screeners to process.
-    :param exchange: The exchange name for the symbol.
+    :param exchange: The exchange key for the symbol.
     :param symbol: The pair symbol to search its screeners.
 
     :return: The matching screeners.
     """
 
     return [
         screener for screener in screeners
```

### Comparing `crypto-screening-6.0.0/crypto_screening/collect/symbols.py` & `crypto-screening-6.1.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/dataset.py` & `crypto-screening-6.1.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/interval.py` & `crypto-screening-6.1.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/dynamic.py` & `crypto-screening-6.1.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/foundation/data.py` & `crypto-screening-6.1.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-6.1.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/foundation/state.py` & `crypto-screening-6.1.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-6.1.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/base.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     Parameters:
 
     - symbol:
         The symbol of an asset to screen.
 
     - exchange:
-        The name of the exchange platform to screen data from.
+        The key of the exchange platform to screen data from.
 
     - location:
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
@@ -142,29 +142,29 @@
     # end await_update
 
     @staticmethod
     def validate_exchange(exchange: str) -> str:
         """
         Validates the symbol value.
 
-        :param exchange: The exchange name.
+        :param exchange: The exchange key.
 
         :return: The validates symbol.
         """
 
         return validate_exchange(exchange=exchange)
     # end validate_exchange
 
     @staticmethod
     def validate_symbol(exchange: str, symbol: Any) -> str:
         """
         Validates the symbol value.
 
-        :param exchange: The exchange name.
-        :param symbol: The name of the symbol.
+        :param exchange: The exchange key.
+        :param symbol: The key of the symbol.
 
         :return: The validates symbol.
         """
 
         return validate_symbol(
             exchange=exchange, symbol=symbol,
             symbols=all_exchange_symbols(exchange=exchange)
@@ -267,19 +267,19 @@
         The delay to wait between each data fetching.
 
     - screeners:
         The screener object to control and fill with data.
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
-    __modifiers__.hidden.extend(["screeners", 'recorder'])
+    __modifiers__.hidden.append("screeners")
 
     screeners: List[BaseScreener]
 
-    __slots__ = 'recorder', 'screeners'
+    __slots__ = 'screeners',
 
     def __init__(
             self,
             screeners: Optional[Iterable[BaseScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/combined.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 from crypto_screening.market.screeners.orders import (
     orders_market_screener, OrdersScreener,
     OrdersMarketRecorder
 )
 from crypto_screening.market.screeners.database.data import (
     validate_database_engines
 )
+from crypto_screening.market.screeners.callbacks import Callback
 from crypto_screening.market.screeners.recorder import (
-    MarketScreener, Callback
+    MarketScreener
 )
 
 __all__ = [
     "CombinedMarketRecorder",
     "CombinedMarketScreener",
     "combined_market_screener",
     "CATEGORIES",
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/container.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/database/data.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/database/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/database/execution.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/database/execution.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # ohlcv.py
 
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any, Union, List, Callable
+    Dict, Optional, Iterable, Any,
+    Union, List, Callable, Tuple
 )
 
 import pandas as pd
 
 from sqlalchemy import Engine
 
 from represent import Modifiers
@@ -20,22 +21,20 @@
 from crypto_screening.dataset import (
     OHLCV_COLUMNS, VOLUME, BIDS, BIDS_VOLUME,
     load_dataset, save_dataset, OHLC_COLUMNS, create_market_dataframe
 )
 from crypto_screening.validate import validate_interval
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.recorder import (
-    MarketRecorder, validate_market, Callback
-)
+from crypto_screening.market.screeners.callbacks import Callback
+from crypto_screening.market.screeners.recorder import MarketRecorder, validate_market
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.orderbook import (
     create_orderbook_dataframe, OrderbookScreener, record_orderbook,
-    OrderbookMarketScreener, create_orderbook_market,
-    OrderbookMarketRecorder
+    OrderbookMarketScreener, create_orderbook_market, OrderbookMarketRecorder
 )
 
 __all__ = [
     "OHLCVMarketScreener",
     "OHLCVMarketRecorder",
     "OHLCVScreener",
     "create_ohlcv_market",
@@ -100,15 +99,15 @@
 
     Parameters:
 
     - symbol:
         The symbol of an asset to screen.
 
     - exchange:
-        The name of the exchange platform to screen data from.
+        The key of the exchange platform to screen data from.
 
     - location:
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
@@ -572,42 +571,45 @@
             adjuster = f'{interval_total_minutes}Min'
 
             ohlcv: pd.DataFrame = spread[BIDS].resample(adjuster).ohlc()
             ohlcv.columns = list(OHLC_COLUMNS)
             volume: pd.DataFrame = spread[BIDS_VOLUME].resample(adjuster).ohlc()
             ohlcv[VOLUME] = volume[list(volume.columns)[-1]]
 
-            data = []
+            data: List[Tuple[float, Dict[str, Any]]] = []
 
             for index, row in ohlcv.iterrows():
+                index: dt.datetime
+
                 ohlcv_dataset.loc[index] = row
 
-                data.append(row.to_dict())
+                data.append((index.timestamp(), row.to_dict()))
             # end for
 
             indexes[exchange][symbol][interval] += 1
-        # end for
 
-        if databases:
-            insert_database_record(
-                exchange=exchange, symbol=symbol,
-                name=OHLCVScreener.NAME, interval=interval,
-                dataset=ohlcv_dataset, databases=databases
-            )
-        # end if
+            for callback in callbacks or []:
+                payload = {
+                    'data': data,
+                    'interval': interval,
+                    'exchange': exchange,
+                    'symbol': symbol
+                }
 
-        for callback in callbacks or []:
-            data = {
-                'data': data,
-                'exchange': exchange,
-                'symbol': symbol
-            }
+                callback.record(payload, timestamp, key=OHLCVScreener.NAME)
+            # end if
 
-            callback.record(data, timestamp, name=OHLCVScreener.NAME)
-        # end if
+            if databases:
+                insert_database_record(
+                    exchange=exchange, symbol=symbol,
+                    name=OHLCVScreener.NAME, interval=interval,
+                    dataset=ohlcv_dataset, databases=databases
+                )
+            # end if
+        # end for
     # end for
 
     return True
 # end record_ohlcv
 
 RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 Databases = Union[Iterable[str], Dict[str, Engine]]
@@ -740,15 +742,15 @@
         )
     # end parameters
 
     def ohlcv(self, exchange: str, symbol: str, interval: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
         :param interval: The interval for the dataset.
 
         :return: The dataset of the spread data.
         """
 
         self.data(exchange=exchange, symbol=symbol)
@@ -768,15 +770,15 @@
         return intervals[interval]
     # end ohlcv
 
     def ohlcv_in_market(self, exchange: str, symbol: str, interval: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
         :param interval: The interval for the dataset.
 
         :return: The dataset of the spread data.
         """
 
         try:
@@ -998,15 +1000,15 @@
         # end for
     # end connect_screeners
 
     def ohlcv(self, exchange: str, symbol: str, interval: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
         :param interval: The interval for the dataset.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.ohlcv(
@@ -1014,15 +1016,15 @@
         )
     # end orderbook
 
     def ohlcv_in_market(self, exchange: str, symbol: str, interval: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
         :param interval: The interval for the dataset.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.ohlcv_in_market(
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, save_dataset,
     create_market_dataframe, ORDERBOOK_COLUMNS, load_dataset
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.recorder import (
-    MarketScreener, MarketRecorder, Callback
-)
+from crypto_screening.market.screeners.callbacks import Callback
+from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
 
 __all__ = [
     "OrderbookMarketScreener",
     "OrderbookMarketRecorder",
     "OrderbookScreener",
     "create_orderbook_market",
     "orderbook_market_screener",
@@ -77,15 +76,15 @@
 
     Parameters:
 
     - symbol:
         The symbol of an asset to screen.
 
     - exchange:
-        The name of the exchange platform to screen data from.
+        The key of the exchange platform to screen data from.
 
     - location:
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
@@ -224,21 +223,21 @@
             insert_database_record(
                 exchange=exchange, symbol=symbol, name=OrderbookScreener.NAME,
                 dataset=dataset, databases=databases
             )
         # end if
 
         for callback in callbacks or []:
-            data = {
-                'data': [data],
+            payload = {
+                'data': [(timestamp, data)],
                 'exchange': exchange,
                 'symbol': symbol
             }
 
-            callback.record(data, timestamp, name=OrderbookScreener.NAME)
+            callback.record(payload, timestamp, key=OrderbookScreener.NAME)
         # end if
 
         return True
 
     except IndexError:
         return False
     # end try
@@ -297,28 +296,28 @@
         )
     # end parameters
 
     def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
     # end orderbook
 
     def orderbook_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         try:
             self.orderbook(exchange=exchange, symbol=symbol)
@@ -473,28 +472,28 @@
         # end for
     # end connect_screeners
 
     def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.orderbook(exchange=exchange, symbol=symbol)
     # end orderbook
 
     def orderbook_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.orderbook_in_market(exchange=exchange, symbol=symbol)
     # end orderbook_in_market
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     BIDS, ASKS, ORDERS_COLUMNS, create_market_dataframe,
     load_dataset, save_dataset
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.recorder import (
-    MarketScreener, MarketRecorder, Callback
-)
+from crypto_screening.market.screeners.callbacks import Callback
+from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
 
 __all__ = [
     "OrdersMarketScreener",
     "OrdersMarketRecorder",
     "OrdersScreener",
     "create_orders_market",
     "orders_market_screener",
@@ -77,15 +76,15 @@
 
     Parameters:
 
     - symbol:
         The symbol of an asset to screen.
 
     - exchange:
-        The name of the exchange platform to screen data from.
+        The key of the exchange platform to screen data from.
 
     - location:
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
@@ -219,21 +218,21 @@
             insert_database_record(
                 exchange=exchange, symbol=symbol, name=OrdersScreener.NAME,
                 dataset=dataset, databases=databases
             )
         # end if
 
         for callback in callbacks or []:
-            data = {
-                'data': [data],
+            payload = {
+                'data': [(timestamp, data)],
                 'exchange': exchange,
                 'symbol': symbol
             }
 
-            callback.record(data, timestamp, name=OrdersScreener.NAME)
+            callback.record(payload, timestamp, key=OrdersScreener.NAME)
         # end if
 
         return True
 
     except IndexError:
         return False
     # end try
@@ -292,28 +291,28 @@
         )
     # end parameters
 
     def orders(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
     # end orders
 
     def orders_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         try:
             self.orders(exchange=exchange, symbol=symbol)
@@ -468,28 +467,28 @@
         # end for
     # end connect_screeners
 
     def orders(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.orders(exchange=exchange, symbol=symbol)
     # end orders
 
     def orders_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.orders_in_market(exchange=exchange, symbol=symbol)
     # end orders_in_market
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/recorder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 # recorder.py
 
 import warnings
-import json
 import threading
 import time
 import datetime as dt
 from typing import (
     Optional, Dict, Any, List,
     Iterable, Type, Union
 )
 from functools import partial
 import asyncio
-from textwrap import wrap
 
 import pandas as pd
 
 from sqlalchemy import Engine
 
 from represent import Modifiers, represent
 
 from cryptofeed import FeedHandler
 from cryptofeed.feed import Feed
-from cryptofeed.backends.socket import UDPProtocol
 
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.database.data import validate_database_engines
 from crypto_screening.market.screeners.base import BaseMarketScreener, BaseScreener
+from crypto_screening.market.screeners.callbacks import Callback
 
 __all__ = [
     "MarketHandler",
     "ExchangeFeed",
     "FEED_GROUP_SIZE",
     "add_feeds",
     "MarketScreener",
     "structure_screeners_datasets",
     "structure_screener_datasets",
     "MarketRecorder",
-    "validate_market",
-    "Callback",
-    "SocketCallback"
+    "validate_market"
 ]
 
 class MarketHandler(FeedHandler):
     """A class to handle the market data feed."""
 
     def __init__(self) -> None:
         """Defines the class attributes."""
@@ -190,215 +186,14 @@
         )
     # end try
 
     return data
 # end validate_market
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
-
-class Callback:
-    """A class to represent a callback."""
-
-    NAME: str = None
-    CONNECTABLE: bool = False
-    ADJUSTABLE: bool = True
-
-    def __init__(self, name: Optional[Any] = None) -> None:
-        """
-        Defines the class attributes.
-
-        :param name: The key od the data.
-        """
-
-        self.name = name if name else self.NAME
-    # end __init__
-
-    def record(self, data: Any, timestamp: float, name: Optional[Any] = None) -> bool:
-        """
-        Records the data from the crypto feed into the dataset.
-
-        :param data: The data from the exchange.
-        :param timestamp: The time of the request.
-        :param name: The key for the data type.
-
-        :return: The validation value.
-        """
-    # end record
-
-    @property
-    def connectable(self) -> bool:
-        """
-        Checks if the connection was created.
-
-        :return: The existence of a connection.
-        """
-
-        return self.CONNECTABLE
-    # end connectable
-
-    @property
-    def adjustable(self) -> bool:
-        """
-        Checks if the connection was created.
-
-        :return: The existence of a connection.
-        """
-
-        return self.ADJUSTABLE
-    # end adjustable
-
-    async def connect(self) -> None:
-        """Connects to the socket service."""
-    # end connect
-# end Callback
-
-class SocketCallback(Callback):
-    """A class to represent a socket callback."""
-
-    BUFFER = 1024
-
-    PROTOCOLS = ('tcp://', 'udp://')
-
-    CONNECTABLE = True
-
-    def __init__(
-            self,
-            address: str,
-            port: int,
-            name: Optional[Any] = None,
-            buffer: Optional[int] = None
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param address: The address of the socket.
-        :param port: The port of the socket.
-        :param name: The key od the data.
-        :param buffer: The buffer size.
-        """
-
-        super().__init__(name=name)
-
-        buffer = buffer or self.BUFFER
-
-        protocol = address[:6]
-
-        if protocol not in self.PROTOCOLS:
-            raise ValueError(
-                f"Invalid protocol: {protocol}. "
-                f"Protocol must be one of: {', '.join(self.PROTOCOLS)}"
-            )
-        # end if
-
-        self.connection = None
-        self.protocol = protocol
-        self.address = address[6:]
-        self.port = port
-        self.buffer = buffer
-
-        self.running = False
-    # end __init__
-
-    @property
-    def connected(self) -> bool:
-        """
-        Checks if the connection was created.
-
-        :return: The existence of a connection.
-        """
-
-        return self.connection is not None
-    # end connected
-
-    # noinspection PyTypeChecker
-    async def connect(self) -> None:
-        """Connects to the socket service."""
-
-        if self.connection is not None:
-            warnings.warn(f"{repr(self)} callback is already connected.")
-
-            return
-        # end if
-
-        try:
-            if self.protocol == 'udp://':
-                loop = asyncio.get_event_loop()
-                self.connection, self.protocol = (
-                    await loop.create_datagram_endpoint(
-                        lambda: UDPProtocol(loop),
-                        remote_addr=(self.address, self.port)
-                    )
-                )
-
-            elif self.protocol == 'tcp://':
-                _, self.connection = await asyncio.open_connection(
-                    host=self.address, port=self.port
-                )
-            # end if
-
-            self.running = True
-
-        except Exception as e:
-            if self.adjustable:
-                warnings.warn(f"{type(e)}: {str(e)}")
-
-            else:
-                raise e
-            # end if
-        # end try
-    # end connect
-
-    def record(self, data: Any, timestamp: float, name: Optional[Any] = None) -> bool:
-        """
-        Records the data from the crypto feed into the dataset.
-
-        :param data: The data from the exchange.
-        :param timestamp: The time of the request.
-        :param name: The key for the data type.
-
-        :return: The validation value.
-        """
-
-        if not (self.running and self.connected):
-            return False
-        # end if
-
-        data = json.dumps({'name': self.name or name, 'data': data})
-
-        if self.protocol == 'udp://':
-            if len(data) > self.buffer:
-                chunks = wrap(data, self.buffer)
-
-                for chunk in chunks:
-                    message = json.dumps(
-                        {
-                            'type': 'chunked',
-                            'chunks': len(chunks),
-                            'data': chunk,
-                            'timestamp': float(timestamp)
-                        }
-                    ).encode()
-
-                    self.connection.sendto(message)
-                # end for
-
-                return True
-            # end if
-        # end if
-
-        self.connection.write(
-            json.dumps(
-                {'data': data, 'timestamp': float(timestamp)}
-            ).encode()
-        )
-
-        return True
-    # end writer
-# end SocketCallback
-
 Callbacks = Iterable[Callback]
 
 @represent
 class MarketRecorder:
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
@@ -516,15 +311,15 @@
         }
     # end structure
 
     def data(self, exchange: str, symbol: str) -> Any:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         exchange = find_string_value(
             value=exchange, values=self.market.keys()
@@ -547,15 +342,15 @@
         return self.market[exchange][symbol]
     # end data
 
     def in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         try:
             self.data(exchange=exchange, symbol=symbol)
@@ -607,15 +402,15 @@
     """
 
     __modifiers__ = Modifiers(**BaseMarketScreener.__modifiers__)
     __modifiers__.excluded.append('handler')
 
     __slots__ = (
         "handler", 'amount', "loop", "limited", "_feeds_parameters",
-        "_run_parameters", 'refresh'
+        "_run_parameters", 'refresh', 'recorder'
     )
 
     screeners: List[BaseScreener]
     recorder: MarketRecorder
 
     DELAY = 1
     AMOUNT = FEED_GROUP_SIZE
@@ -876,15 +671,15 @@
         Starts the screening process.
 
         :param start: The value to start the loop.
         :param loop: The event loop.
         """
 
         if self.screening:
-            warnings.warn(f"Timeout process of {self} is already running.")
+            warnings.warn(f"Timeout screening of {self} is already running.")
 
             return
         # end if
 
         self._screening_process = threading.Thread(
             target=lambda: self.screening_loop(loop=loop, start=start)
         )
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-6.1.0/crypto_screening/market/screeners/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     TRADES_COLUMNS, create_market_dataframe,
     AMOUNT, PRICE, SIDE, load_dataset, save_dataset
 )
 from crypto_screening.market.screeners.database.data import insert_database_record
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.recorder import (
-    MarketScreener, MarketRecorder, Callback
-)
+from crypto_screening.market.screeners.callbacks import Callback
+from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
 
 __all__ = [
     "TradesMarketScreener",
     "TradesMarketRecorder",
     "TradesScreener",
     "create_trades_market",
     "trades_market_screener",
@@ -77,15 +76,15 @@
 
     Parameters:
 
     - symbol:
         The symbol of an asset to screen.
 
     - exchange:
-        The name of the exchange platform to screen data from.
+        The key of the exchange platform to screen data from.
 
     - location:
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
@@ -220,21 +219,21 @@
             insert_database_record(
                 exchange=exchange, symbol=symbol, name=TradesScreener.NAME,
                 dataset=dataset, databases=databases
             )
         # end if
 
         for callback in callbacks or []:
-            data = {
-                'data': [data],
+            payload = {
+                'data': [(timestamp, data)],
                 'exchange': exchange,
                 'symbol': symbol
             }
 
-            callback.record(data, timestamp, name=TradesScreener.NAME)
+            callback.record(payload, timestamp, key=TradesScreener.NAME)
         # end if
 
         return True
 
     except IndexError:
         return False
     # end try
@@ -293,28 +292,28 @@
         )
     # end parameters
 
     def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
     # end trades
 
     def trades_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         try:
             self.trades(exchange=exchange, symbol=symbol)
@@ -471,28 +470,28 @@
         # end for
     # end connect_screeners
 
     def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.trades(exchange=exchange, symbol=symbol)
     # end trades
 
     def trades_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
-        :param exchange: The source name of the exchange.
+        :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.trades_in_market(exchange=exchange, symbol=symbol)
     # end trades_in_market
```

### Comparing `crypto-screening-6.0.0/crypto_screening/market/waiting.py` & `crypto-screening-6.1.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/process.py` & `crypto-screening-6.1.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/symbols.py` & `crypto-screening-6.1.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening/validate.py` & `crypto-screening-6.1.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-6.0.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-6.1.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 6.0.0
+Version: 6.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-6.0.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-6.1.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,19 @@
 crypto_screening/market/waiting.py
 crypto_screening/market/foundation/data.py
 crypto_screening/market/foundation/protocols.py
 crypto_screening/market/foundation/state.py
 crypto_screening/market/foundation/waiting.py
 crypto_screening/market/screeners/__init__.py
 crypto_screening/market/screeners/base.py
+crypto_screening/market/screeners/callbacks.py
 crypto_screening/market/screeners/combined.py
 crypto_screening/market/screeners/container.py
 crypto_screening/market/screeners/ohlcv.py
 crypto_screening/market/screeners/orderbook.py
 crypto_screening/market/screeners/orders.py
 crypto_screening/market/screeners/recorder.py
+crypto_screening/market/screeners/sockets.py
 crypto_screening/market/screeners/trades.py
 crypto_screening/market/screeners/database/__init__.py
 crypto_screening/market/screeners/database/data.py
 crypto_screening/market/screeners/database/execution.py
```

### Comparing `crypto-screening-6.0.0/pyproject.toml` & `crypto-screening-6.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '6.0.0'
+version = '6.1.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-6.0.0/setup.py` & `crypto-screening-6.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='6.0.0',
+        version='6.1.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

