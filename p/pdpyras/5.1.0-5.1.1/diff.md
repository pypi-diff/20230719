# Comparing `tmp/pdpyras-5.1.0.tar.gz` & `tmp/pdpyras-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpyras-5.1.0.tar", last modified: Mon Jun 26 16:41:32 2023, max compression
+gzip compressed data, was "pdpyras-5.1.1.tar", last modified: Wed Jul 19 15:46:08 2023, max compression
```

## Comparing `pdpyras-5.1.0.tar` & `pdpyras-5.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-26 16:41:32.338811 pdpyras-5.1.0/
--rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.1.0/LICENSE
--rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-26 16:41:32.338665 pdpyras-5.1.0/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-17 22:04:20.000000 pdpyras-5.1.0/README.rst
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-26 16:41:32.338465 pdpyras-5.1.0/pdpyras.egg-info/
--rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)      192 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/SOURCES.txt
--rw-r--r--   0 demitri    (503) staff       (20)        1 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/dependency_links.txt
--rw-r--r--   0 demitri    (503) staff       (20)       29 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/requires.txt
--rw-r--r--   0 demitri    (503) staff       (20)        8 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/top_level.txt
--rw-r--r--   0 demitri    (503) staff       (20)    82928 2023-06-26 16:39:56.000000 pdpyras-5.1.0/pdpyras.py
--rw-r--r--   0 demitri    (503) staff       (20)       38 2023-06-26 16:41:32.338862 pdpyras-5.1.0/setup.cfg
--rw-r--r--   0 demitri    (503) staff       (20)      657 2023-06-26 16:39:56.000000 pdpyras-5.1.0/setup.py
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-07-19 15:46:08.856900 pdpyras-5.1.1/
+-rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.1.1/LICENSE
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-07-19 15:46:08.856752 pdpyras-5.1.1/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-17 22:04:20.000000 pdpyras-5.1.1/README.rst
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-07-19 15:46:08.856570 pdpyras-5.1.1/pdpyras.egg-info/
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-07-19 15:46:08.000000 pdpyras-5.1.1/pdpyras.egg-info/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)      192 2023-07-19 15:46:08.000000 pdpyras-5.1.1/pdpyras.egg-info/SOURCES.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        1 2023-07-19 15:46:08.000000 pdpyras-5.1.1/pdpyras.egg-info/dependency_links.txt
+-rw-r--r--   0 demitri    (503) staff       (20)       29 2023-07-19 15:46:08.000000 pdpyras-5.1.1/pdpyras.egg-info/requires.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        8 2023-07-19 15:46:08.000000 pdpyras-5.1.1/pdpyras.egg-info/top_level.txt
+-rw-r--r--   0 demitri    (503) staff       (20)    82910 2023-07-19 15:45:50.000000 pdpyras-5.1.1/pdpyras.py
+-rw-r--r--   0 demitri    (503) staff       (20)       38 2023-07-19 15:46:08.856953 pdpyras-5.1.1/setup.cfg
+-rw-r--r--   0 demitri    (503) staff       (20)      657 2023-07-19 15:45:50.000000 pdpyras-5.1.1/setup.py
```

### Comparing `pdpyras-5.1.0/LICENSE` & `pdpyras-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdpyras-5.1.0/README.rst` & `pdpyras-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pdpyras-5.1.0/pdpyras.py` & `pdpyras-5.1.1/pdpyras.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Libraries from PyPI
 import requests
 from deprecation import deprecated, DeprecatedWarning
 from urllib3.exceptions import HTTPError, PoolError
 from requests.exceptions import RequestException
 
-__version__ = '5.1.0'
+__version__ = '5.1.1'
 
 #######################
 ### CLIENT DEFAULTS ###
 #######################
 ITERATION_LIMIT = 1e4
 """
 The maximum position of a result in classic pagination.
@@ -1715,14 +1715,17 @@
         :type params: dict or None
         :type page_size: int or None
         :type total: bool
         """
         # Get entity wrapping and validate that the URL being requested is
         # likely to support pagination:
         path = canonical_path(self.url, url)
+        # Short-circuit to cursor-based iteration:
+        if path in CURSOR_BASED_PAGINATION_PATHS:
+            return self.iter_cursor(url, params=params)
         endpoint = f"GET {path}"
         nodes = path.split('/')
         if is_path_param(nodes[-1]):
             # This is based on an as-yet universal pattern, but like classic
             # entity wrapping conventions, it isn't explicitly in the API
             # contract and so it may be subject to change. Therefore, I can only
             # hope our API developers do not deviate from it. If ever a path
@@ -1731,18 +1734,14 @@
             raise URLError(f"Path {path} (URL={url}) is for accessing an " \
                 "individual resource, versus a resource collection, and as " \
                 "such does not feature pagination.")
         _, wrapper = entity_wrappers('GET', path)
         if wrapper is None:
             raise URLError(f"Pagination is not supported for GET {path}.")
 
-        # Short-circuit to cursor-based iteration:
-        if path in CURSOR_BASED_PAGINATION_PATHS:
-            return self.iter_cursor(url, attribute=res_w, params=params)
-
         # Parameters to send:
         data = {}
         if page_size is None:
             data['limit'] = self.default_page_size
         else:
             data['limit'] = page_size
         if total:
```

### Comparing `pdpyras-5.1.0/setup.py` & `pdpyras-5.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '5.1.0'
+__version__ = '5.1.1'
 
 if __name__ == '__main__':
     setup(
         name='pdpyras',
         description="PagerDuty Python REST API Sessions",
         long_description="A basic REST API client for PagerDuty based on Requests' Session class",
         py_modules=['pdpyras'],
```

