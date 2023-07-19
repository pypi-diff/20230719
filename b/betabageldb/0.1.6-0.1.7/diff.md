# Comparing `tmp/betabageldb-0.1.6.tar.gz` & `tmp/betabageldb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.6.tar", last modified: Fri Jul 14 10:36:14 2023, max compression
+gzip compressed data, was "betabageldb-0.1.7.tar", last modified: Wed Jul 19 09:08:02 2023, max compression
```

## Comparing `betabageldb-0.1.6.tar` & `betabageldb-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-14 10:36:14.012907 betabageldb-0.1.6/
--rw-r--r--   0 bidhan     (501) staff       (20)     2234 2023-07-14 10:36:14.012684 betabageldb-0.1.6/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     1679 2023-07-14 10:25:37.000000 betabageldb-0.1.6/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-14 10:36:14.012364 betabageldb-0.1.6/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     2234 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      192 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-14 10:36:14.012946 betabageldb-0.1.6/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)     1624 2023-07-14 10:33:33.000000 betabageldb-0.1.6/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.869695 betabageldb-0.1.7/
+-rw-r--r--   0 bidhan     (501) staff       (20)     2837 2023-07-19 09:08:02.869354 betabageldb-0.1.7/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     2283 2023-07-19 08:55:03.000000 betabageldb-0.1.7/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.862606 betabageldb-0.1.7/bagel/
+-rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.864490 betabageldb-0.1.7/bagel/api/
+-rw-r--r--   0 bidhan     (501) staff       (20)    10695 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/api/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    12159 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/api/fastapi.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/api/types.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     6274 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/config.py
+-rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/errors.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.865719 betabageldb-0.1.7/bagel/utils/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/utils/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11810 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/utils/embedding_utils.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.868786 betabageldb-0.1.7/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     2837 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      359 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-19 09:08:02.869749 betabageldb-0.1.7/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1641 2023-07-19 09:07:59.000000 betabageldb-0.1.7/setup.py
```

### Comparing `betabageldb-0.1.6/PKG-INFO` & `betabageldb-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,116 +1,120 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.6
+Version: 0.1.7
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # BagelDB Python Client Example
 
-This README provides steps on how to use the BagelDB python client example code.
+Welcome to the BagelDB Python Client Example! BagelDB is your bread-and-butter library for interacting with the BagelDB API without breaking a sweat. 
+
+One of the perks? **No need to call the OpenAI Embeddings method or any other model to generate embeddings!** That's right, the BagelDB client handles that for you. So, you don't need to spend extra bucks on generating embeddings. Quite a dough-saver, isn't it? 🥯💰
 
 ## Prerequisites
 
 - Python 3.6+
 - pip package manager
 - BagelDB account and API key
 
 ## Installation
 
-Install the BagelDB python client:
+To install the BagelDB Python client, run the following command in your terminal:
 
-```
-pip install bagel
+```shell
+pip install betabageldb
 ```
 
 ## Usage
 
-1. Import the necessary modules:
+1. **Import the necessary modules:**
 
 ```python
 import uuid
 import bagel
 from bagel.config import Settings
 ```
 
-2. Define the BagelDB server settings:
+2. **Define the BagelDB server settings:**
 
 ```python 
 server_settings = Settings(
     bagel_api_impl="rest",
     bagel_server_host="api2.bageldb.ai",
     bagel_server_http_port="8000"
 )
 ```
 
-3. Create the BagelDB client:
+3. **Create the BagelDB client:**
 
 ```python
 client = bagel.Client(server_settings)
 ```
 
-4. Ping the BagelDB server:
+4. **Ping the BagelDB server:**
 
 ```python
 print(client.ping())
 ```
 
-5. Get the BagelDB server version:
+5. **Get the BagelDB server version:**
 
 ```python
 print(client.get_version()) 
 ```
 
-6. Create and delete a cluster:
+6. **Create and delete a cluster:**
 
 ```python
 name = str(uuid.uuid4())
 client.create_cluster(name)
 client.delete_cluster(name)
 ```
 
-7. Create, add documents, and query a cluster:
+7. **Create, add documents, and query a cluster:**
 
 ```python
 cluster = client.get_or_create_cluster("testing")
 
 cluster.add(documents=["doc1", "doc2"]) 
 
 results = cluster.find(query_texts=["query"], n_results=5)
 ```
 
-8. Add embeddings and query:
+8. **Add embeddings and query (without needing to generate embeddings yourself!):**
 
 ```python
 cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]])
 
 results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2) 
 ```
 
-9. Modify cluster name:
+9. **Modify cluster name:**
 
 ```python 
 cluster.modify(name="new_name")
 ```
 
-10. Update document metadata:
+10. **Update document metadata:**
 
 ```python
 cluster.update(ids=["doc1"], metadatas=[{"new":"metadata"}])
 ```
 
-11. Upsert documents:
+11. **Upsert documents:**
 
 ```python
 cluster.upsert(documents=["new doc"], ids=["doc1"])
 ```
 
-See the [example code](paste.txt) for more details on using the BagelDB python client.
+Need more dough-tails? See the [example code](example.py) for a more comprehensive guide on using the BagelDB Python client.
+
+Happy coding and enjoy your fresh Bagels! 🥯👩‍💻👨‍💻
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `betabageldb-0.1.6/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.1.7/betabageldb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,116 +1,120 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.6
+Version: 0.1.7
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # BagelDB Python Client Example
 
