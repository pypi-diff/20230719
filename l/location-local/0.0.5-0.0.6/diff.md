# Comparing `tmp/location-local-0.0.5.tar.gz` & `tmp/location-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "location-local-0.0.5.tar", last modified: Wed Jul 19 08:46:06 2023, max compression
+gzip compressed data, was "location-local-0.0.6.tar", last modified: Wed Jul 19 12:56:01 2023, max compression
```

## Comparing `location-local-0.0.5.tar` & `location-local-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/CirclesGetCountryName/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:53.000000 location-local-0.0.5/CirclesGetCountryName/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-19 08:45:53.000000 location-local-0.0.5/CirclesGetCountryName/opencage_get_country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 08:46:06.958697 location-local-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/location_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 08:46:06.000000 location-local-0.0.5/location_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:46:06.958697 location-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-19 08:45:53.000000 location-local-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:06.958697 location-local-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-19 08:45:53.000000 location-local-0.0.5/tests/test_opnecage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.442494 location-local-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.442494 location-local-0.0.6/CirclesGetCountryName/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:48.000000 location-local-0.0.6/CirclesGetCountryName/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-19 12:55:48.000000 location-local-0.0.6/CirclesGetCountryName/opencage_get_country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 12:56:01.442494 location-local-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.442494 location-local-0.0.6/location_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 12:56:01.000000 location-local-0.0.6/location_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-19 12:56:01.000000 location-local-0.0.6/location_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:56:01.000000 location-local-0.0.6/location_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 12:56:01.000000 location-local-0.0.6/location_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:56:01.442494 location-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-19 12:55:48.000000 location-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.442494 location-local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-19 12:55:48.000000 location-local-0.0.6/tests/test_opnecage.py
```

### Comparing `location-local-0.0.5/CirclesGetCountryName/opencage_get_country_name.py` & `location-local-0.0.6/CirclesGetCountryName/opencage_get_country_name.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
 from opencage.geocoder import OpenCageGeocode
-from LoggerLocalPythonPackage.LocalLogger import _Local_Logger as local_logger
+from logger_local_python_package.localLogger import _Local_Logger as local_logger
 from dotenv import load_dotenv
 load_dotenv()
 
 class Country:
     def __init__(self):
         pass
     
     @staticmethod
     def get_country_name(location):
         # Create a geocoder instance
-        local_logger.start("start get_country_name(${location}) ")
+        object1={
+            'function': 'get_country_name',
+            'location':location
+        }
+        local_logger.start(object=object1)
         api_key = os.getenv("OPENCAGE_KEY")
 
         # Define the city or state
         geocoder = OpenCageGeocode(api_key)
 
         # Use geocoding to get the location details
         results = geocoder.geocode(location)
@@ -25,18 +29,26 @@
             components = first_result['components']
 
             # Extract the country from components
             country = components.get('country', '')
             if not country:
                 # If country is not found, check for country_code as an alternative
                 country = components.get('country_code', '')
-            local_logger.end("end get_country_name return value= "+str(country))
+            object2={
+                'function': 'get_country_name',
+                'return':country
+            }
+            local_logger.end(object=object2)
             return country
 
         else:
             local_logger.error("country didnt found for %s."%location)
-            local_logger.end("end get_country_name return value= None")
+            object3={
+                'function': 'get_country_name',
+                'return':'None'
+            }
+            local_logger.end(object=object3)
             return None
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `location-local-0.0.5/setup.py` & `location-local-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='location-local',
-     version='0.0.5', # https://pypi.org/project/location-local/
+     version='0.0.6', # https://pypi.org/project/location-local/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local OpenCage Python",
      long_description="This is a package for sharing common OpenCage function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `location-local-0.0.5/tests/test_opnecage.py` & `location-local-0.0.6/tests/test_opnecage.py`

 * *Files identical despite different names*

