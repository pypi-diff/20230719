# Comparing `tmp/talkytrend-1.9.0.tar.gz` & `tmp/talkytrend-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.9.0.tar", max compression
+gzip compressed data, was "talkytrend-1.9.1.tar", max compression
```

## Comparing `talkytrend-1.9.0.tar` & `talkytrend-1.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-17 16:47:26.940350 talkytrend-1.9.0/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-17 16:47:26.940350 talkytrend-1.9.0/README.md
--rw-r--r--   0        0        0     2651 2023-07-17 16:47:27.692346 talkytrend-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-17 16:47:27.692346 talkytrend-1.9.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-17 16:47:26.940350 talkytrend-1.9.0/talkytrend/config.py
--rw-r--r--   0        0        0     2216 2023-07-17 16:47:26.940350 talkytrend-1.9.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6450 2023-07-17 16:47:26.940350 talkytrend-1.9.0/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-19 15:22:48.076501 talkytrend-1.9.1/LICENSE
+-rw-r--r--   0        0        0     3419 2023-07-19 15:22:48.076501 talkytrend-1.9.1/README.md
+-rw-r--r--   0        0        0     3107 2023-07-19 15:22:51.404527 talkytrend-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-19 15:22:51.412527 talkytrend-1.9.1/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-19 15:22:48.076501 talkytrend-1.9.1/talkytrend/config.py
+-rw-r--r--   0        0        0     2542 2023-07-19 15:22:48.076501 talkytrend-1.9.1/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6432 2023-07-19 15:22:48.076501 talkytrend-1.9.1/talkytrend/main.py
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 talkytrend-1.9.1/PKG-INFO
```

### Comparing `talkytrend-1.9.0/LICENSE` & `talkytrend-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.9.0/README.md` & `talkytrend-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
        </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/v/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/dm/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
-      <a href="https://github.com/mraniki/talkytrend/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/talkytrend/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
+      <a href="https://github.com/mraniki/talkytrend/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/talkytrend/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
       <a href="https://talky.readthedocs.io/projects/talkytrend/en/latest/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
       <a href="https://codebeat.co/projects/github-com-mraniki-talkytrend-main"><img src="https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6"/></a> <br>
       <a href="https://codecov.io/gh/mraniki/talkytrend"><img src="https://codecov.io/gh/mraniki/talkytrend/branch/main/graph/badge.svg?token=WAHUEMAJN6"/></a><br>
     </td>
     <td align="left"> 
 Retrieve asset trend and economic data.<br>
 Trading view connectivity with signal scanner<br>
```

#### html2text {}

```diff
@@ -11,20 +11,19 @@
 badge&logo=buymeacoffee&logoColor=white] [https://
 img.shields.io/badge/talky-blue?style=for-the-
 badge&logo=telegram&logoColor=white] [https://
 img.shields.io/discord/1049307055867035648?style=for-the-
 badge&logo=discord&logoColor=white&label=%20%20&color=blue]
 [https://img.shields.io/pypi/v/talkytrend?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/pypi/dm/talkytrend?style=for-the-
-badge&logo=PyPI&logoColor=white]                            Retrieve asset
-[https://img.shields.io/github/actions/workflow/status/     trend and economic
-mraniki/talkytrend/                                         data.
-%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-  Trading view
-the-badge&logo=GitHub&logoColor=white]                      connectivity with
+[https://img.shields.io/pypi/dm/talkytrend?style=for-the-   Retrieve asset
+badge&logo=PyPI&logoColor=white]                            trend and economic
+[https://img.shields.io/github/actions/workflow/status/     data.
+mraniki/talkytrend/%F0%9F%91%B7Flow.yml?style=for-the-      Trading view
+badge&logo=GitHub&logoColor=white]                          connectivity with
 [https://readthedocs.org/projects/talkytrend/badge/         signal scanner
 ?version=latest&style=for-the-badge]                        News connectivity
 [https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-        FOMC reminder
 5907e180c9e6]
 [https://codecov.io/gh/mraniki/talkytrend/branch/main/
 graph/badge.svg?token=WAHUEMAJN6]
 ** How to use it **
```

### Comparing `talkytrend-1.9.0/talkytrend/config.py` & `talkytrend-1.9.1/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.9.0/talkytrend/default_settings.toml` & `talkytrend-1.9.1/talkytrend/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,30 @@
 fomc_decision_date = ["2023-09-20","2023-11-01","2023-12-13"]
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&max=2&apikey="
 news_api_key = ""
 enable_feed = true
 news_feed = "https://www.dailyfx.com/feeds/market-news"