-This README provides steps on how to use the BagelDB python client example code.
+Welcome to the BagelDB Python Client Example! BagelDB is your bread-and-butter library for interacting with the BagelDB API without breaking a sweat. 
+
+One of the perks? **No need to call the OpenAI Embeddings method or any other model to generate embeddings!** That's right, the BagelDB client handles that for you. So, you don't need to spend extra bucks on generating embeddings. Quite a dough-saver, isn't it? 🥯💰
 
 ## Prerequisites
 
 - Python 3.6+
 - pip package manager
 - BagelDB account and API key
 
 ## Installation
 
-Install the BagelDB python client:
+To install the BagelDB Python client, run the following command in your terminal:
 
-```
-pip install bagel
+```shell
+pip install betabageldb
 ```
 
 ## Usage
 
-1. Import the necessary modules:
+1. **Import the necessary modules:**
 
 ```python
 import uuid
 import bagel
 from bagel.config import Settings
 ```
 
-2. Define the BagelDB server settings:
+2. **Define the BagelDB server settings:**
 
 ```python 
 server_settings = Settings(
     bagel_api_impl="rest",
     bagel_server_host="api2.bageldb.ai",
     bagel_server_http_port="8000"
 )
 ```
 
-3. Create the BagelDB client:
+3. **Create the BagelDB client:**
 
 ```python
 client = bagel.Client(server_settings)
 ```
 
-4. Ping the BagelDB server:
+4. **Ping the BagelDB server:**
 
 ```python
 print(client.ping())
 ```
 
-5. Get the BagelDB server version:
+5. **Get the BagelDB server version:**
 
 ```python
 print(client.get_version()) 
 ```
 
-6. Create and delete a cluster:
+6. **Create and delete a cluster:**
 
 ```python
 name = str(uuid.uuid4())
 client.create_cluster(name)
 client.delete_cluster(name)
 ```
 
-7. Create, add documents, and query a cluster:
+7. **Create, add documents, and query a cluster:**
 
 ```python
 cluster = client.get_or_create_cluster("testing")
 
 cluster.add(documents=["doc1", "doc2"]) 
 
 results = cluster.find(query_texts=["query"], n_results=5)
 ```
 
-8. Add embeddings and query:
+8. **Add embeddings and query (without needing to generate embeddings yourself!):**
 
 ```python
 cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]])
 
 results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2) 
 ```
 
-9. Modify cluster name:
+9. **Modify cluster name:**
 
 ```python 
 cluster.modify(name="new_name")
 ```
 
-10. Update document metadata:
+10. **Update document metadata:**
 
 ```python
 cluster.update(ids=["doc1"], metadatas=[{"new":"metadata"}])
 ```
 
-11. Upsert documents:
+11. **Upsert documents:**
 
 ```python
 cluster.upsert(documents=["new doc"], ids=["doc1"])
 ```
 
-See the [example code](paste.txt) for more details on using the BagelDB python client.
+Need more dough-tails? See the [example code](example.py) for a more comprehensive guide on using the BagelDB Python client.
+
+Happy coding and enjoy your fresh Bagels! 🥯👩‍💻👨‍💻
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `betabageldb-0.1.6/betabageldb.egg-info/requires.txt` & `betabageldb-0.1.7/betabageldb.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.6/setup.py` & `betabageldb-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="betabageldb",
-    version="0.1.6",
+    version="0.1.7",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
-    py_modules=["BagelDB"],
+    packages=find_packages(),
     install_requires=[
         "annotated-types==0.5.0",
         "backoff==2.2.1",
         "certifi==2023.5.7",
         "charset-normalizer==3.2.0",
         "colorama==0.4.6",
         "coloredlogs==15.0.1",
```

