# Comparing `tmp/tychos-0.0.89.tar.gz` & `tmp/tychos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.89.tar", last modified: Sun Jul 16 14:40:21 2023, max compression
+gzip compressed data, was "tychos-0.0.9.tar", last modified: Wed Jul 19 15:16:02 2023, max compression
```

## Comparing `tychos-0.0.89.tar` & `tychos-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.162263 tychos-0.0.89/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.89/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)     2775 2023-07-16 14:40:21.162033 tychos-0.0.89/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)     2587 2023-07-16 14:16:28.000000 tychos-0.0.89/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-16 14:40:21.162320 tychos-0.0.89/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      503 2023-07-16 14:39:53.000000 tychos-0.0.89/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.160331 tychos-0.0.89/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.89/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.89/tychos/cli.py
--rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.89/tychos/config.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.161763 tychos-0.0.89/tychos/helpers/
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.89/tychos/helpers/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1553 2023-07-16 14:30:04.000000 tychos-0.0.89/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)     1732 2023-07-16 14:30:02.000000 tychos-0.0.89/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-16 14:40:21.161522 tychos-0.0.89/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)     2775 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      330 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/entry_points.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-16 14:40:21.000000 tychos-0.0.89/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:16:02.702265 tychos-0.0.9/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.9/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:16:02.702088 tychos-0.0.9/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     2507 2023-07-18 21:52:54.000000 tychos-0.0.9/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-19 15:16:02.702306 tychos-0.0.9/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-19 15:15:19.000000 tychos-0.0.9/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:16:02.700582 tychos-0.0.9/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.9/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.9/tychos/cli.py
+-rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.9/tychos/config.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1551 2023-07-19 14:48:09.000000 tychos-0.0.9/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1749 2023-07-19 14:47:57.000000 tychos-0.0.9/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:16:02.701882 tychos-0.0.9/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      303 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-19 15:16:02.000000 tychos-0.0.9/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.89/LICENSE` & `tychos-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.89/PKG-INFO` & `tychos-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.89
+Version: 0.0.9
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
@@ -48,20 +48,14 @@
 ```
 
 Query live vector datasets
 ```python
 # initialize data store
 data_store = tychos.VectorDataStore()
 
-# list available datasets
-datasets = data_store.list()
-
-# get name of the first dataset's id
-print(datasets['data'][0]['name'])
-
 # query the data store object
 query_results = data_store.query(
     index_name = "pub-med-abstracts", # dataset
     query_string = "What is the latest research on molecular peptides", # search string
     limit = 5, # number of results
 )
 
@@ -74,18 +68,18 @@
 
 ```sh
 tychos-cli query --api-key <YOUR-API-KEY> --name pub-med-abstracts --query-string <"Your query string"> --limit 5
 
 ```
 
 ## Datasets available
-We currently support a handful of research datasets. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
+We currently support the PubMed dataset and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
 
 ### Vector datasets
--   PubMed abstracts ([source][pub-med]): 33.2M documents, updated daily at 07:00 UTC.
+-   PubMed abstracts ([source][pub-med]): 33.8M documents, updated daily at 07:00 UTC.
 
 
 
 ## Feedback and support
 If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise an issue via GitHub.
```

### Comparing `tychos-0.0.89/README.md` & `tychos-0.0.9/tychos.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: tychos
+Version: 0.0.9
+Summary: Python client library for the Tychos API.
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
 To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
@@ -40,20 +48,14 @@
 ```
 
 Query live vector datasets
 ```python
 # initialize data store
 data_store = tychos.VectorDataStore()
 
-# list available datasets
-datasets = data_store.list()
-
-# get name of the first dataset's id
-print(datasets['data'][0]['name'])
-
 # query the data store object
 query_results = data_store.query(
     index_name = "pub-med-abstracts", # dataset
     query_string = "What is the latest research on molecular peptides", # search string
     limit = 5, # number of results
 )
 
@@ -66,18 +68,18 @@
 
 ```sh
 tychos-cli query --api-key <YOUR-API-KEY> --name pub-med-abstracts --query-string <"Your query string"> --limit 5
 
 ```
 
 ## Datasets available
-We currently support a handful of research datasets. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
+We currently support the PubMed dataset and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
 
 ### Vector datasets
