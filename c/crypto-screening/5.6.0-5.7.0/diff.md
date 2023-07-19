# Comparing `tmp/crypto-screening-5.6.0.tar.gz` & `tmp/crypto-screening-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.6.0.tar", last modified: Tue Jul 18 09:15:46 2023, max compression
+gzip compressed data, was "crypto-screening-5.7.0.tar", last modified: Tue Jul 18 22:08:43 2023, max compression
```

## Comparing `crypto-screening-5.6.0.tar` & `crypto-screening-5.7.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.030021 crypto-screening-5.6.0/
--rw-rw-rw-   0        0        0       98 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-18 09:15:46.030021 crypto-screening-5.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.6.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.6.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:45.997510 crypto-screening-5.6.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.009510 crypto-screening-5.6.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.6.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.6.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.013513 crypto-screening-5.6.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.6.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19456 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12436 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.016514 crypto-screening-5.6.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24779 2023-07-17 09:51:27.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    14887 2023-07-17 10:00:22.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21766 2023-07-17 09:50:45.000000 crypto-screening-5.6.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    14999 2023-07-17 09:43:58.000000 crypto-screening-5.6.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16697 2023-07-17 09:46:37.000000 crypto-screening-5.6.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.6.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.6.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.6.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.6.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.018513 crypto-screening-5.6.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19658 2023-07-16 14:05:40.000000 crypto-screening-5.6.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.020513 crypto-screening-5.6.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10763 2023-07-16 14:12:22.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.6.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.027017 crypto-screening-5.6.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10987 2023-07-17 21:45:06.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13753 2023-07-18 09:13:48.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/container.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.029021 crypto-screening-5.6.0/crypto_screening/market/screeners/database/
--rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/database/__init__.py
--rw-rw-rw-   0        0        0     8835 2023-07-18 09:10:50.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/database/data.py
--rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/database/execution.py
--rw-rw-rw-   0        0        0    37739 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19397 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18899 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    21401 2023-07-18 09:10:57.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18931 2023-07-18 09:10:16.000000 crypto-screening-5.6.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.6.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.6.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.6.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4233 2023-07-17 08:56:51.000000 crypto-screening-5.6.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:15:46.006510 crypto-screening-5.6.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-18 09:15:45.000000 crypto-screening-5.6.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-18 08:49:04.000000 crypto-screening-5.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-5.6.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-5.6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 09:15:46.030021 crypto-screening-5.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-18 08:48:48.000000 crypto-screening-5.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.800255 crypto-screening-5.7.0/
+-rw-rw-rw-   0        0        0       98 2023-07-18 22:08:42.000000 crypto-screening-5.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-18 22:08:43.800255 crypto-screening-5.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.7.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.7.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.727247 crypto-screening-5.7.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.754247 crypto-screening-5.7.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.7.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.7.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.767247 crypto-screening-5.7.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-5.7.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-5.7.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-5.7.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-5.7.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.773247 crypto-screening-5.7.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24747 2023-07-18 21:10:08.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21735 2023-07-18 21:10:09.000000 crypto-screening-5.7.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-5.7.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16703 2023-07-18 21:41:58.000000 crypto-screening-5.7.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-5.7.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.7.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.7.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.7.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.775277 crypto-screening-5.7.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-5.7.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.777248 crypto-screening-5.7.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-5.7.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.783247 crypto-screening-5.7.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11429 2023-07-18 22:07:23.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13670 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/container.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.799248 crypto-screening-5.7.0/crypto_screening/market/screeners/database/
+-rw-rw-rw-   0        0        0       17 2023-07-18 09:11:14.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/database/__init__.py
+-rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/database/data.py
+-rw-rw-rw-   0        0        0    19095 2023-07-17 23:07:10.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/database/execution.py
+-rw-rw-rw-   0        0        0    38366 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    19721 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    19217 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    21485 2023-07-18 21:41:58.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    19249 2023-07-18 17:21:00.000000 crypto-screening-5.7.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-5.7.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.7.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-5.7.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-5.7.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:08:43.741277 crypto-screening-5.7.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-18 22:08:43.000000 crypto-screening-5.7.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-18 22:08:42.000000 crypto-screening-5.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-5.7.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-5.7.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 22:08:43.800255 crypto-screening-5.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-18 22:08:32.000000 crypto-screening-5.7.0/setup.py
```

### Comparing `crypto-screening-5.6.0/PKG-INFO` & `crypto-screening-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.6.0
+Version: 5.7.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.6.0/README.md` & `crypto-screening-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/build.py` & `crypto-screening-5.7.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/assets.py` & `crypto-screening-5.7.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/exchanges.py` & `crypto-screening-5.7.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
+from crypto_screening.dataset import OPEN, HIGH, LOW, CLOSE, VOLUME
+
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
-    MarketState, assets_market_values, OHLCV_ATTRIBUTES,
+    MarketState, assets_market_values, SymbolsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
-    merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
+    merge_assets_market_states_data, AssetsMarketState
 )
 
 __all__ = [
     "symbols_ohlcv_market_state",
     "merge_assets_ohlcv_market_states",
     "merge_symbols_ohlcv_market_states",
     "assets_ohlcv_market_state",
@@ -33,14 +35,22 @@
     "assets_to_symbols_ohlcv_market_state",
     "OHLCV_ATTRIBUTES"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
+OHLCV_ATTRIBUTES = {
+    "opens": OPEN,
+    "highs": HIGH,
+    "lows": LOW,
+    "closes": CLOSE,
+    "volumes": VOLUME
+}
+
 @define(repr=False)
 @represent
 class OHLCVMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
@@ -48,17 +58,15 @@
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
 
-    __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **MarketState.__modifiers__
-    )
+    __modifiers__: ClassVar[Modifiers] = Modifiers(**MarketState.__modifiers__)
     __modifiers__.excluded.extend(["open", "high", "low", "close", "volume"])
 
     ATTRIBUTES: ClassVar[Dict[str, str]] = OHLCV_ATTRIBUTES
 # end OrderbookMarketBase
 
 AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
 AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/orders.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
