# Comparing `tmp/Google-Ads-Transparency-Scraper-1.5.6.tar.gz` & `tmp/Google-Ads-Transparency-Scraper-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.6.tar", last modified: Wed Jul 19 10:32:47 2023, max compression
+gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.7.tar", last modified: Wed Jul 19 10:38:54 2023, max compression
```

## Comparing `Google-Ads-Transparency-Scraper-1.5.6.tar` & `Google-Ads-Transparency-Scraper-1.5.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/
--rw-r--r--   0 fani      (1000) fani      (1000)       55 2023-07-19 09:38:14.000000 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/__init__.py
--rw-r--r--   0 fani      (1000) fani      (1000)    10685 2023-07-19 10:29:57.000000 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/main.py
--rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/regions.py
-drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/
--rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 fani      (1000) fani      (1000)      363 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-r--r--   0 fani      (1000) fani      (1000)       10 2023-07-19 10:32:47.000000 Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/PKG-INFO
--rw-r--r--   0 fani      (1000) fani      (1000)     5443 2023-07-19 09:44:59.000000 Google-Ads-Transparency-Scraper-1.5.6/README.md
--rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-19 10:32:47.675995 Google-Ads-Transparency-Scraper-1.5.6/setup.cfg
--rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-19 10:31:38.000000 Google-Ads-Transparency-Scraper-1.5.6/setup.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:38:54.861199 Google-Ads-Transparency-Scraper-1.5.7/
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:38:54.861199 Google-Ads-Transparency-Scraper-1.5.7/GoogleAds/
+-rw-r--r--   0 fani      (1000) fani      (1000)       55 2023-07-19 09:38:14.000000 Google-Ads-Transparency-Scraper-1.5.7/GoogleAds/__init__.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    10677 2023-07-19 10:36:42.000000 Google-Ads-Transparency-Scraper-1.5.7/GoogleAds/main.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-07-19 09:14:20.000000 Google-Ads-Transparency-Scraper-1.5.7/GoogleAds/regions.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-19 10:38:54.861199 Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:38:54.000000 Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)      363 2023-07-19 10:38:54.000000 Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-19 10:38:54.000000 Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-19 10:38:54.000000 Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       10 2023-07-19 10:38:54.000000 Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-19 10:38:54.861199 Google-Ads-Transparency-Scraper-1.5.7/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)     5443 2023-07-19 09:44:59.000000 Google-Ads-Transparency-Scraper-1.5.7/README.md
+-rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-19 10:38:54.865198 Google-Ads-Transparency-Scraper-1.5.7/setup.cfg
+-rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-19 10:37:39.000000 Google-Ads-Transparency-Scraper-1.5.7/setup.py
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/main.py` & `Google-Ads-Transparency-Scraper-1.5.7/GoogleAds/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class GoogleAds:
     def __init__(self, region="anywhere", proxy=None):
         self.reqs = requests.Session()
         self.headers = HEADERS
         #proxy config
         self.proxy = proxy
-        if not proxy:
+        if proxy:
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
-        if not proxy:
+        if proxy:
             self.proxy = proxy
         self.reqs.proxies.update(self.proxy)
 
     def get_all_search_suggestions(self, keyword: str) -> list:
         """
             Gets All suggestions from the Google Ads Transparency for given keyword.
             Returns list of Suggestions along with their details
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.6/GoogleAds/regions.py` & `Google-Ads-Transparency-Scraper-1.5.7/GoogleAds/regions.py`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.6/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.7/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5.6
+Version: 1.5.7
 Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.6.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.7.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.6/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5.6
+Version: 1.5.7
 Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.6.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.7.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.6/README.md` & `Google-Ads-Transparency-Scraper-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.6/setup.py` & `Google-Ads-Transparency-Scraper-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import setup, find_packages
 setup(
     name="Google-Ads-Transparency-Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
     description="A scraper for getting Ads from Google Ads Transparency",
-    version="1.5.6",
+    version="1.5.7",
     packages=find_packages(),
-    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.6.tar.gz',
+    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.7.tar.gz',
     keywords= ['Google', 'Transparency', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scraper'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
         "Requests>=2.31.0",
         "lxml>=4.6.3",
```

