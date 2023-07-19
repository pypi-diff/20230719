# Comparing `tmp/location-local-0.0.4.tar.gz` & `tmp/location-local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "location-local-0.0.4.tar", last modified: Tue Jul 18 11:36:38 2023, max compression
+gzip compressed data, was "location-local-0.0.5.tar", last modified: Wed Jul 19 08:46:06 2023, max compression
```

## Comparing `location-local-0.0.4.tar` & `location-local-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:38.307837 location-local-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:38.307837 location-local-0.0.4/CirclesGetCountryName/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:22.000000 location-local-0.0.4/CirclesGetCountryName/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 11:36:22.000000 location-local-0.0.4/CirclesGetCountryName/opencage_get_country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 11:36:38.307837 location-local-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:38.307837 location-local-0.0.4/location_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 11:36:38.000000 location-local-0.0.4/location_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 11:36:38.000000 location-local-0.0.4/location_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:36:38.000000 location-local-0.0.4/location_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 11:36:38.000000 location-local-0.0.4/location_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:36:38.307837 location-local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-18 11:36:22.000000 location-local-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:38.307837 location-local-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-18 11:36:22.000000 location-local-0.0.4/tests/test_opnecage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/CirclesGetCountryName/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:53.000000 location-local-0.0.5/CirclesGetCountryName/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-19 08:45:53.000000 location-local-0.0.5/CirclesGetCountryName/opencage_get_country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 08:46:06.958697 location-local-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/location_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:46:06.958697 location-local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-19 08:45:53.000000 location-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-19 08:45:53.000000 location-local-0.0.5/tests/test_opnecage.py
```

### Comparing `location-local-0.0.4/CirclesGetCountryName/opencage_get_country_name.py` & `location-local-0.0.5/CirclesGetCountryName/opencage_get_country_name.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 from opencage.geocoder import OpenCageGeocode
-from LoggerLocalPythonPackage import LocalLogger
+from LoggerLocalPythonPackage.LocalLogger import _Local_Logger as local_logger
 from dotenv import load_dotenv
 load_dotenv()
-Local_Logger=LocalLogger._Local_Logger
+
 class Country:
     def __init__(self):
         pass
-
-    def get_country_name(self, location):
+    
+    @staticmethod
+    def get_country_name(location):
         # Create a geocoder instance
-        Local_Logger.start("start get_country_name(${location}) ")
+        local_logger.start("start get_country_name(${location}) ")
         api_key = os.getenv("OPENCAGE_KEY")
 
         # Define the city or state
         geocoder = OpenCageGeocode(api_key)
 
         # Use geocoding to get the location details
         results = geocoder.geocode(location)
@@ -24,17 +25,18 @@
             components = first_result['components']
 
             # Extract the country from components
             country = components.get('country', '')
             if not country:
                 # If country is not found, check for country_code as an alternative
                 country = components.get('country_code', '')
-            Local_Logger.end("end get_country_name return value= "+str(country))
+            local_logger.end("end get_country_name return value= "+str(country))
             return country
 
         else:
-            Local_Logger.end("end get_country_name return value= None")
+            local_logger.error("country didnt found for %s."%location)
+            local_logger.end("end get_country_name return value= None")
             return None
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `location-local-0.0.4/setup.py` & `location-local-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='location-local',
-     version='0.0.4',
+     version='0.0.5', # https://pypi.org/project/location-local/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local OpenCage Python",
      long_description="This is a package for sharing common OpenCage function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