+from crypto_screening.dataset import BIDS, ASKS
+
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
-    MarketState, assets_market_values, ORDERS_ATTRIBUTES,
+    MarketState, assets_market_values, SymbolsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
-    merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
+    merge_assets_market_states_data, AssetsMarketState
 )
 
 __all__ = [
     "symbols_orders_market_state",
     "merge_assets_orders_market_states",
     "merge_symbols_orders_market_states",
     "assets_orders_market_state",
@@ -33,14 +35,19 @@
     "assets_to_symbols_orders_market_state",
     "ORDERS_ATTRIBUTES"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
+ORDERS_ATTRIBUTES = {
+    "bids": BIDS,
+    "asks": ASKS
+}
+
 @define(repr=False)
 @represent
 class OrdersMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/state/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -770,16 +770,16 @@
 
 @define(repr=False)
 @represent
 class AssetsMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
-    This object contains the state of the market, as Close,
-    bids and asks values of specific assets, gathered from the network.
+    This class is a base class for containers of structured market data,
+    with assets structure.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/state/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,45 @@
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, bid_ask_to_ohlcv,
-    OPEN, HIGH, LOW, CLOSE, VOLUME, AMOUNT, SIDE, PRICE
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, bid_ask_to_ohlcv
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.market.screeners.orders import OrdersScreener
 from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.dataset import dataset_to_json
 from crypto_screening.collect.screeners import find_screeners
 
 __all__ = [
     "is_exchange_in_market_data",
     "dataset_to_data_rows",
     "MarketState",
     "ORDERBOOK_ATTRIBUTES",
-    "OHLCV_ATTRIBUTES",
-    "ORDERS_ATTRIBUTES",
-    "TRADES_ATTRIBUTES",
     "add_data_to_symbols_screeners",
     "add_data_to_screeners",
     "adjusted_dataset_length",
     "set_screener_dataset",
     "is_match",
     "screener_dataset",
     "get_last_value",
     "no_match_error",
     "is_ohlcv_orderbook_match",
     "minimum_common_dataset_length",
     "index_to_datetime",
     "data_from_dataset",
     "adjusted_screener_dataset_length",
-    "sort_data"
+    "sort_data",
+    "validate_market_state_attributes",
+    "is_valid_state_attributes"
 ]
 
 _V = TypeVar("_V")
 
 Data = List[Tuple[dt.datetime, _V]]
 
 def data_from_dataset(
@@ -116,40 +114,112 @@
 
 @define(repr=False)
 @represent
 class MarketState(metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
-    This object contains the state of the market, as Close,
-    bids and asks values of specific assets, gathered from the network.
+    This class is a base class for containers of structured market data,
+    with assets structure or symbols structure.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
 
     screeners: Iterable[BaseScreener]
 
-    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
+    __modifiers__: ClassVar[Modifiers] = Modifiers(hidden=["screeners"])
 
     ATTRIBUTES: ClassVar[Dict[str, str]]
 
     def __hash__(self) -> int:
         """
         Returns the hash of the object.
 
         :return: The hash of the object.
         """
 
         return id(self)
     # end __hash__
+
+    def __attrs_post_init__(self) -> None:
+        """Defines the class attributes."""
+
+        self.validate_market_state_attributes()
+
+    # end __init__
+
+    def validate_market_state_attributes(self) -> None:
+        """Validates the market state's attributes."""
+
+        validate_market_state_attributes(self)
+    # end validate_market_state_attributes
 # end MarketState
 
+def validate_market_state_attributes(state: MarketState) -> None:
+    """
+    Validates the market state's attributes.
+
+    :param state: The market state object.
+    """
+
+    if not hasattr(state, "ATTRIBUTES"):
+        raise ValueError(
+            f"'ATTRIBUTES' instance or class attribute "
+            f"must be defined for: {repr(state)}"
+        )
+
+    elif not (
+        isinstance(state.ATTRIBUTES, dict) and
+        all(
+            isinstance(key, str) and isinstance(value, str)
+            for key, value in state.ATTRIBUTES.items()
+        )
+    ):
+        raise ValueError(
+            f"'ATTRIBUTES' must de of type: {Dict[str, str]}, "
+            f"not: {state.ATTRIBUTES}"
+        )
+    # end if
+
+    missing = [
+        attribute for attribute in state.ATTRIBUTES
+        if not hasattr(state, attribute)
+    ]
+
+    if missing:
+        raise ValueError(
+            f"{repr(state)} must contain all attributes defined in "
+            f"'ATTRIBUTES': {state.ATTRIBUTES}. "
+            f"Missing attributes: {', '.join(missing)}"
+        )
+    # end if
+# end validate_market_state_attributes
+
+def is_valid_state_attributes(state: MarketState) -> bool:
+    """
+    Validates the market state's attributes.
+
+    :param state: The market state object.
+
+    :return: The value of validation.
+    """
+
+    try:
+        validate_market_state_attributes(state)
+
+        return True
+
+    except ValueError:
+        return False
+    # end if
+# end is_valid_state_attributes
+
 def sort_data(data: Data) -> None:
     """
     Sorts the data of the market.
 
     :param data: The data to sort.
     """
 
@@ -184,53 +254,26 @@
 
 ORDERBOOK_ATTRIBUTES = {
     "bids": BIDS,
     "asks": ASKS,
     "bids_volume": BIDS_VOLUME,
     "asks_volume": ASKS_VOLUME
 }
-OHLCV_ATTRIBUTES = {
-    "opens": OPEN,
-    "highs": HIGH,
-    "lows": LOW,
-    "closes": CLOSE,
-    "volumes": VOLUME
-}
-ORDERS_ATTRIBUTES = {
-    "bids": BIDS,
-    "asks": ASKS
-}
-TRADES_ATTRIBUTES = {
-    "amounts": AMOUNT,
-    "prices": PRICE,
-    "sides": SIDE
-}
-
-SCREENER_ATTRIBUTES_MATCHES = {
-    OrderbookScreener: ORDERBOOK_ATTRIBUTES,
-    OHLCVScreener: OHLCV_ATTRIBUTES,
-    OrdersScreener: ORDERS_ATTRIBUTES,
-    TradesScreener: TRADES_ATTRIBUTES
-}
 
 def is_match(screener: BaseScreener, columns: Iterable[str]) -> bool:
     """
     Checks if the screener matches the columns of the data.
 
     :param screener: The screener object.
     :param columns: The columns.
 
     :return: The matching boolean flag.
     """
 
-    return any(
-        isinstance(screener, base) and
-        (set(columns) == set(attributes.values()))
-        for base, attributes in SCREENER_ATTRIBUTES_MATCHES.items()
-    )
+    return set(screener.market.columns) == set(columns)
 # end is_match
 
 def is_ohlcv_orderbook_match(screener: BaseScreener, columns: Iterable[str]) -> bool:
     """
     Checks if the screener matches the columns of the data.
 
     :param screener: The screener object.
@@ -284,28 +327,28 @@
 
     :return: The screener object.
     """
 
     if is_ohlcv_orderbook_match(screener=screener, columns=dataset.columns):
         spread_dataset = dataset
 
-        if (screener.orderbook_market is not None) and clean:
+        if isinstance(screener.orderbook_market, pd.DataFrame) and clean:
             screener.orderbook_market.drop(screener.orderbook_market.index, inplace=True)
         # end if
 
         if (screener.orderbook_market is None) or replace:
             screener.orderbook_market = spread_dataset
 
         else:
             for index, row in spread_dataset.iterrows():
                 screener.orderbook_market[index] = row
             # end for
         # end if
 
-        if (screener.market is not None) and clean:
+        if isinstance(screener.market, pd.DataFrame) and clean:
             screener.market.drop(screener.market.index, inplace=True)
         # end if
 
         ohlcv_dataset = bid_ask_to_ohlcv(spread_dataset, interval=screener.interval)
 
         if (screener.market is None) or replace:
             screener.market = ohlcv_dataset
@@ -318,15 +361,15 @@
 
     elif not (force or is_match(screener=screener, columns=dataset.columns)):
         if not adjust:
             raise no_match_error(screener=screener, columns=dataset.columns)
         # end if
 
     else:
-        if (screener.market is not None) and clean:
+        if isinstance(screener.market, pd.DataFrame) and clean:
             screener.market.drop(screener.market.index, inplace=True)
         # end if
 
         if (screener.market is None) or replace:
             screener.market = dataset
 
         else:
@@ -488,15 +531,15 @@
     """
 
     if adjust and (length is None):
         length = len(dataset)
 
     elif adjust:
         length = min([len(dataset), length])
-        # end if
+    # end if
 
     if length > len(dataset):
         raise ValueError(
             f"Data is not long enough for the requested length: {length}. "
             f"Consider using the 'adjust' parameter as {True}, "
             f"to adjust to the actual length of the data."
         )
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/state/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,16 +701,16 @@
 
 @define(repr=False)
 @represent
 class SymbolsMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
-    This object contains the state of the market, as Close,
-    bids and asks values of specific assets, gathered from the network.
+    This class is a base class for containers of structured market data,
+    with symbols structure.
 
     attributes:
 
     - screeners:
         The screener objects to collect the values of the assets.
     """
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/market/trades.py` & `crypto-screening-5.7.0/crypto_screening/collect/market/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
+from crypto_screening.dataset import PRICE, AMOUNT, SIDE
+
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.collect.market.state import (
-    MarketState, assets_market_values, TRADES_ATTRIBUTES,
+    MarketState, assets_market_values, SymbolsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
-    merge_assets_market_states_data, AssetsMarketState, SymbolsMarketState
+    merge_assets_market_states_data, AssetsMarketState
 )
 
 __all__ = [
     "symbols_trades_market_state",
     "merge_assets_trades_market_states",
     "merge_symbols_trades_market_states",
     "assets_trades_market_state",
@@ -35,14 +37,20 @@
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 AssetsSides = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, str]]]]]
 SymbolsSides = Dict[str, Dict[str, List[Tuple[dt.datetime, str]]]]
 
