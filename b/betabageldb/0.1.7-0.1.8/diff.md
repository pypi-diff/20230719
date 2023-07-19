# Comparing `tmp/betabageldb-0.1.7.tar.gz` & `tmp/betabageldb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.7.tar", last modified: Wed Jul 19 09:08:02 2023, max compression
+gzip compressed data, was "betabageldb-0.1.8.tar", last modified: Wed Jul 19 09:42:49 2023, max compression
```

## Comparing `betabageldb-0.1.7.tar` & `betabageldb-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.869695 betabageldb-0.1.7/
--rw-r--r--   0 bidhan     (501) staff       (20)     2837 2023-07-19 09:08:02.869354 betabageldb-0.1.7/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     2283 2023-07-19 08:55:03.000000 betabageldb-0.1.7/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.862606 betabageldb-0.1.7/bagel/
--rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.864490 betabageldb-0.1.7/bagel/api/
--rw-r--r--   0 bidhan     (501) staff       (20)    10695 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/api/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    12159 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/api/fastapi.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/api/types.py
--rw-r--r--   0 bidhan     (501) staff       (20)     6274 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/config.py
--rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/errors.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.865719 betabageldb-0.1.7/bagel/utils/
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/utils/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11810 2023-07-19 08:55:03.000000 betabageldb-0.1.7/bagel/utils/embedding_utils.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:08:02.868786 betabageldb-0.1.7/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     2837 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      359 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-07-19 09:08:02.000000 betabageldb-0.1.7/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-19 09:08:02.869749 betabageldb-0.1.7/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)     1641 2023-07-19 09:07:59.000000 betabageldb-0.1.7/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:49.197704 betabageldb-0.1.8/
+-rw-r--r--   0 bidhan     (501) staff       (20)     2837 2023-07-19 09:42:49.197379 betabageldb-0.1.8/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     2283 2023-07-19 08:55:03.000000 betabageldb-0.1.8/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:49.177189 betabageldb-0.1.8/bagel/
+-rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:49.187199 betabageldb-0.1.8/bagel/api/
+-rw-r--r--   0 bidhan     (501) staff       (20)    10695 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/api/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    12159 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/api/fastapi.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:49.188130 betabageldb-0.1.8/bagel/api/models/
+-rw-r--r--   0 bidhan     (501) staff       (20)    15111 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/api/models/Cluster.py
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:32.000000 betabageldb-0.1.8/bagel/api/models/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/api/types.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     6274 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/config.py
+-rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/errors.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:49.193954 betabageldb-0.1.8/bagel/utils/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/utils/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11810 2023-07-19 08:55:03.000000 betabageldb-0.1.8/bagel/utils/embedding_utils.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:49.196173 betabageldb-0.1.8/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     2837 2023-07-19 09:42:49.000000 betabageldb-0.1.8/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      416 2023-07-19 09:42:49.000000 betabageldb-0.1.8/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-19 09:42:49.000000 betabageldb-0.1.8/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-19 09:42:49.000000 betabageldb-0.1.8/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-07-19 09:42:49.000000 betabageldb-0.1.8/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-19 09:42:49.197744 betabageldb-0.1.8/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1641 2023-07-19 09:42:43.000000 betabageldb-0.1.8/setup.py
```

### Comparing `betabageldb-0.1.7/PKG-INFO` & `betabageldb-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.7
+Version: 0.1.8
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betabageldb-0.1.7/README.md` & `betabageldb-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/__init__.py` & `betabageldb-0.1.8/bagel/__init__.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/api/__init__.py` & `betabageldb-0.1.8/bagel/api/__init__.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/api/fastapi.py` & `betabageldb-0.1.8/bagel/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/api/types.py` & `betabageldb-0.1.8/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/config.py` & `betabageldb-0.1.8/bagel/config.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/errors.py` & `betabageldb-0.1.8/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/bagel/utils/embedding_utils.py` & `betabageldb-0.1.8/bagel/utils/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.1.8/betabageldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.7
+Version: 0.1.8
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betabageldb-0.1.7/betabageldb.egg-info/requires.txt` & `betabageldb-0.1.8/betabageldb.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.7/setup.py` & `betabageldb-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betabageldb",
-    version="0.1.7",
+    version="0.1.8",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
     packages=find_packages(),
```

