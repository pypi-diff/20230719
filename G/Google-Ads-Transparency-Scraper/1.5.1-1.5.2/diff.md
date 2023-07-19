# Comparing `tmp/Google-Ads-Transparency-Scraper-1.5.1.tar.gz` & `tmp/Google-Ads-Transparency-Scraper-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.1.tar", last modified: Sat Jul  1 10:52:06 2023, max compression
+gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.2.tar", last modified: Tue Jul 18 17:49:48 2023, max compression
```

## Comparing `Google-Ads-Transparency-Scraper-1.5.1.tar` & `Google-Ads-Transparency-Scraper-1.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 10:52:06.842738 Google-Ads-Transparency-Scraper-1.5.1/
-drwxrwxrwx   0        0        0        0 2023-07-01 10:52:06.813738 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/
--rw-rw-rw-   0        0        0      106 2023-06-28 05:20:16.000000 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/__init__.py
--rw-rw-rw-   0        0        0    10314 2023-06-28 07:22:06.000000 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/main.py
--rw-rw-rw-   0        0        0    11448 2023-06-28 06:06:26.000000 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/regions.py
-drwxrwxrwx   0        0        0        0 2023-07-01 10:52:06.841744 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/
--rw-rw-rw-   0        0        0      876 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      876 2023-07-01 10:52:06.842738 Google-Ads-Transparency-Scraper-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-06-26 11:23:38.000000 Google-Ads-Transparency-Scraper-1.5.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-01 10:52:06.845738 Google-Ads-Transparency-Scraper-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-07-01 10:51:48.000000 Google-Ads-Transparency-Scraper-1.5.1/setup.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-18 17:49:48.083448 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/
+-rw-r--r--   0 fani      (1000) fani      (1000)       67 2023-07-05 16:41:06.000000 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/__init__.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    10691 2023-07-18 17:19:23.000000 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/main.py
+-rw-r--r--   0 fani      (1000) fani      (1000)    11448 2023-06-28 18:06:28.000000 Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/regions.py
+drwxr-xr-x   0 fani      (1000) fani      (1000)        0 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)      399 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)        1 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       69 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)       22 2023-07-18 17:49:48.000000 Google-Ads-Transparency-Scraper-1.5.2/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-r--r--   0 fani      (1000) fani      (1000)      858 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/PKG-INFO
+-rw-r--r--   0 fani      (1000) fani      (1000)     5455 2023-07-18 17:43:14.000000 Google-Ads-Transparency-Scraper-1.5.2/README.md
+-rw-r--r--   0 fani      (1000) fani      (1000)       79 2023-07-18 17:49:48.087448 Google-Ads-Transparency-Scraper-1.5.2/setup.cfg
+-rw-r--r--   0 fani      (1000) fani      (1000)     1273 2023-07-18 17:49:17.000000 Google-Ads-Transparency-Scraper-1.5.2/setup.py
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/main.py` & `Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,39 +28,48 @@
 def show_regions_list():
     """Displays Supported Regions Name along with their Region Codes"""
     print("Regions List")
     for region_code in Regions.keys():
         print(f"Region Name: {Regions[region_code]['Region']}\tRegion Code: {region_code}")
 
 class GoogleAds:
-    def __init__(self, region="anywhere"):
+    def __init__(self, region="anywhere", proxy=None):
         self.reqs = requests.Session()
         self.headers = HEADERS
+        #proxy config
+        self.proxy = proxy
+        if proxy is not None:
+            self.reqs.proxies.update(proxy)
+
         self.r_check = True
         if region == "anywhere":
             self.r_check = False
-        if not Regions.get(region) and not self.r_check:
+        print((not Regions.get(region)) and self.r_check)
+        if (not Regions.get(region)) and self.r_check:
             raise Exception("Invalid Region Code")
         self.region = region
         self.region_num = Regions[region]["1"] if self.r_check else 0
         self.get_cookies()
 
     def get_cookies(self):
         """Get Cookies from the main url https://adstransparency.google.com/ and store them in requests Session"""
         params = {
             'region': self.region,
         }
         self.reqs.get('https://adstransparency.google.com/', params=params, headers=self.headers)#.text.replace("\/","")
         #response = str(response[response.find("tfaaReportAppInfo"):]).encode('utf8').decode('unicode_escape')
         #print(json.loads(response[response.find("["):response.find(']')+1]))
 
-    def refresh_session(self):
+    def refresh_session(self, proxy=None):
         """Refresh Session cookies"""
         self.reqs = requests.Session()
         self.get_cookies()
+        if proxy is not None:
+            self.proxy = proxy
+        self.reqs.proxies.update(self.proxy)
 
     def get_all_search_suggestions(self, keyword: str) -> list:
         """
             Gets All suggestions from the Google Ads Transparency for given keyword.
             Returns list of Suggestions along with their details
             Returns Empty list [] if no suggestion found"""
         data = {
@@ -206,15 +215,16 @@
         else:
             ad_detail["Video URL"] = ad_detail["Ad Link"]
         return ad_detail
 
 if __name__ == '__main__':
     a = GoogleAds()
     keyword = "ibbedesign"
-    keyword = "facebook"
+    keyword = "Google"
+    print(a.get_advistisor_by_domain(keyword), end="\n\n")
     creatives = a.get_creative_Ids(keyword)
     if creatives["Ad Count"]:
         advertisor_id = creatives["Advertisor Id"]
         for creative_id in creatives["Creative_Ids"]:
             #print(a.get_breif_ads(advertisor_id, creative_id))
             print(a.get_detailed_ad(advertisor_id,creative_id))
     else:
```

### Comparing `Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/regions.py` & `Google-Ads-Transparency-Scraper-1.5.2/GoogleAdsTransparency/regions.py`

 * *Files identical despite different names*

### Comparing `Google-Ads-Transparency-Scraper-1.5.1/setup.py` & `Google-Ads-Transparency-Scraper-1.5.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Install packages as defined in this file into the Python environment."""
 from setuptools import setup, find_packages
-
 setup(
     name="Google-Ads-Transparency-Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
     description="A scraper for getting Ads from Google Ads Transparency",
-    version="1.5.1",
+    version="1.5.2",
     packages=find_packages(),
-    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.1.tar.gz',
-    keywords= ['Google', 'Transparency', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scrapre'],
+    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.2.tar.gz',
+    keywords= ['Google', 'Transparency', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scraper'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
         "Requests>=2.31.0",
         "lxml>=4.6.3",
     ],
```