--   PubMed abstracts ([source][pub-med]): 33.2M documents, updated daily at 07:00 UTC.
+-   PubMed abstracts ([source][pub-med]): 33.8M documents, updated daily at 07:00 UTC.
 
 
 
 ## Feedback and support
 If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise an issue via GitHub.
```

### Comparing `tychos-0.0.89/tychos/cli.py` & `tychos-0.0.9/tychos/cli.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.89/tychos/vector.py` & `tychos-0.0.9/tychos/vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import requests
 
 class _Vector:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('TYCHOS_API_KEY')
-        self.base_url = 'https://api.tychos.ai/api/'
-        # self.base_url = 'http://localhost:3001/api/'
+        # self.base_url = 'https://api.tychos.ai/v1/'
+        self.base_url = 'http://localhost:3001/v1/'
         
     def create(self, type, input_text, model, model_provider_key=None):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
         if type == "text_embedding":
             if model == "text-embedding-ada-002":
                 try:
-                    url = f'{self.base_url}create-vector'
+                    url = f'{self.base_url}vector/create'
                     headers = {'api_key': self.api_key}
                     payload = {
                                 'model_provider_key': model_provider_key,
                                 'input': input_text,
                                 'model': model,
                             }
                     response = requests.post(url=url, headers=headers, json=payload)
```

### Comparing `tychos-0.0.89/tychos/vector_data_store.py` & `tychos-0.0.9/tychos/vector_data_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 import requests
 from .vector import _Vector
 
 class VectorDataStore:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('TYCHOS_API_KEY')
-        self.base_url = 'https://api.tychos.ai/api/'
-        # self.base_url = 'http://localhost:3001/api/'
+        # self.base_url = 'https://api.tychos.ai/v1/'
+        self.base_url = 'http://localhost:3001/v1/'
         self.vector = _Vector(api_key=self.api_key)
 
     def query(self, name, query_string, limit):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
         # vectorize query string
         query_vector = self.vector.create(
             type="text_embedding",
             input_text=query_string,
             model="text-embedding-ada-002"
         )
 
         # send query request to vector data store
-        url = f'{self.base_url}query-vector-store'
+        url = f'{self.base_url}vector_data_store/query'
         headers = {'api_key': self.api_key}
         payload = {
                     'name': name,
                     'query_vector': query_vector,
                     'top': limit,
                 }
         response = requests.post(url=url, headers=headers, json=payload)
@@ -33,15 +33,15 @@
         response.raise_for_status()
 
         return response.json()
     
     def list(self):
         if self.api_key is None:
             raise ValueError("API key not set. Please set the API key using 'tychos.api_key = <your_api_key>'. If you need to create an API key, you can go so at tychos.ai")
-        url = f'{self.base_url}datasets'
+        url = f'{self.base_url}vector_data_store/list'
         headers = {'api_key': self.api_key}
         response = requests.get(url=url, headers=headers)
 
         # error handling
         response.raise_for_status()
 
         return response.json()
```

### Comparing `tychos-0.0.89/tychos.egg-info/PKG-INFO` & `tychos-0.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: tychos
-Version: 0.0.89
-Summary: Python client library for the Tychos API.
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
 To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
@@ -48,20 +40,14 @@
 ```
 
 Query live vector datasets
 ```python
 # initialize data store
 data_store = tychos.VectorDataStore()
 
-# list available datasets
-datasets = data_store.list()
-
-# get name of the first dataset's id
-print(datasets['data'][0]['name'])
-
 # query the data store object
 query_results = data_store.query(
     index_name = "pub-med-abstracts", # dataset
     query_string = "What is the latest research on molecular peptides", # search string
     limit = 5, # number of results
 )
 
@@ -74,18 +60,18 @@
 
 ```sh
 tychos-cli query --api-key <YOUR-API-KEY> --name pub-med-abstracts --query-string <"Your query string"> --limit 5
 
 ```
 
 ## Datasets available
-We currently support a handful of research datasets. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
+We currently support the PubMed dataset and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
 
 ### Vector datasets
--   PubMed abstracts ([source][pub-med]): 33.2M documents, updated daily at 07:00 UTC.
+-   PubMed abstracts ([source][pub-med]): 33.8M documents, updated daily at 07:00 UTC.
 
 
 
 ## Feedback and support
 If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise an issue via GitHub.
```

