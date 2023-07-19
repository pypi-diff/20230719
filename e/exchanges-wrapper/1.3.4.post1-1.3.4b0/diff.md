# Comparing `tmp/exchanges_wrapper-1.3.4.post1.tar.gz` & `tmp/exchanges-wrapper-1.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-1.3.4.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges-wrapper-1.3.4b0.tar", last modified: Sun Jul 16 16:11:52 2023, max compression
```

## Comparing `exchanges_wrapper-1.3.4.post1.tar` & `exchanges-wrapper-1.3.4b0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
--rw-r--r--   0        0        0     1114 2023-07-19 14:05:09.675815 exchanges_wrapper-1.3.4.post1/LICENSE.md
--rw-r--r--   0        0        0     7068 2023-07-19 14:05:09.675815 exchanges_wrapper-1.3.4.post1/README.md
--rw-r--r--   0        0        0     1320 2023-07-19 14:05:09.675815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    25161 2023-07-19 14:05:09.675815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-07-19 14:05:09.675815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19607 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6184 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    61866 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12485 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    47673 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4429 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10260 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15715 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16089 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22397 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1181 2023-07-19 14:05:09.679815 exchanges_wrapper-1.3.4.post1/pyproject.toml
--rw-r--r--   0        0        0     8028 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.4.post1/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.4b0/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.4b0/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.4b0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.4b0/.github/dependabot.yml
+-rw-r--r--   0        0        0      950 2023-06-21 13:50:12.422384 exchanges-wrapper-1.3.4b0/.github/workflows/docker-image.yml
+-rw-r--r--   0        0        0     1105 2023-06-21 11:56:25.815510 exchanges-wrapper-1.3.4b0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0     6960 2023-07-11 17:04:46.392454 exchanges-wrapper-1.3.4b0/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.4b0/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.4b0/LICENSE.md
+-rw-r--r--   0        0        0     7068 2023-07-06 10:11:57.993253 exchanges-wrapper-1.3.4b0/README.md
+-rw-r--r--   0        0        0    15398 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.4b0/example/exch_client.py
+-rwxr-xr-x   0        0        0      216 2023-06-20 16:57:56.566218 exchanges-wrapper-1.3.4b0/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1319 2023-07-16 16:05:47.206493 exchanges-wrapper-1.3.4b0/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    25161 2023-07-16 16:08:14.630475 exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-07-16 16:08:14.634480 exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19609 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6184 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61849 2023-07-12 07:21:31.626804 exchanges-wrapper-1.3.4b0/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.4b0/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12485 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    47721 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4429 2023-06-29 16:06:47.201826 exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10260 2023-07-08 19:35:27.596549 exchanges-wrapper-1.3.4b0/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15714 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16089 2023-07-04 16:39:16.922863 exchanges-wrapper-1.3.4b0/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.4b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22397 2023-06-29 16:57:42.989839 exchanges-wrapper-1.3.4b0/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1147 2023-07-16 16:05:47.190524 exchanges-wrapper-1.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-07-16 16:05:47.198509 exchanges-wrapper-1.3.4b0/requirements.txt
+-rw-r--r--   0        0        0     7982 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.4b0/PKG-INFO
```

### Comparing `exchanges_wrapper-1.3.4.post1/LICENSE.md` & `exchanges-wrapper-1.3.4b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/README.md` & `exchanges-wrapper-1.3.4b0/README.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
- for crypto exchanges (Binance, Bitfinex, OKX, Huobi)
+ for crypto exchanges (Binance, Bitfinex, OKX, Huobi,)
  Utilizes one connection for many accounts and trading pairs.
  For SPOT market only
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.4-1"
+__version__ = "1.3.4b0"
 
 from pathlib import Path
 import shutil
 
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "exch_srv_cfg.toml")
 LOG_PATH = Path(WORK_PATH, "exch_srv_log")
 LOG_FILE = Path(LOG_PATH, "exch_srv.log")
 
-
 def init():
     if CONFIG_FILE.exists():
         print(f"Server config found at {CONFIG_FILE}")
     else:
         print("Can't find config file! Creating it...")
         CONFIG_PATH.mkdir(parents=True, exist_ok=True)
         LOG_PATH.mkdir(parents=True, exist_ok=True)
         shutil.copy(Path(Path(__file__).parent.absolute(), "exch_srv_cfg.toml.template"), CONFIG_FILE)
         print(f"Before first run place account(s) API key into {CONFIG_FILE}")
         raise SystemExit(1)
 
-
 if __name__ == '__main__':
     init()
