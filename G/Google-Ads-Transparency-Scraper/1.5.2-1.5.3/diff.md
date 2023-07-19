# Comparing `tmp/Google-Ads-Transparency-Scraper-1.5.2.tar.gz` & `tmp/Google-Ads-Transparency-Scraper-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.2.tar", last modified: Tue Jul 18 17:49:48 2023, max compression
+gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.3.tar", last modified: Wed Jul 19 09:34:23 2023, max compression
```

## Comparing `Google-Ads-Transparency-Scraper-1.5.2.tar` & `Google-Ads-Transparency-Scraper-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-18 17:49:48.083448 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/
--rw-r--r--   0 fani      (1000) fani      (1000)       67 2023-07-05 16:41:06.000000 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/__init__.py
--rw-r--r--   0 fani      (1000) fani      (1000)    10691 2023-07-18 17:19:23.000000 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/main.py
--rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-06-28 18:06:28.000000 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/regions.py
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/
--rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 fani      (1000) fani      (1000)      399 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-r--r--   0 fani      (1000) fani      (1000)       22 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/PKG-INFO
--rw-r--r--   0 fani      (1000) fani      (1000)     5455 2023-07-18 17:43:14.000000 Google-Ads-Transparency-Scraper-1.5.2/README.md
--rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/setup.cfg
--rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-18 17:49:17.000000 Google-Ads-Transparency-Scraper-1.5.2/setup.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 09:34:23.768173 Google-Ads-Transparency-Scraper-1.5.3/
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 09:34:23.768173 Google-Ads-Transparency-Scraper-1.5.3/GoogleAds/
+-rw-r--r--   0 fani      (1000) fani      (1000)       67 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.3/GoogleAds/__init__.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    10718 2023-07-19 09:19:55.000000 Google-Ads-Transparency-Scraper-1.5.3/GoogleAds/main.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.3/GoogleAds/regions.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 09:34:23.768173 Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 09:34:23.000000 Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)      363 2023-07-19 09:34:23.000000 Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-19 09:34:23.000000 Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-19 09:34:23.000000 Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       10 2023-07-19 09:34:23.000000 Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 09:34:23.768173 Google-Ads-Transparency-Scraper-1.5.3/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)     5455 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.3/README.md
+-rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-19 09:34:23.768173 Google-Ads-Transparency-Scraper-1.5.3/setup.cfg
+-rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-19 09:18:15.000000 Google-Ads-Transparency-Scraper-1.5.3/setup.py
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/main.py` & `Google-Ads-Transparency-Scraper-1.5.3/GoogleAds/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import requests
 from typing import Union
 from bs4 import BeautifulSoup as soap
-from regions import Regions
+from .regions import Regions
 
 HEADERS = {
     'authority': 'adstransparency.google.com',
     'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
     'accept-language': 'en-US,en;q=0.9',
     'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
     'sec-ch-ua-arch': '"x86"',
@@ -33,15 +33,15 @@
 
 class GoogleAds:
     def __init__(self, region="anywhere", proxy=None):
         self.reqs = requests.Session()
         self.headers = HEADERS
         #proxy config
         self.proxy = proxy
-        if proxy is not None:
+        if proxy is not None or not proxy:
             self.reqs.proxies.update(proxy)
 
         self.r_check = True
         if region == "anywhere":
             self.r_check = False
         print((not Regions.get(region)) and self.r_check)
         if (not Regions.get(region)) and self.r_check:
@@ -59,15 +59,15 @@
         #response = str(response[response.find("tfaaReportAppInfo"):]).encode('utf8').decode('unicode_escape')
         #print(json.loads(response[response.find("["):response.find(']')+1]))
 
     def refresh_session(self, proxy=None):
         """Refresh Session cookies"""
         self.reqs = requests.Session()
         self.get_cookies()
-        if proxy is not None:
+        if proxy is not None or not proxy:
             self.proxy = proxy
         self.reqs.proxies.update(self.proxy)
 
     def get_all_search_suggestions(self, keyword: str) -> list:
         """
             Gets All suggestions from the Google Ads Transparency for given keyword.
             Returns list of Suggestions along with their details
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/regions.py` & `Google-Ads-Transparency-Scraper-1.5.3/GoogleAds/regions.py`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.3/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5.2
+Version: 1.5.3
 Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.2.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.3.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.2/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5.2
+Version: 1.5.3
 Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.2.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.3.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.2/README.md` & `Google-Ads-Transparency-Scraper-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.2/setup.py` & `Google-Ads-Transparency-Scraper-1.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import setup, find_packages
 setup(
     name="Google-Ads-Transparency-Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
     description="A scraper for getting Ads from Google Ads Transparency",
-    version="1.5.2",
+    version="1.5.3",
     packages=find_packages(),
-    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.2.tar.gz',
+    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.3.tar.gz',
     keywords= ['Google', 'Transparency', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scraper'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
         "Requests>=2.31.0",
         "lxml>=4.6.3",
```

