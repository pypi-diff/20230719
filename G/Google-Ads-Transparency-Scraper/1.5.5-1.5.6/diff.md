# Comparing `tmp/Google-Ads-Transparency-Scraper-1.5.5.tar.gz` & `tmp/Google-Ads-Transparency-Scraper-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.5.tar", last modified: Wed Jul 19 10:24:29 2023, max compression
+gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.6.tar", last modified: Wed Jul 19 10:32:47 2023, max compression
```

## Comparing `Google-Ads-Transparency-Scraper-1.5.5.tar` & `Google-Ads-Transparency-Scraper-1.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:24:29.371506 Google-Ads-Transparency-Scraper-1.5.5/
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:24:29.371506 Google-Ads-Transparency-Scraper-1.5.5/GoogleAds/
--rw-r--r--   0 fani      (1000) fani      (1000)       55 2023-07-19 09:38:14.000000 Google-Ads-Transparency-Scraper-1.5.5/GoogleAds/__init__.py
--rw-r--r--   0 fani      (1000) fani      (1000)    10676 2023-07-19 10:12:25.000000 Google-Ads-Transparency-Scraper-1.5.5/GoogleAds/main.py
--rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.5/GoogleAds/regions.py
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:24:29.371506 Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/
--rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:24:29.000000 Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 fani      (1000) fani      (1000)      363 2023-07-19 10:24:29.000000 Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-19 10:24:29.000000 Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-19 10:24:29.000000 Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-r--r--   0 fani      (1000) fani      (1000)       10 2023-07-19 10:24:29.000000 Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:24:29.371506 Google-Ads-Transparency-Scraper-1.5.5/PKG-INFO
--rw-r--r--   0 fani      (1000) fani      (1000)     5443 2023-07-19 09:44:59.000000 Google-Ads-Transparency-Scraper-1.5.5/README.md
--rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-19 10:24:29.371506 Google-Ads-Transparency-Scraper-1.5.5/setup.cfg
--rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-19 10:12:57.000000 Google-Ads-Transparency-Scraper-1.5.5/setup.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/
+-rw-r--r--   0 fani      (1000) fani      (1000)       55 2023-07-19 09:38:14.000000 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/__init__.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    10685 2023-07-19 10:29:57.000000 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/main.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/regions.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)      363 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       10 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)     5443 2023-07-19 09:44:59.000000 Google-Ads-Transparency-Scraper-1.5.6/README.md
+-rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/setup.cfg
+-rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-19 10:31:38.000000 Google-Ads-Transparency-Scraper-1.5.6/setup.py
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.5/GoogleAds/main.py` & `Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import requests
 from typing import Union
 from bs4 import BeautifulSoup as soap
-from .regions import Regions
+from GoogleAds.regions import Regions
 
 HEADERS = {
     'authority': 'adstransparency.google.com',
     'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
     'accept-language': 'en-US,en;q=0.9',
     'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
     'sec-ch-ua-arch': '"x86"',
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.5/GoogleAds/regions.py` & `Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/regions.py`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.5/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5.5
+Version: 1.5.6
 Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.5.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.6.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.5/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5.5
+Version: 1.5.6
 Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.5.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.6.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.5/README.md` & `Google-Ads-Transparency-Scraper-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.5/setup.py` & `Google-Ads-Transparency-Scraper-1.5.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import setup, find_packages
 setup(
     name="Google-Ads-Transparency-Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
     description="A scraper for getting Ads from Google Ads Transparency",
-    version="1.5.5",
+    version="1.5.6",
     packages=find_packages(),
-    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.5.tar.gz',
+    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.6.tar.gz',
     keywords= ['Google', 'Transparency', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scraper'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
         "Requests>=2.31.0",
         "lxml>=4.6.3",
```