```

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/api_pb2.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/bitfinex_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     cummulative_quote_qty = str(Decimal(executed_qty) * Decimal(avg_fill_price))
     orig_quote_order_qty = str(Decimal(orig_qty) * Decimal(price))
     #
     if 'CANCELED' in res[13]:
         status = 'CANCELED'
     elif Decimal(orig_qty) > Decimal(executed_qty) > 0:
         status = 'PARTIALLY_FILLED'
-    elif Decimal(executed_qty) >= Decimal(orig_qty):
+    elif  Decimal(executed_qty) >= Decimal(orig_qty):
         status = 'FILLED'
     elif cancelled:
         status = 'CANCELED'
     else:
         status = 'NEW'
     #
     _type = "LIMIT"
@@ -530,15 +530,15 @@
         last_executed_quantity = last_event[1]
         last_executed_price = last_event[2]
     last_quote_asset_transacted = str(Decimal(last_executed_quantity) * Decimal(last_executed_price))
     if 'CANCELED' in res[13]:
         status = 'CANCELED'
     elif Decimal(order_quantity) > Decimal(cumulative_filled_quantity) > 0:
         status = 'PARTIALLY_FILLED'
-    elif Decimal(cumulative_filled_quantity) >= Decimal(order_quantity):
+    elif  Decimal(cumulative_filled_quantity) >= Decimal(order_quantity):
         status = 'FILLED'
     else:
         status = 'NEW'
     #
     msg_binance = {
         "e": "executionReport",
         "E": res[5],
```

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/c_structures.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/client.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             price = price - (price % decimal.Decimal(price_filter["tickSize"]))
             # noinspection PyStringFormat
             price = (
                 (f"%.{precision}f" % truncate(price, precision))
                 .rstrip("0")
                 .rstrip(".")
             )
-        return decimal.Decimal(price)
+        return price
 
     def assert_symbol(self, symbol):
         if not symbol:
             raise ValueError("This query requires a symbol.")
         self.assert_symbol_exists(symbol)
 
     # keep support for hardcoded string but allow enums usage
```

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/events.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 #
 logger = logging.getLogger(__name__)
 formatter = logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s")
 #
 fh = logging.handlers.RotatingFileHandler(LOG_FILE, maxBytes=1000000, backupCount=10)
 fh.setFormatter(formatter)
 fh.setLevel(logging.DEBUG)
+# logger.addHandler(fh)
 #
 sh = logging.StreamHandler()
 sh.setFormatter(formatter)
 sh.setLevel(logging.INFO)
+# logger.addHandler(sh)
 #
 root_logger = logging.getLogger()
 root_logger.setLevel(min([fh.level, sh.level]))
 root_logger.addHandler(fh)
 root_logger.addHandler(sh)
```

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/huobi_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,30 +298,30 @@
             "v": str(tick.get('amount')),
             "q": str(tick.get('vol'))
         }
     }
     return msg_binance
 
 
-def interval(_interval) -> str:
+def interval(_interval: str) -> str:
     resolution = {
         '1m': '1min',
         '5m': '5min',
         '15m': '15min',
         '30m': '30min',
         '1h': '60min',
         '4h': '4hour',
         '1d': '1day',
         '1w': '1week',
         '1M': '1mon'
     }
-    return resolution.get(_interval, 'unresolved')
+    return resolution.get(_interval, 0)
 
 
-def interval2value(_interval) -> int:
+def interval2value(_interval: str) -> int:
     resolution = {
         '1min': 60,
         '5min': 5 * 60,
         '15min': 15 * 60,
         '30min': 30 * 60,
         '60min': 60 * 60,
         '4hour': 4 * 60 * 60,
```

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.3.4b0/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.4.post1/pyproject.toml` & `exchanges-wrapper-1.3.4b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,20 @@
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
     "aiohttp==3.8.4",
     "grpcio==1.56.0",
-    "grpcio-tools==1.56.0",
     "toml==0.10.2",
     "idna==3.4",
     "pyotp~=2.8.0",
     "simplejson==3.19.1",
     "shortuuid~=1.0.11",
-    "crypto-ws-api==1.0.1.post3",
+    "crypto_ws_api~=1.0.1",
 ]
 
 [tool.flit.module]
 name = "exchanges_wrapper"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/exchanges-wrapper"
```

### Comparing `exchanges_wrapper-1.3.4.post1/PKG-INFO` & `exchanges-wrapper-1.3.4b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.4.post1
+Version: 1.3.4b0
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: grpcio==1.56.0
-Requires-Dist: grpcio-tools==1.56.0
 Requires-Dist: toml==0.10.2
 Requires-Dist: idna==3.4
 Requires-Dist: pyotp~=2.8.0
 Requires-Dist: simplejson==3.19.1
 Requires-Dist: shortuuid~=1.0.11
-Requires-Dist: crypto-ws-api==1.0.1.post3
+Requires-Dist: crypto_ws_api~=1.0.1
 Project-URL: Source, https://github.com/DogsTailFarmer/exchanges-wrapper
 
 <h1 align="center"><img align="center" src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="75">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
 
 <h2 align="center">Binance, Bitfinex, Huobi, OKX,</h2>
 
 <h3 align="center">For SPOT markets</h3>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.4.post1 Summary:
-REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
-Author-email: Thomas Marchand
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.4b0 Summary: REST
+API and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
+email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.56.0 Requires-Dist: grpcio-
-tools==1.56.0 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
-Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Requires-Dist:
-shortuuid~=1.0.11 Requires-Dist: crypto-ws-api==1.0.1.post3 Project-URL:
-Source, https://github.com/DogsTailFarmer/exchanges-wrapper
+Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.56.0 Requires-Dist: toml==0.10.2
+Requires-Dist: idna==3.4 Requires-Dist: pyotp~=2.8.0 Requires-Dist:
+simplejson==3.19.1 Requires-Dist: shortuuid~=1.0.11 Requires-Dist:
+crypto_ws_api~=1.0.1 Project-URL: Source, https://github.com/DogsTailFarmer/
+exchanges-wrapper
         ****** [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
 Logo%202v3.svg]Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
```

