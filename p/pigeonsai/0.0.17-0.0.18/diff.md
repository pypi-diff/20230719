# Comparing `tmp/pigeonsai-0.0.17.tar.gz` & `tmp/pigeonsai-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.17.tar", last modified: Wed Jul 19 04:57:53 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.18.tar", last modified: Wed Jul 19 13:50:24 2023, max compression
```

## Comparing `pigeonsai-0.0.17.tar` & `pigeonsai-0.0.18.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.644374 pigeonsai-0.0.17/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-07-19 04:57:53.644226 pigeonsai-0.0.17/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.17/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-07-19 04:57:53.644420 pigeonsai-0.0.17/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2065 2023-07-19 04:57:36.000000 pigeonsai-0.0.17/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.640925 pigeonsai-0.0.17/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.642153 pigeonsai-0.0.17/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       50 2023-06-15 18:46:00.000000 pigeonsai-0.0.17/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     7826 2023-07-19 04:56:41.000000 pigeonsai-0.0.17/src/pigeonsai/pigeonsdb.py
--rw-r--r--   0 ariaattar   (501) staff       (20)      710 2023-07-19 03:40:55.000000 pigeonsai-0.0.17/src/pigeonsai/utils.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.643825 pigeonsai-0.0.17/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      302 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       90 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.643964 pigeonsai-0.0.17/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.17/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 13:50:24.290836 pigeonsai-0.0.18/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-07-19 13:50:24.290698 pigeonsai-0.0.18/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.18/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-07-19 13:50:24.290880 pigeonsai-0.0.18/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2065 2023-07-19 13:50:13.000000 pigeonsai-0.0.18/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 13:50:24.288818 pigeonsai-0.0.18/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 13:50:24.289554 pigeonsai-0.0.18/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       50 2023-06-15 18:46:00.000000 pigeonsai-0.0.18/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     8373 2023-07-19 13:49:54.000000 pigeonsai-0.0.18/src/pigeonsai/pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 13:50:24.290300 pigeonsai-0.0.18/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-07-19 13:50:24.000000 pigeonsai-0.0.18/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-07-19 13:50:24.000000 pigeonsai-0.0.18/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-07-19 13:50:24.000000 pigeonsai-0.0.18/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       90 2023-07-19 13:50:24.000000 pigeonsai-0.0.18/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-07-19 13:50:24.000000 pigeonsai-0.0.18/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 13:50:24.290430 pigeonsai-0.0.18/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.18/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.17/PKG-INFO` & `pigeonsai-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.17
+Version: 0.0.18
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.17/README.md` & `pigeonsai-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.17/setup.py` & `pigeonsai-0.0.18/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.17",
+    version="0.0.18",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.17/src/pigeonsai/pigeonsdb.py` & `pigeonsai-0.0.18/src/pigeonsai/pigeonsdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests
 import json
 import warnings
 from tenacity import retry, wait_exponential, stop_after_attempt
 from tqdm import tqdm
-from utils import _get_db_info
 
 warnings.filterwarnings("ignore")
 
 API_URL = "http://test-search-1248249294.us-east-2.elb.amazonaws.com:8080/search"
 API_URL_TEST = "http://172.30.36.170:3000/api/v1"
 GET_DB_INFO_API = "https://api.pigeonsai.com/api/v1/sdk/get-db-info"
 ADD_API_URL = "http://add-dev-177401989.us-east-2.elb.amazonaws.com:8080/add_documents"
@@ -160,14 +159,32 @@
                 response = response.json()
                 print('Res:', response.get('Message'))
         except Exception as e:
             raise PigeonsDBError(f"Error occurred while deleting a db instance.")
 
 
 
+def _get_db_info(api_key: str, dbname: str):
+    url = GET_DB_INFO_API
+    headers = {"Content-Type": "application/json"}
+    data = {"api_key": api_key, "dbname": dbname}
+    response = requests.post(url, headers=headers, data=json.dumps(data))
+
+    if response.status_code != 200:
+        raise PigeonsDBError("API_KEY or db_name doesn't match.")
+
+    db_info = response.json().get('DB info', {})
+    index_p = db_info.get('s3_identifier')
+    keys = ['dbname', 'user', 'password', 'host']
+    connect = {key: db_info.get(key) for key in keys}
+
+    return index_p, connect
+
+
+
 class SemanticChunking:
 
     def ada(text, min_tokens, max_tokens):
         # Tokenize the text into sentences
         sentences = sent_tokenize(text)
         print(sentences)
         # Convert sentences to embeddings using a pre-trained model
```

### Comparing `pigeonsai-0.0.17/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.18/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.17
+Version: 0.0.18
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.17/tests/test_pigeonsdb.py` & `pigeonsai-0.0.18/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