+finnhub_api_key=""
+alphavantage_api_key = "demo"
+twelvedata_api_key = ""
 
 
+
+
+
+
+###############################
+###      TESTING SETTINGS   ###
+###############################
+# Any of those settings are used 
+# for testing purpose.
+# It can be ignored. 
+
 [testing]
 VALUE = "On Testing"
 talkytrend_enabled = true
 scanner_frequency = 2
 enable_signals = true
 assets = [
     { id ="EURUSD", exchange='FX_IDC',screener="forex"},
@@ -53,7 +67,10 @@
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
 enable_feed = true
 news_feed = "http://feeds.feedburner.com/zerohedge/feed/"
 # news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
 # news_feed = "https://www.dailyfx.com/feeds/market-news"
 #news_feed="https://www.reutersagency.com/feed/?taxonomy=best-sectors&post_type=best"
+finnhub_api_key= ""
+alphavantage_api_key = "demo"
+twelvedata_api_key = ""
```

### Comparing `talkytrend-1.9.0/talkytrend/main.py` & `talkytrend-1.9.1/talkytrend/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
  talky trend Main
 """
 
 import asyncio
 import logging
-from datetime import date
+from datetime import date, datetime, timezone
+
 import aiohttp
 import xmltodict
 from prettytable import PrettyTable
 from tradingview_ta import TA_Handler
+
 from talkytrend import __version__
 from talkytrend.config import settings
 
 
 class TalkyTrend:
     def __init__(self):
         self.logger = logging.getLogger("TalkyTrend")
         self.enabled = settings.talkytrend_enabled
         if not self.enabled:
             return
         self.assets = settings.assets
-        self.asset_signals = {}
         self.economic_calendar = settings.economic_calendar
         self.news_url = (
             f"{settings.news_url}{settings.news_api_key}"
             if settings.news_api_key
             else settings.news_url
         )
         self.live_tv = settings.live_tv_url
@@ -81,15 +82,15 @@
                 table.add_row([asset["id"], current_signal])
                 signals.append(signal_item)
 
         return table.get_string()
 
     async def fetch_key_events(self):
         def filter_events(data, today):
-            return [event for event in data if event.get('date', '').startswith(today)]
+            return [event for event in data if event.get('date', '') > today]
 
         def is_usd_high_impact(event):
             return (
                 event.get('impact') == 'High' and
                 event.get('country') in {'USD', 'ALL'}
             )
 
@@ -102,15 +103,15 @@
         def format_event(event):
             return f"💬 {event['title']}\n⏰ {event['date']}"
 
         async with aiohttp.ClientSession() as session:
             async with session.get(self.economic_calendar, timeout=10) as response:
                 response.raise_for_status()
                 data = await response.json()
-                today = date.today().isoformat()
+                today = datetime.now().isoformat()
                 events = filter_events(data, today)
                 for event in events:
                     if is_usd_high_impact(event) or is_all_high_impact(event):
                         return format_event(event)
                     if is_opec_or_fomc(event):
                         return format_event(event)
         return None
```

### Comparing `talkytrend-1.9.0/PKG-INFO` & `talkytrend-1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.9.0
+Version: 1.9.1
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: finnhub-python (>=2.4.18,<3.0.0)
 Requires-Dist: prettytable (>=3.8.0,<4.0.0)
 Requires-Dist: tradingview_ta (>=3.3.0,<4.0.0)
+Requires-Dist: twelvedata (>=1.2.12,<2.0.0)
 Requires-Dist: xmltodict
 Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/talkytrend/issues
 Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 
 <br>
@@ -39,15 +41,15 @@
        </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/v/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/dm/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
-      <a href="https://github.com/mraniki/talkytrend/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/talkytrend/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
+      <a href="https://github.com/mraniki/talkytrend/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/talkytrend/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
       <a href="https://talky.readthedocs.io/projects/talkytrend/en/latest/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
       <a href="https://codebeat.co/projects/github-com-mraniki-talkytrend-main"><img src="https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6"/></a> <br>
       <a href="https://codecov.io/gh/mraniki/talkytrend"><img src="https://codecov.io/gh/mraniki/talkytrend/branch/main/graph/badge.svg?token=WAHUEMAJN6"/></a><br>
     </td>
     <td align="left"> 
 Retrieve asset trend and economic data.<br>
 Trading view connectivity with signal scanner<br>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.9.0 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.9.1 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
-Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist: prettytable
-(>=3.8.0,<4.0.0) Requires-Dist: tradingview_ta (>=3.3.0,<4.0.0) Requires-Dist:
-xmltodict Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/
-dev/CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/talkytrend/
-issues Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
-Description-Content-Type: text/markdown
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist: finnhub-python
+(>=2.4.18,<3.0.0) Requires-Dist: prettytable (>=3.8.0,<4.0.0) Requires-Dist:
+tradingview_ta (>=3.3.0,<4.0.0) Requires-Dist: twelvedata (>=1.2.12,<2.0.0)
+Requires-Dist: xmltodict Project-URL: Changelog, https://github.com/mraniki/
+talkytrend/blob/dev/CHANGELOG.rst Project-URL: Issues, https://github.com/
+mraniki/talkytrend/issues Project-URL: Support, https://github.com/mraniki/
+talkytrend/discussions Description-Content-Type: text/markdown
 *** TalkyTrend ***
 
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
 badge&logo=github&logoColor=white] [https://img.shields.io/
@@ -24,20 +25,19 @@
 badge&logo=buymeacoffee&logoColor=white] [https://
 img.shields.io/badge/talky-blue?style=for-the-
 badge&logo=telegram&logoColor=white] [https://
 img.shields.io/discord/1049307055867035648?style=for-the-
 badge&logo=discord&logoColor=white&label=%20%20&color=blue]
 [https://img.shields.io/pypi/v/talkytrend?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/pypi/dm/talkytrend?style=for-the-
-badge&logo=PyPI&logoColor=white]                            Retrieve asset
-[https://img.shields.io/github/actions/workflow/status/     trend and economic
-mraniki/talkytrend/                                         data.
-%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-  Trading view
-the-badge&logo=GitHub&logoColor=white]                      connectivity with
+[https://img.shields.io/pypi/dm/talkytrend?style=for-the-   Retrieve asset
+badge&logo=PyPI&logoColor=white]                            trend and economic
+[https://img.shields.io/github/actions/workflow/status/     data.
+mraniki/talkytrend/%F0%9F%91%B7Flow.yml?style=for-the-      Trading view
+badge&logo=GitHub&logoColor=white]                          connectivity with
 [https://readthedocs.org/projects/talkytrend/badge/         signal scanner
 ?version=latest&style=for-the-badge]                        News connectivity
 [https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-        FOMC reminder
 5907e180c9e6]
 [https://codecov.io/gh/mraniki/talkytrend/branch/main/
 graph/badge.svg?token=WAHUEMAJN6]
 ** How to use it **
```

