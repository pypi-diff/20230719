# Comparing `tmp/getpaper-0.2.4.tar.gz` & `tmp/getpaper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.2.4.tar", last modified: Thu Jun 29 13:17:31 2023, max compression
+gzip compressed data, was "getpaper-0.2.5.tar", last modified: Wed Jul 19 00:03:02 2023, max compression
```

## Comparing `getpaper-0.2.4.tar` & `getpaper-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 13:17:31.175314 getpaper-0.2.4/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.2.4/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5155 2023-06-29 13:17:31.175314 getpaper-0.2.4/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4540 2023-06-29 07:41:46.000000 getpaper-0.2.4/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 13:17:31.175314 getpaper-0.2.4/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.2.4/getpaper/__init__.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.2.4/getpaper/clean.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1020 2023-06-29 07:49:25.000000 getpaper-0.2.4/getpaper/config.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12926 2023-06-29 13:16:29.000000 getpaper-0.2.4/getpaper/download.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6845 2023-06-29 10:57:47.000000 getpaper-0.2.4/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12854 2023-06-29 07:52:58.000000 getpaper-0.2.4/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5052 2023-06-29 10:54:05.000000 getpaper-0.2.4/getpaper/splitting.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 13:17:31.175314 getpaper-0.2.4/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5155 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      233 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-29 13:17:31.175314 getpaper-0.2.4/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1627 2023-06-29 12:53:37.000000 getpaper-0.2.4/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-19 00:03:02.160500 getpaper-0.2.5/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.2.5/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5477 2023-07-19 00:03:02.160500 getpaper-0.2.5/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4862 2023-07-18 23:54:32.000000 getpaper-0.2.5/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-19 00:03:02.160500 getpaper-0.2.5/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.2.5/getpaper/__init__.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.2.5/getpaper/clean.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1020 2023-06-29 07:49:25.000000 getpaper-0.2.5/getpaper/config.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12926 2023-06-29 13:16:29.000000 getpaper-0.2.5/getpaper/download.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    11962 2023-07-18 23:57:16.000000 getpaper-0.2.5/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12854 2023-06-29 07:52:58.000000 getpaper-0.2.5/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5052 2023-06-29 10:54:05.000000 getpaper-0.2.5/getpaper/splitting.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-19 00:03:02.160500 getpaper-0.2.5/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5477 2023-07-19 00:03:02.000000 getpaper-0.2.5/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-07-19 00:03:02.000000 getpaper-0.2.5/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-07-19 00:03:02.000000 getpaper-0.2.5/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-07-19 00:03:02.000000 getpaper-0.2.5/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      247 2023-07-19 00:03:02.000000 getpaper-0.2.5/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-07-19 00:03:02.000000 getpaper-0.2.5/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-07-19 00:03:02.160500 getpaper-0.2.5/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1666 2023-07-19 00:01:43.000000 getpaper-0.2.5/setup.py
```

### Comparing `getpaper-0.2.4/LICENSE` & `getpaper-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.4/PKG-INFO` & `getpaper-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.2.4
+Version: 0.2.5
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -104,19 +104,27 @@
 getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
+It is possible to use both Chroma and Qdrant. To use qdrant we provide docker-compose file to set it up:
+```bash
+cd services
+docker compose -f docker-compose.yaml up
+getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection mypapers --chunk_size 6000 --database Qdrant
+```
+
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
 
 index.py has local dependencies on other modules, for this reason if you are running it inside getpaper project folder consider having it installed locally:
```

### Comparing `getpaper-0.2.4/README.md` & `getpaper-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,19 +86,27 @@
 getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
+It is possible to use both Chroma and Qdrant. To use qdrant we provide docker-compose file to set it up:
+```bash
+cd services
+docker compose -f docker-compose.yaml up
+getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection mypapers --chunk_size 6000 --database Qdrant
+```
+
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
 
 index.py has local dependencies on other modules, for this reason if you are running it inside getpaper project folder consider having it installed locally:
```

### Comparing `getpaper-0.2.4/getpaper/clean.py` & `getpaper-0.2.5/getpaper/clean.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.4/getpaper/config.py` & `getpaper-0.2.5/getpaper/config.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.4/getpaper/download.py` & `getpaper-0.2.5/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.4/getpaper/parse.py` & `getpaper-0.2.5/getpaper/parse.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.4/getpaper/splitting.py` & `getpaper-0.2.5/getpaper/splitting.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.4/getpaper.egg-info/PKG-INFO` & `getpaper-0.2.5/getpaper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.2.4
+Version: 0.2.5
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -104,19 +104,27 @@
 getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
+It is possible to use both Chroma and Qdrant. To use qdrant we provide docker-compose file to set it up:
+```bash
+cd services
+docker compose -f docker-compose.yaml up
+getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection mypapers --chunk_size 6000 --database Qdrant
+```
+
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
 
 index.py has local dependencies on other modules, for this reason if you are running it inside getpaper project folder consider having it installed locally:
```

### Comparing `getpaper-0.2.4/setup.py` & `getpaper-0.2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
@@ -19,15 +19,16 @@
     author_email="<antonkulaga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['pyfunctional', 'more-itertools', 'click', 'python-dotenv', 'tiktoken', 'pynction',
                       'unstructured', 'unstructured-inference', 'unstructured[local-inference]', 'unstructured.PaddleOCR',
-                      'scidownl', 'langchain', 'openai', 'chromadb', 'Deprecated', 'semanticscholar', 'pdfminer', 'loguru'],
+                      'scidownl', 'langchain', 'openai', 'Deprecated', 'semanticscholar', 'pdfminer', 'loguru',
+                      'qdrant-client', 'chromadb'],
     keywords=['python', 'utils', 'files', 'papers', 'download'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
```

