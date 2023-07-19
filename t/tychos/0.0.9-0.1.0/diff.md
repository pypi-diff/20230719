# Comparing `tmp/tychos-0.0.9.tar.gz` & `tmp/tychos-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.9.tar", last modified: Wed Jul 19 15:16:02 2023, max compression
+gzip compressed data, was "tychos-0.1.0.tar", last modified: Wed Jul 19 15:32:07 2023, max compression
```

## Comparing `tychos-0.0.9.tar` & `tychos-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:16:02.702265 tychos-0.0.9/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.9/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:16:02.702088 tychos-0.0.9/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)     2507 2023-07-18 21:52:54.000000 tychos-0.0.9/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-19 15:16:02.702306 tychos-0.0.9/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-19 15:15:19.000000 tychos-0.0.9/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:16:02.700582 tychos-0.0.9/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.9/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.9/tychos/cli.py
--rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.9/tychos/config.py
--rw-r--r--   0 abe732     (501) staff       (20)     1551 2023-07-19 14:48:09.000000 tychos-0.0.9/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)     1749 2023-07-19 14:47:57.000000 tychos-0.0.9/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:16:02.701882 tychos-0.0.9/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      303 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/entry_points.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:32:07.727715 tychos-0.1.0/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.1.0/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:32:07.727381 tychos-0.1.0/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     2507 2023-07-19 15:30:24.000000 tychos-0.1.0/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-19 15:32:07.727781 tychos-0.1.0/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-19 15:29:30.000000 tychos-0.1.0/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:32:07.722829 tychos-0.1.0/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.1.0/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.1.0/tychos/cli.py
+-rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.1.0/tychos/config.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1497 2023-07-19 15:29:14.000000 tychos-0.1.0/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1695 2023-07-19 15:28:59.000000 tychos-0.1.0/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:32:07.725728 tychos-0.1.0/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      303 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.9/LICENSE` & `tychos-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.9/PKG-INFO` & `tychos-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
```

### Comparing `tychos-0.0.9/README.md` & `tychos-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tychos-0.0.9/tychos/cli.py` & `tychos-0.1.0/tychos/cli.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.9/tychos/vector.py` & `tychos-0.1.0/tychos/vector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import requests
 
 class _Vector:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('TYCHOS_API_KEY')
-        # self.base_url = 'https://api.tychos.ai/v1/'
-        self.base_url = 'http://localhost:3001/v1/'
+        self.base_url = 'https://api.tychos.ai/v1/'
         
     def create(self, type, input_text, model, model_provider_key=None):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
         if type == "text_embedding":
             if model == "text-embedding-ada-002":
                 try:
```

### Comparing `tychos-0.0.9/tychos/vector_data_store.py` & `tychos-0.1.0/tychos/vector_data_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import requests
 from .vector import _Vector
 
 class VectorDataStore:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('TYCHOS_API_KEY')
-        # self.base_url = 'https://api.tychos.ai/v1/'
-        self.base_url = 'http://localhost:3001/v1/'
+        self.base_url = 'https://api.tychos.ai/v1/'
         self.vector = _Vector(api_key=self.api_key)
 
     def query(self, name, query_string, limit):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
         # vectorize query string
         query_vector = self.vector.create(
```

### Comparing `tychos-0.0.9/tychos.egg-info/PKG-INFO` & `tychos-0.1.0/tychos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
```