+TRADES_ATTRIBUTES = {
+    "amounts": AMOUNT,
+    "prices": PRICE,
+    "sides": SIDE
+}
+
 @define(repr=False)
 @represent
 class TradesMarketState(MarketState, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/screeners.py` & `crypto-screening-5.7.0/crypto_screening/collect/screeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from crypto_screening.symbols import symbol_to_pair, symbol_to_parts
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature,
     exchanges_symbols
 )
 from crypto_screening.market.screeners.base import (
-    BaseScreener, BaseMultiScreener
+    BaseScreener, BaseMarketScreener
 )
 
 __all__ = [
     "matching_screener_signatures",
     "matching_screener_pair",
     "matching_screener_pairs",
     "MarketScreenerSignature",
@@ -179,29 +179,29 @@
         )
     # end for
 
     return set(pairs)
 # end matching_screener_signatures
 
 def live_screeners(
-        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]]
-) -> Set[Union[BaseScreener, BaseMultiScreener]]:
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
+) -> Set[Union[BaseScreener, BaseMarketScreener]]:
     """
     Returns a list of all the live create_screeners.
 
     :param screeners: The create_screeners to search from.
 
     :return: A list the live create_screeners.
     """
 
     return {
         screener for screener in screeners
         if (
             screener.screening and (
-                isinstance(screener, BaseMultiScreener) or
+                isinstance(screener, BaseMarketScreener) or
                 len(screener.market) > 0
             )
         )
     }
 # end live_screeners
 
 def structure_screeners(
@@ -330,15 +330,15 @@
         )
     # end for
 
     return structure
 # end structure_exchanges_symbols_screener
 
 def gather_screeners(
-        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]]
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
 ) -> List[BaseScreener]:
     """
     Gathers the base screeners.
 
     :param screeners: The screeners to process.
 
     :return: The gathered base screeners.
@@ -346,15 +346,15 @@
 
     checked_screeners: List[BaseScreener] = []
 
     for screener in screeners:
         if isinstance(screener, BaseScreener):
             checked_screeners.append(screener)
 
-        elif isinstance(screener, BaseMultiScreener):
+        elif isinstance(screener, BaseMarketScreener):
             checked_screeners.extend(screener.screeners)
         # end if
     # end for
 
     return checked_screeners
 # end gather_screeners
```

### Comparing `crypto-screening-5.6.0/crypto_screening/collect/symbols.py` & `crypto-screening-5.7.0/crypto_screening/collect/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,34 +60,42 @@
     saved = []
 
     quotes = upper_string_values(quotes or [])
     bases = upper_string_values(bases or [])
     included = upper_string_values(included or [])
 
     for symbol in symbols:
-        symbol = adjust_symbol(symbol=symbol, separator=separator)
-
         if symbol in included:
             saved.append(symbol)
+
+            continue
         # end if
 
         try:
-            base, quote = symbol_to_parts(
-                symbol=symbol, separator=separator
-            )
+            symbol = adjust_symbol(symbol=symbol, separator=separator)
 
         except ValueError as e:
             if adjust:
                 continue
 
             else:
                 raise e
             # end if
         # end try
 
+        if symbol in included:
+            saved.append(symbol)
+
+            continue
+        # end if
+
+        base, quote = symbol_to_parts(
+            symbol=symbol, separator=separator
+        )
+
         if (
             (find_string_value(value=base, values=bases) in bases) or
             (find_string_value(value=quote, values=quotes) in quotes)
         ):
             saved.append(symbol)
         # end if
     # end for
@@ -119,34 +127,36 @@
     saved = []
 
     quotes = upper_string_values(quotes or [])
     bases = upper_string_values(bases or [])
     excluded = upper_string_values(excluded or [])
 
     for symbol in symbols:
-        symbol = adjust_symbol(symbol=symbol, separator=separator)
-
         if symbol in excluded:
             continue
         # end if
 
         try:
-            base, quote = symbol_to_parts(
-                symbol=symbol, separator=separator
-            )
+            symbol = adjust_symbol(symbol=symbol, separator=separator)
 
         except ValueError as e:
             if adjust:
                 continue
 
             else:
                 raise e
             # end if
         # end try
 
+        if symbol in excluded:
+            continue
+        # end if
+
+        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+
         if (
             (find_string_value(value=base, values=bases) in bases) or
             (find_string_value(value=quote, values=quotes) in quotes)
         ):
             continue
         # end if
 
@@ -285,40 +295,40 @@
     symbols = []
 
     if separator is None:
         separator = Separator.value
     # end if
 
     for symbol in found_symbols:
-        symbol = adjust_symbol(symbol=symbol, separator=separator)
-
         try:
+            symbol = adjust_symbol(symbol=symbol, separator=separator)
+
             if symbol.count(separator) != 1:
                 raise ValueError(
                     f"Invalid symbol structure: {symbol}. "
                     f"Symbol must contain only one separator."
                 )
             # end if
 
-            base, quote = symbol_to_parts(symbol=symbol, separator=separator)
-
-            if (not test) and base.startswith("TEST") and quote.startswith("TEST"):
-                continue
-            # end if
-
-            symbols.append(symbol)
-
         except ValueError as e:
             if adjust:
                 continue
 
             else:
                 raise e
             # end if
         # end try
+
+        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+
+        if (not test) and base.startswith("TEST") and quote.startswith("TEST"):
+            continue
+        # end if
+
+        symbols.append(symbol)
     # end for
 
     return set(symbols)
 # end all_exchange_symbols
 
 def all_exchanges_symbols(
         exchanges: Iterable[str],
@@ -337,16 +347,15 @@
     :return: The data of the exchanges.
     """
 
     return {
         exchange: all_exchange_symbols(
             exchange=exchange, separator=separator,
             adjust=adjust, test=test
-        )
-        for exchange in exchanges
+        ) for exchange in exchanges
     }
 # end all_exchanges_symbols
 
 def exchange_symbols(
         exchange: Optional[str] = None,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
@@ -370,16 +379,15 @@
     """
 
     symbols = all_exchange_symbols(
         exchange=exchange, adjust=adjust, separator=separator
     )
 
     symbols = (
-        symbols
-        if all(value is None for value in (included, bases, quotes)) else
+        symbols if all(value is None for value in (included, bases, quotes)) else
         include_symbols(
             symbols=symbols, included=included,
             bases=bases, quotes=quotes, separator=separator
         )
     )
 
     return symbols if excluded is None else exclude_symbols(
@@ -519,28 +527,22 @@
     :return: The validation value for the symbols.
     """
 
     pairs = []
     exchange_symbol_pairs = []
 
     for exchange, symbols in data.items():
-        exchange_symbol_pairs.extend(
-            [(exchange, symbol) for symbol in symbols]
-        )
+        exchange_symbol_pairs.extend([(exchange, symbol) for symbol in symbols])
     # end for
 
     for exchange1, symbol1 in exchange_symbol_pairs:
         for exchange2, symbol2 in exchange_symbol_pairs:
             exchanges_matches = (
-                matches
-                if not isinstance(matches, dict) else
-                [
-                    *matches.get(exchange1, []),
-                    *matches.get(exchange2, [])
-                ]
+                matches if not isinstance(matches, dict) else
+                [*matches.get(exchange1, []), *matches.get(exchange2, [])]
             )
 
             if (
                 (exchange1 != exchange2) and
                 matching_symbol_pair(
                     symbol1, symbol2,
                     matches=exchanges_matches or None,
```

### Comparing `crypto-screening-5.6.0/crypto_screening/dataset.py` & `crypto-screening-5.7.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/interval.py` & `crypto-screening-5.7.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/market/dynamic.py` & `crypto-screening-5.7.0/crypto_screening/market/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,32 +23,32 @@
 from crypto_screening.collect.market.trades import (
     assets_trades_market_state, symbols_trades_market_state,
     SymbolsTradesMarketState, AssetsTradesMarketState
 )
 from crypto_screening.market.screeners.container import ScreenersContainer
 
 __all__ = [
-    "DynamicScreener"
+    "DynamicScreenerContainer"
 ]
 
-class DynamicScreener(ScreenersContainer):
+class DynamicScreenerContainer(ScreenersContainer):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects.
 
-    >>> from crypto_screening.market.dynamic import DynamicScreener
+    >>> from crypto_screening.market.dynamic import DynamicScreenerContainer
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
-    >>> dynamic_screener = DynamicScreener(
+    >>> dynamic_screener = DynamicScreenerContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
     >>> dynamic_screener.find_screener(exchange="binance", symbol="BTC/USDT"))
     >>> dynamic_screener.data(exchange="binance", symbol="BTC/USDT", length=10))
     """
 
@@ -508,8 +508,8 @@
             included=included, excluded=excluded, adjust=adjust
         )
 
         return symbols_orders_market_state(
             screeners=screeners, length=length, adjust=adjust
         )
     # end symbols_orders_market_state
-# end DynamicScreener
+# end DynamicScreenerContainer
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/foundation/data.py` & `crypto-screening-5.7.0/crypto_screening/market/foundation/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,27 @@
 import warnings
 import datetime as dt
 import time
 from abc import ABCMeta, abstractmethod
 import threading
 from typing import Optional, Union, Dict, Any
 
-from represent import represent, Modifiers
+from represent import represent
 
 
 from crypto_screening.market.foundation.state import WaitingState
 
 __all__ = [
     "DataCollector"
 ]
 
 @represent
 class DataCollector(metaclass=ABCMeta):
     """A class to represent an abstract parent class of data collectors."""
 
-    __modifiers__ = Modifiers()
-    __modifiers__.excluded.extend(
-        [
-            'screening_process', 'timeout_process',
-            'saving_process', 'update_process'
-        ]
-    )
-
     __slots__ = (
         '_screening_process', '_timeout_process',
         '_saving_process', '_update_process',
         '_updating', '_saving', '_blocking',
         '_screening', "location", "delay", "cancel"
     )
 
@@ -68,18 +60,18 @@
         self.location = location or self.LOCATION
 
         self._screening = False
         self._blocking = False
         self._saving = False
         self._updating = False
 
-        self._screening_process = None
-        self._timeout_process = None
-        self._saving_process = None
-        self._update_process = None
+        self._screening_process: Optional[threading.Thread] = None
+        self._timeout_process: Optional[threading.Thread] = None
+        self._saving_process: Optional[threading.Thread] = None
+        self._update_process: Optional[threading.Thread] = None
     # end __init__
 
     def __getstate__(self) -> Dict[str, Any]:
         """
         Returns the data of the object.
 
         :return: The state of the object.
@@ -149,15 +141,15 @@
     # end saving_loop
 
     def update_loop(self) -> None:
         """Updates the state of the screeners."""
     # end update_loop
 
     @abstractmethod
-    def wait_for_initialization(
+    def await_initialization(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
     ) -> WaitingState:
         """
         Waits for all the create_screeners to update.
@@ -167,15 +159,15 @@
         :param cancel: The time to cancel the waiting.
 
         :returns: The total delay.
         """
     # end base_wait_for_initialization
 
     @abstractmethod
-    def wait_for_update(
+    def await_update(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
     ) -> WaitingState:
         """
         Waits for all the create_screeners to update.
@@ -268,15 +260,15 @@
         # end if
 
         if isinstance(wait, dt.timedelta):
             wait = wait.total_seconds()
         # end if
 
         if isinstance(wait, bool) and wait:
-            self.wait_for_initialization()
+            self.await_initialization()
 
         elif isinstance(wait, (int, float)):
             time.sleep(wait)
         # end if
     # end start_waiting
 
     def start_timeout(
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.7.0/crypto_screening/market/foundation/protocols.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # protocols.py
 
 import datetime as dt
-from typing import Protocol, Dict, List, Union
+from typing import Protocol, List, Union
 
 import pandas as pd
 
 __all__ = [
     "BaseScreenerProtocol",
-    "BaseMultiScreenerProtocol",
+    "BaseMarketScreenerProtocol",
     "DataCollectorProtocol"
 ]
 
 class DataCollectorProtocol(Protocol):
     """A class for the base data collector protocol."""
 
     location: str
@@ -25,13 +25,12 @@
 
     symbol: str
     exchange: str
 
     market: pd.DataFrame
 # end BaseScreenerProtocol
 
-class BaseMultiScreenerProtocol(DataCollectorProtocol):
+class BaseMarketScreenerProtocol(DataCollectorProtocol):
     """A class for the base multi-screener protocol."""
 
-    market: Dict[str, Dict[str, pd.DataFrame]]
     screeners: List[BaseScreenerProtocol]
-# end BaseMultiScreenerProtocol
+# end BaseMarketScreenerProtocol
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/foundation/state.py` & `crypto-screening-5.7.0/crypto_screening/market/foundation/state.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,37 +6,30 @@
 )
 
 from attrs import define
 
 from represent import represent, Modifiers
 
 from crypto_screening.market.foundation.protocols import (
-    BaseScreenerProtocol, BaseMultiScreenerProtocol, DataCollectorProtocol
+    BaseScreenerProtocol, BaseMarketScreenerProtocol
 )
 
 __all__ = [
     "WaitingState"
 ]
 
 
-_BS = TypeVar("_BS")
+_BS = TypeVar("_BS", BaseScreenerProtocol, BaseMarketScreenerProtocol)
 
 @define(repr=False)
 @represent
 class WaitingState(Generic[_BS]):
     """A class to represent the waiting state of screener objects."""
 
-    screeners: Iterable[
-        Union[
-            _BS,
-            BaseScreenerProtocol,
-            BaseMultiScreenerProtocol,
-            DataCollectorProtocol
-        ]
-    ]
+    screeners: Iterable[_BS]
     start: dt.datetime
     end: dt.datetime
     stop: Optional[bool] = False
     delay: Optional[float] = 0
     count: Optional[int] = 0
     canceled: Optional[bool] = False
     cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.7.0/crypto_screening/market/foundation/waiting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # waiting.py
 
 import datetime as dt
 import time
 from typing import (
-    Optional, Union, Iterable, Callable, Any
+    Optional, Union, Iterable, Callable, TypeVar
 )
 
-from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.data import DataCollector
+from crypto_screening.market.foundation.state import WaitingState
+from crypto_screening.market.foundation.protocols import (
+    BaseScreenerProtocol, BaseMarketScreenerProtocol
+)
 
 __all__ = [
-    "base_wait_for_update",
-    "base_wait_for_initialization",
-    "base_wait_for_dynamic_update",
-    "base_wait_for_dynamic_initialization"
+    "base_await_update",
+    "base_await_initialization",
+    "base_await_dynamic_update",
+    "base_await_dynamic_initialization"
 ]
 
-Gatherer = Callable[[Iterable[Any]], Iterable[Any]]
 
-def base_wait_for_dynamic_initialization(
-        screeners: Iterable[DataCollector],
+_BS = TypeVar("_BS", BaseScreenerProtocol, BaseMarketScreenerProtocol, DataCollector)
+
+Gatherer = Callable[[Iterable[_BS]], Iterable[_BS]]
+
+def base_await_dynamic_initialization(
+        screeners: Iterable[_BS],
         stop: Optional[bool] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
         gatherer: Optional[Gatherer] = None
-) -> WaitingState[DataCollector]:
+) -> WaitingState[_BS]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
@@ -91,53 +97,53 @@
 
     if stop:
         for screener in screeners:
             screener.stop()
         # end for
     # end if
 
-    return WaitingState(
+    return WaitingState[_BS](
         screeners=screeners, delay=delay,
         count=count, end=dt.datetime.now(), start=start,
         cancel=cancel, canceled=canceled
     )
-# end base_wait_for_dynamic_initialization
+# end base_await_dynamic_initialization
 
-def base_wait_for_initialization(
-        *screeners: DataCollector,
+def base_await_initialization(
+        *screeners: _BS,
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
         gatherer: Optional[Gatherer] = None
-) -> WaitingState[DataCollector]:
+) -> WaitingState[_BS]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
     :param gatherer: The gathering callable to gather the screeners.
 
     :returns: The total delay.
     """
 
-    return base_wait_for_dynamic_initialization(
+    return base_await_dynamic_initialization(
         screeners, delay=delay, stop=stop,
         cancel=cancel, gatherer=gatherer
     )
-# end base_wait_for_initialization
+# end base_await_initialization
 
-def base_wait_for_dynamic_update(
-        screeners: Iterable[DataCollector],
+def base_await_dynamic_update(
+        screeners: Iterable[_BS],
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
         gatherer: Optional[Gatherer] = None
-) -> WaitingState[DataCollector]:
+) -> WaitingState[_BS]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
@@ -162,15 +168,15 @@
         delay = delay.total_seconds()
     # end if
 
     start = dt.datetime.now()
     count = 0
     canceled = False
 
-    wait = base_wait_for_dynamic_initialization(
+    wait = base_await_dynamic_initialization(
         screeners, delay=delay, cancel=cancel, stop=stop
     )
 
     if not screeners:
         return wait
     # end if
 
@@ -211,38 +217,38 @@
 
     if stop:
         for screener in screeners:
             screener.stop()
         # end for
     # end if
 
-    return WaitingState(
+    return WaitingState[_BS](
         screeners=screeners, delay=delay,
         count=count, end=dt.datetime.now(), start=start,
         cancel=cancel, canceled=canceled
     )
-# end base_wait_for_dynamic_update
+# end base_await_dynamic_update
 
-def base_wait_for_update(
-        *screeners: DataCollector,
+def base_await_update(
+        *screeners: _BS,
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
         gatherer: Optional[Gatherer] = None
-) -> WaitingState[DataCollector]:
+) -> WaitingState[_BS]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
     :param gatherer: The gathering callable to gather the screeners.
 
     :returns: The total delay.
     """
 
-    return base_wait_for_dynamic_update(
+    return base_await_dynamic_update(
         screeners, delay=delay, stop=stop,
         cancel=cancel, gatherer=gatherer
     )
-# end base_wait_for_update
+# end base_await_update
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/base.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 import pandas as pd
 
 from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import save_dataset, load_dataset
-from crypto_screening.symbols import Separator
+from crypto_screening.symbols import Separator, adjust_symbol
 from crypto_screening.validate import validate_exchange, validate_symbol
+from crypto_screening.collect.symbols import all_exchange_symbols
 from crypto_screening.market.foundation.state import WaitingState
+from crypto_screening.market.foundation.data import DataCollector
+from crypto_screening.market.foundation.protocols import BaseScreenerProtocol
 from crypto_screening.market.foundation.waiting import (
-    base_wait_for_initialization, base_wait_for_dynamic_initialization,
-    base_wait_for_dynamic_update, base_wait_for_update
+    base_await_initialization, base_await_dynamic_initialization,
+    base_await_dynamic_update, base_await_update
 )
-from crypto_screening.market.foundation.data import DataCollector
 
 __all__ = [
     "BaseScreener",
-    "BaseMultiScreener"
+    "BaseMarketScreener"
 ]
 
 class BaseScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
@@ -84,62 +86,64 @@
         :param cancel: The cancel time for the loops.
         :param market: The data for the market.
         """
 
         super().__init__(location=location, cancel=cancel, delay=delay)
 
         self.exchange = self.validate_exchange(exchange=exchange)
-        self.symbol = self.validate_symbol(
-            exchange=self.exchange, symbol=symbol
-        )
+        self.symbol = self.validate_symbol(exchange=self.exchange, symbol=symbol)
 
         self.market = market
     # end __init__
 
-    def wait_for_initialization(
+    def await_initialization(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
+    ) -> WaitingState[BaseScreenerProtocol]:
         """
         Waits for all the create_screeners to update.
 
         :param delay: The delay for the waiting.
         :param stop: The value to stop the screener objects.
         :param cancel: The time to cancel the waiting.
 
         :returns: The total delay.
         """
 
-        return base_wait_for_initialization(
+        self: Union[BaseScreener, BaseScreenerProtocol]
+
+        return base_await_initialization(
             self, stop=stop, delay=delay, cancel=cancel
         )
-    # end base_wait_for_initialization
+    # end await_initialization
 
-    def wait_for_update(
+    def await_update(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
+    ) -> WaitingState[BaseScreenerProtocol]:
         """
         Waits for all the create_screeners to update.
 
         :param delay: The delay for the waiting.
         :param stop: The value to stop the screener objects.
         :param cancel: The time to cancel the waiting.
 
         :returns: The total delay.
         """
 
-        return base_wait_for_update(
+        self: Union[BaseScreener, BaseScreenerProtocol]
+
+        return base_await_update(
             self, stop=stop, delay=delay, cancel=cancel
         )
-    # end base_wait_for_update
+    # end await_update
 
     @staticmethod
     def validate_exchange(exchange: str) -> str:
         """
         Validates the symbol value.
 
         :param exchange: The exchange name.
@@ -157,15 +161,18 @@
 
         :param exchange: The exchange name.
         :param symbol: The name of the symbol.
 
         :return: The validates symbol.
         """
 
-        return validate_symbol(exchange=exchange, symbol=symbol)
+        return validate_symbol(
+            exchange=exchange, symbol=symbol,
+            symbols=all_exchange_symbols(exchange=exchange)
+        )
     # end validate_symbol
 
     def dataset_path(self, location: Optional[str] = None) -> str:
         """
         Creates the path to the saving file for the screener object.
 
         :param location: The saving location of the dataset.
@@ -178,15 +185,15 @@
         if location is None:
             location = "."
         # end if
 
         return (
             f"{location}/"
             f"{self.exchange.lower()}/"
-            f"{self.symbol.replace(Separator.value, '-')}.csv"
+            f"{adjust_symbol(self.symbol).replace(Separator.value, '-')}.csv"
         )
     # end dataset_path
 
     def save_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -236,15 +243,15 @@
             end = time.time()
 
             time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
         # end while
     # end saving_loop
 # end BaseScreener
 
-class BaseMultiScreener(DataCollector):
+class BaseMarketScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -254,14 +261,17 @@
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
+
+    - screeners:
+        The screener object to control and fill with data.
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.extend(["screeners", 'recorder'])
 
     screeners: List[BaseScreener]
 
@@ -283,55 +293,55 @@
         """
 
         super().__init__(location=location, cancel=cancel, delay=delay)
 
         self.screeners = list(screeners or [])
     # end __init__
 
-    def wait_for_initialization(
+    def await_initialization(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
+    ) -> WaitingState[BaseScreener]:
         """
         Waits for all the create_screeners to update.
 
         :param delay: The delay for the waiting.
         :param stop: The value to stop the screener objects.
         :param cancel: The time to cancel the waiting.
 
         :returns: The total delay.
         """
 
-        return base_wait_for_dynamic_initialization(
+        return base_await_dynamic_initialization(
             self.screeners, stop=stop, delay=delay, cancel=cancel
         )
-    # end base_wait_for_initialization
+    # end await_initialization
 
-    def wait_for_update(
+    def await_update(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
+    ) -> WaitingState[BaseScreener]:
         """
         Waits for all the create_screeners to update.
 
         :param delay: The delay for the waiting.
         :param stop: The value to stop the screener objects.
         :param cancel: The time to cancel the waiting.
 
         :returns: The total delay.
         """
 
-        return base_wait_for_dynamic_update(
+        return base_await_dynamic_update(
             self.screeners, stop=stop, delay=delay, cancel=cancel
         )
-    # end base_wait_for_update
+    # end await_update
 
     def save_datasets(self, location: Optional[str] = None) -> None:
         """
         Runs the data handling loop.
 
         :param location: The saving location.
         """
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/combined.py`

 * *Files 11% similar despite different names*

```diff
@@ -135,25 +135,20 @@
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
+    - recorders:
+        The Recorder objects to contron and collect data from, into the markets.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_recorder
+    >>> from crypto_screening.market.screeners import CombinedMarketRecorder
     >>>
-    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
-    >>>
-    >>> recorder = orderbook_market_recorder(data=market)
+    >>> recorder = CombinedMarketRecorder(...)
     """
 
     def __init__(self, recorders: Iterable[Recorder]) -> None:
         """
         Defines the class attributes.
 
         :param recorders: The categories for the market screener.
@@ -273,19 +268,31 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_screener
+    - screeners:
+        The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
+    >>> from crypto_screening.market.screeners import combined_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener = orderbook_market_screener(data=structure)
+    >>> screener = combined_market_screener(data=structure)
     >>> screener.run()
     """
 
     recorder: CombinedMarketRecorder
 
     def __init__(
             self,
@@ -415,29 +422,27 @@
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         amount: Optional[int] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrderbookMarketRecorder] = None,
         fixed: Optional[bool] = True,
-        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> CombinedMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param categories: The categories for the markets.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
     :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
-    :param separator: The separator of the assets.
     :param databases: The paths to the databases.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
 
     :return: The market screener object.
@@ -448,25 +453,24 @@
     # end if
 
     markets = [
         CATEGORY_RECORDER_CONSTRUCTOR_MATCHES[category](
             recorder=recorder, handler=handler, data=data,
             location=location, amount=amount, cancel=cancel,
             delay=delay, limited=limited, refresh=refresh,
-            fixed=fixed, separator=separator, parameters=parameters,
-            databases=databases
+            fixed=fixed, parameters=parameters, databases=databases
         ) for category in set(categories)
     ]
 
     screener = CombinedMarketScreener(
         markets=markets, recorder=recorder, handler=handler,
         location=location, amount=amount, cancel=cancel,
         delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
-        data=screener.recorder.structure(), fixed=fixed,
-        separator=separator, parameters=parameters
+        data=screener.recorder.structure(),
+        fixed=fixed, parameters=parameters
     )
 
     return screener
 # end combined_market_screener
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/container.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.market.screeners.orders import OrdersScreener
 
-_S = TypeVar("_S")
+_S = TypeVar(
+    "_S",
+    BaseScreener,
+    OHLCVScreener,
+    OrderbookScreener,
+    TradesScreener,
+    OrdersScreener
+)
 
 class ScreenersContainer(MarketRecorder):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/database/data.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/database/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,18 +180,25 @@
     table = parts_database_table_name(
         name=name, exchange=exchange,
         symbol=symbol, interval=interval
     )
 
     query = 'SELECT COUNT(' + DATE_TIME + ') FROM ' + table
 
-    return {
-        path: engine.connect().execute(text(query)).all()[0][0]
-        for path, engine in databases.items()
-    }
+    results: Dict[str, int] = {}
+
+    for path, engine in databases.items():
+        connection = engine.connect()
+
+        results[path] = connection.execute(text(query)).all()[0][0]
+
+        connection.close()
+    # end for
+
+    return results
 # end extract_database_length
 
 def extract_database_record(
         name: str,
         exchange: str,
         symbol: str,
         databases: Dict[str, Engine],
@@ -225,16 +232,16 @@
             length_query = f" WHERE DateTime > {start}"
 
         else:
             length_query = f'COUNT(*) - {length}'
         # end if
 
         query += (
-                f' LIMIT {length} OFFSET '
-                f'(SELECT {length_query} FROM  ' + table + ')'
+            f' LIMIT {length} OFFSET '
+            f'(SELECT {length_query} FROM  ' + table + ')'
         )
 
     elif isinstance(start, int) and (start > 0):
         query += f' WHERE DateTime > {start}'
     # end if
 
     return {
@@ -257,17 +264,15 @@
     :param path: The path to the database.
     :param engine: The database engine.
     :param length: The length of data to extract.
     :param start: The start index.
     """
 
     interval = (
-        screener.interval
-        if (screener.NAME == "OHLCV") else
-        None
+        screener.interval if (screener.NAME == "OHLCV") else None
     )
 
     data = extract_database_record(
         name=screener.NAME, exchange=screener.exchange,
         symbol=screener.symbol, interval=interval, start=start,
         length=length, databases={path: engine}
     )[path]
@@ -320,15 +325,15 @@
     data = data or []
 
     if not isinstance(data, dict):
         data = {path: create_engine(path) for path in data}
     # end if
 
     if not all(
-            isinstance(path, str) and isinstance(engine, Engine)
-            for path, engine in data.items()
+        isinstance(path, str) and isinstance(engine, Engine)
+        for path, engine in data.items()
     ):
         raise ValueError(f"databases must be: {Databases}, not: {data}")
     # end if
 
     return data
 # end validate_database_engines
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/database/execution.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/database/execution.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,18 +604,28 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
+
+    - ohlcv_market:
+        The OHLCV market structure of the data to store the fetched data in.
+        This structure is a dictionary with exchange names as keys
+        and dictionaries as values, where their keys are symbols,
+        and their values are the dataframes to record the data.
+
     - intervals:
         The structure to set a specific interval to the dataset
         of each symbol in each exchange, matching the market data.
 
+    - databases:
+        The databases and their engines for storing data in databases.
+
     >>> from crypto_screening.market.screeners import ohlcv_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': {'1m': 'ETH/USDT'}}
     >>>
     >>> recorder = ohlcv_market_recorder(data=market)
     """
 
@@ -853,14 +863,26 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
+    - screeners:
+        The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
     >>> from crypto_screening.market.screeners import ohlcv_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = ohlcv_market_screener(data=structure)
     >>> screener.run()
     """
@@ -1150,15 +1172,14 @@
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         amount: Optional[int] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OHLCVMarketRecorder] = None,
         fixed: Optional[bool] = True,
-        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OHLCVMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
@@ -1166,15 +1187,14 @@
     :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
     :param intervals: The intervals for the datasets.
     :param ohlcv_market: The OHLCV market structure.
     :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
-    :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
 
     :return: The market screener object.
@@ -1193,13 +1213,13 @@
             intervals=intervals, databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
-        data=screener.recorder.structure(), fixed=fixed,
-        separator=separator, parameters=parameters
+        data=screener.recorder.structure(),
+        fixed=fixed, parameters=parameters
     )
 
     return screener
 # end orderbook_market_recorder
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 5% similar despite different names*

```diff
@@ -240,14 +240,17 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
+    - databases:
+        The databases and their engines for storing data in databases.
+
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
@@ -347,14 +350,26 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
+    - screeners:
+        The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
     >>> from crypto_screening.market.screeners import orderbook_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = orderbook_market_screener(data=structure)
     >>> screener.run()
     """
@@ -573,29 +588,27 @@
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrderbookMarketRecorder] = None,
         fixed: Optional[bool] = True,
-        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OrderbookMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
     :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
-    :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
 
     :return: The market screener object.
@@ -607,13 +620,13 @@
             databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
-        data=screener.recorder.structure(), fixed=fixed,
-        separator=separator, parameters=parameters
+        data=screener.recorder.structure(),
+        fixed=fixed, parameters=parameters
     )
 
     return screener
 # end orderbook_market_recorder
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,17 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
+    - databases:
+        The databases and their engines for storing data in databases.
+
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
@@ -342,19 +345,31 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_screener
+    - screeners:
+        The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
+    >>> from crypto_screening.market.screeners import orders_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener = orderbook_market_screener(data=structure)
+    >>> screener = orders_market_screener(data=structure)
     >>> screener.run()
     """
 
     screeners: List[OrdersScreener]
     recorder: OrdersMarketRecorder
 
     COLUMNS = OrdersMarketRecorder.COLUMNS
@@ -568,29 +583,27 @@
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         databases: Optional[Databases] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[OrdersMarketRecorder] = None,
         fixed: Optional[bool] = True,
-        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> OrdersMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
     :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
-    :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
 
     :return: The market screener object.
@@ -602,13 +615,13 @@
             databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
-        data=screener.recorder.structure(), fixed=fixed,
-        separator=separator, parameters=parameters
+        data=screener.recorder.structure(),
+        fixed=fixed, parameters=parameters
     )
 
     return screener
 # end orders_market_screener
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/recorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 from cryptofeed import FeedHandler
 from cryptofeed.feed import Feed
 
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
-from crypto_screening.symbols import Separator
+from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.database.data import validate_database_engines
-from crypto_screening.market.screeners.base import BaseMultiScreener, BaseScreener
+from crypto_screening.market.screeners.base import BaseMarketScreener, BaseScreener
 
 __all__ = [
     "MarketHandler",
     "ExchangeFeed",
     "FEED_GROUP_SIZE",
     "add_feeds",
     "MarketScreener",
@@ -84,49 +84,40 @@
 FEED_GROUP_SIZE = 20
 
 def add_feeds(
         handler: FeedHandler,
         data: Dict[str, Iterable[str]],
         fixed: Optional[bool] = False,
         amount: Optional[int] = FEED_GROUP_SIZE,
-        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> None:
     """
     Adds the symbols to the handler for each exchange.
 
     :param handler: The handler object.
     :param data: The data of the exchanges and symbols to add.
     :param parameters: The parameters for the exchanges.
     :param fixed: The value for fixed parameters to all exchanges.
-    :param separator: The separator of the assets.
     :param amount: The maximum amount of symbols for each feed.
     """
 
     base_parameters = None
 
     if not fixed:
         parameters = parameters or {}
 
     else:
         base_parameters = parameters or {}
         parameters = {}
     # end if
 
-    if separator is None:
-        separator = Separator.value
-    # end if
-
     for exchange, symbols in data.items():
         exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
 
-        symbols = [
-            symbol.replace(separator, '-')
-            for symbol in symbols
-        ]
+        symbols = [adjust_symbol(symbol, separator='-') for symbol in symbols]
 
         if fixed:
             parameters.setdefault(exchange, base_parameters)
         # end if
 
         EXCHANGES[exchange]: Type[ExchangeFeed]
 
@@ -214,14 +205,17 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
+    - databases:
+        The databases and their engines for storing data in databases.
+
     >>> from crypto_screening.market.screeners.recorder import MarketRecorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = MarketRecorder(data=market)
 
     """
@@ -360,15 +354,15 @@
 
         except ValueError:
             return False
         # end try
     # end in_market
 # end MarketRecorder
 
-class MarketScreener(BaseMultiScreener):
+class MarketScreener(BaseMarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -384,17 +378,29 @@
         The delay to wait between each data fetching.
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
+
+    - screeners:
+        The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
     """
 
-    __modifiers__ = Modifiers(**BaseMultiScreener.__modifiers__)
+    __modifiers__ = Modifiers(**BaseMarketScreener.__modifiers__)
     __modifiers__.excluded.append('handler')
 
     __slots__ = (
         "handler", 'amount', "loop", "limited", "_feeds_parameters",
         "_run_parameters", 'refresh'
     )
 
@@ -466,42 +472,39 @@
         return self.recorder.structure()
     # end structure
 
     def add_feeds(
             self,
             data: Optional[Dict[str, Iterable[str]]] = None,
             fixed: Optional[bool] = True,
-            separator: Optional[str] = None,
             amount: Optional[int] = None,
             parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
     ) -> None:
         """
         Adds the symbols to the handler for each exchange.
 
         :param data: The data of the exchanges and symbols to add.
         :param parameters: The parameters for the exchanges.
         :param fixed: The value for fixed parameters to all exchanges.
         :param amount: The maximum amount of symbols for each feed.
-        :param separator: The separator of the assets.
         """
 
         if data is None:
             data = self.structure()
         # end if
 
         self._feeds_parameters = dict(
-            data=data, fixed=fixed, separator=separator,
-            parameters=parameters
+            data=data, fixed=fixed, parameters=parameters
         )
 
         feed_params = self.recorder.parameters()
         feed_params.update(parameters or {})
 
         add_feeds(
-            self.handler, data=data, fixed=fixed, separator=separator,
+            self.handler, data=data, fixed=fixed,
             parameters=feed_params, amount=amount or self.amount
         )
     # end add_feeds
 
     def refresh_feeds(self) -> None:
         """Refreshes the feed objects."""
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.7.0/crypto_screening/market/screeners/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,17 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
+    - databases:
+        The databases and their engines for storing data in databases.
+
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
@@ -343,19 +346,31 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_screener
+    - screeners:
+        The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
+    >>> from crypto_screening.market.screeners import trades_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener = orderbook_market_screener(data=structure)
+    >>> screener = trades_market_screener(data=structure)
     >>> screener.run()
     """
 
     screeners: List[TradesScreener]
     recorder: TradesMarketRecorder
 
     COLUMNS = TradesMarketRecorder.COLUMNS
@@ -569,29 +584,27 @@
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         databases: Optional[Databases] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[TradesMarketRecorder] = None,
         fixed: Optional[bool] = True,
-        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> TradesMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
     :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
-    :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param databases: The paths to the databases.
 
     :return: The market screener object.
@@ -603,13 +616,13 @@
             databases=databases
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
-        data=screener.recorder.structure(), fixed=fixed,
-        separator=separator, parameters=parameters
+        data=screener.recorder.structure(),
+        fixed=fixed, parameters=parameters
     )
 
     return screener
 # end trades_market_screener
```

### Comparing `crypto-screening-5.6.0/crypto_screening/market/waiting.py` & `crypto-screening-5.7.0/crypto_screening/market/waiting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# dynamic.py
+# waiting.py
 
 import datetime as dt
 from typing import (
     Optional, Union, Iterable
 )
 
 from crypto_screening.collect.screeners import gather_screeners
-from crypto_screening.market.screeners import BaseScreener, BaseMultiScreener
+from crypto_screening.market.screeners import BaseScreener, BaseMarketScreener
 from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.waiting import (
-    base_wait_for_update, base_wait_for_dynamic_initialization,
-    base_wait_for_initialization, base_wait_for_dynamic_update
+    base_await_update, base_await_dynamic_initialization,
+    base_await_initialization, base_await_dynamic_update
 )
 
 __all__ = [
-    "wait_for_dynamic_initialization",
-    "wait_for_update",
-    "wait_for_initialization",
-    "wait_for_dynamic_update",
+    "await_dynamic_initialization",
+    "await_update",
+    "await_initialization",
+    "await_dynamic_update",
     "WaitingState"
 ]
 
-def wait_for_dynamic_initialization(
-        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]],
+def await_dynamic_initialization(
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]],
         stop: Optional[bool] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
 ) -> WaitingState:
     """
     Waits for all the create_screeners to update.
 
@@ -34,22 +34,22 @@
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
 
     :returns: The total delay.
     """
 
-    return base_wait_for_dynamic_initialization(
+    return base_await_dynamic_initialization(
         screeners=screeners, stop=stop, delay=delay,
         cancel=cancel, gatherer=gather_screeners
     )
-# end wait_for_dynamic_initialization
+# end await_dynamic_initialization
 
-def wait_for_initialization(
-        *screeners: Union[BaseScreener, BaseMultiScreener],
+def await_initialization(
+        *screeners: Union[BaseScreener, BaseMarketScreener],
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
 ) -> WaitingState:
     """
     Waits for all the create_screeners to update.
 
@@ -57,22 +57,22 @@
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
 
     :returns: The total delay.
     """
 
-    return base_wait_for_initialization(
+    return base_await_initialization(
         *screeners, stop=stop, delay=delay,
         cancel=cancel, gatherer=gather_screeners
     )
-# end wait_for_initialization
+# end await_initialization
 
-def wait_for_dynamic_update(
-        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]],
+def await_dynamic_update(
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]],
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
 ) -> WaitingState:
     """
     Waits for all the create_screeners to update.
 
@@ -80,22 +80,22 @@
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
 
     :returns: The total delay.
     """
 
-    return base_wait_for_dynamic_update(
+    return base_await_dynamic_update(
         screeners=screeners, stop=stop, delay=delay,
         cancel=cancel, gatherer=gather_screeners
     )
-# end wait_for_dynamic_update
+# end await_dynamic_update
 
-def wait_for_update(
-        *screeners: Union[BaseScreener, BaseMultiScreener],
+def await_update(
+        *screeners: Union[BaseScreener, BaseMarketScreener],
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
 ) -> WaitingState:
     """
     Waits for all the create_screeners to update.
 
@@ -103,12 +103,12 @@
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
 
     :returns: The total delay.
     """
 
-    return base_wait_for_update(
+    return base_await_update(
         *screeners, stop=stop, delay=delay,
         cancel=cancel, gatherer=gather_screeners
     )
-# end wait_for_update
+# end await_update
```

### Comparing `crypto-screening-5.6.0/crypto_screening/process.py` & `crypto-screening-5.7.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/crypto_screening/symbols.py` & `crypto-screening-5.7.0/crypto_screening/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,31 @@
     :return: The adjusted asset symbol.
     """
 
     if separator is None:
         separator = Separator.value
     # end if
 
-    return symbol.replace("-", separator).upper()
+    saved = symbol
+
+    for char in "\"!@#$%^&*()_+-=+,.|:`~/\\'":
+        symbol = symbol.replace(char, " ")
+    # end for
+
+    parts = [part.upper() for part in symbol.split(" ") if part]
+
+    try:
+        return parts_to_symbol(*parts, separator=separator)
+
+    except TypeError:
+        raise ValueError(
+            f"Cannot adjust symbol: {saved} "
+            f"with separator: {separator}."
+        )
+    # end try
 # end adjust_symbol
 
 def symbols_to_parts(symbols: Dict[str, Dict[str, Any]]) -> Tuple[List[str], List[str]]:
     """
     Collects the bases and quotes of the symbols.
 
     :param symbols: The symbols to separate.
```

### Comparing `crypto-screening-5.6.0/crypto_screening/validate.py` & `crypto-screening-5.7.0/crypto_screening/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,48 @@
 # validate.py
 
 from typing import Optional, Iterable, Any
 
 from crypto_screening.process import find_string_value
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.interval import interval_to_total_time
-from crypto_screening.exchanges import EXCHANGE_NAMES, EXCHANGES
+from crypto_screening.exchanges import EXCHANGE_NAMES
 
 __all__ = [
     "is_valid_symbol",
     "validate_exchange",
     "validate_symbol",
     "is_valid_exchange",
     "validate_interval"
 ]
 
-def is_valid_symbol(
-        exchange: str,
-        symbol: str,
-        exchanges: Optional[Iterable[str]] = None,
-        symbols: Optional[Iterable[str]] = None
-) -> bool:
+def is_valid_symbol(symbol: str, symbols: Iterable[str]) -> bool:
     """
     Returns a value for the symbol being valid for the source exchange.
 
-    :param exchange: The name of the exchange platform.
     :param symbol: The symbol of the assets.
     :param symbols: The valid symbols.
-    :param exchanges: The valid exchanges.
 
     :return: The validation-value.
     """
 
-    if symbols is None:
-        exchange = find_string_value(
-            value=exchange, values=EXCHANGE_NAMES
-        )
-
-        if not is_valid_exchange(
-                exchange=exchange, exchanges=exchanges
-        ):
-            return False
-        # end if
-
-        symbols = EXCHANGES[exchange].symbols()
-    # end for
-
     symbols = [adjust_symbol(symbol=s) for s in symbols]
 
     symbol = find_string_value(
         value=adjust_symbol(symbol=symbol), values=symbols
     )
 
     return symbol in symbols
 # end is_valid_symbol
 
 def validate_symbol(
         exchange: str,
         symbol: str,
+        symbols: Iterable[str],
         exchanges: Optional[Iterable[str]] = None,
-        symbols: Optional[Iterable[str]] = None,
         provider: Optional[Any] = None
 ) -> str:
     """
     Returns a value for the symbol being valid for the source exchange.
 
     :param exchange: The name of the exchange platform.
     :param symbol: The symbol of the assets.
@@ -71,21 +50,18 @@
     :param exchanges: The valid exchanges.
     :param provider: Any provider object.
 
     :return: The validation-value.
     """
 
     validate_exchange(
-        exchange=exchange, exchanges=exchanges,
-        provider=provider
+        exchange=exchange, exchanges=exchanges, provider=provider
     )
 
-    if not is_valid_symbol(
-            exchange=exchange, symbol=symbol, symbols=symbols
-    ):
+    if not is_valid_symbol(symbol=symbol, symbols=symbols):
         raise ValueError(
             f"'{symbol}' is not a valid "
             f"symbol for the '{exchange}' exchange. "
             f"Valid symbols: {', '.join(symbols or [])}"
             f"{f' for {repr(provider)}.' if provider else ''}"
         )
     # end if
```

### Comparing `crypto-screening-5.6.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.7.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.6.0
+Version: 5.7.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.6.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.7.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.6.0/pyproject.toml` & `crypto-screening-5.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.6.0'
+version = '5.7.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.6.0/setup.py` & `crypto-screening-5.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.6.0',
+        version='5.7.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

