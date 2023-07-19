# Comparing `tmp/nids_transformers-0.0.6.tar.gz` & `tmp/nids_transformers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_transformers-0.0.6.tar", last modified: Wed Jul 19 02:03:57 2023, max compression
+gzip compressed data, was "nids_transformers-0.0.7.tar", last modified: Wed Jul 19 02:16:10 2023, max compression
```

## Comparing `nids_transformers-0.0.6.tar` & `nids_transformers-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 02:03:57.454589 nids_transformers-0.0.6/
--rw-r--r--   0 rdp        (501) staff       (20)      178 2023-07-19 01:47:15.000000 nids_transformers-0.0.6/MANIFEST.in
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 02:03:57.454327 nids_transformers-0.0.6/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-19 01:11:31.000000 nids_transformers-0.0.6/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 02:03:57.453085 nids_transformers-0.0.6/nids_transformers/
--rw-r--r--   0 rdp        (501) staff       (20)  5495089 2023-07-06 03:59:04.000000 nids_transformers-0.0.6/nids_transformers/CORPUS.txt
--rw-r--r--   0 rdp        (501) staff       (20)  1585280 2023-07-19 01:16:55.000000 nids_transformers-0.0.6/nids_transformers/KMEANS-CLUSTER-CENTERS.npy
--rw-r--r--   0 rdp        (501) staff       (20)    10034 2023-07-19 02:03:37.000000 nids_transformers-0.0.6/nids_transformers/NIDSTransformers.py
--rw-r--r--   0 rdp        (501) staff       (20)    23489 2023-07-19 01:14:48.000000 nids_transformers-0.0.6/nids_transformers/SCALER.pkl
--rw-r--r--   0 rdp        (501) staff       (20)  3170432 2023-07-19 01:17:11.000000 nids_transformers-0.0.6/nids_transformers/TAGS-NAMES-EMBEDDINGS.npy
--rw-r--r--   0 rdp        (501) staff       (20)       35 2023-07-19 00:52:36.000000 nids_transformers-0.0.6/nids_transformers/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 02:03:57.454087 nids_transformers-0.0.6/nids_transformers.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 02:03:57.000000 nids_transformers-0.0.6/nids_transformers.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      449 2023-07-19 02:03:57.000000 nids_transformers-0.0.6/nids_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-19 02:03:57.000000 nids_transformers-0.0.6/nids_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      177 2023-07-19 02:03:57.000000 nids_transformers-0.0.6/nids_transformers.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       18 2023-07-19 02:03:57.000000 nids_transformers-0.0.6/nids_transformers.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-19 02:03:57.454643 nids_transformers-0.0.6/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      924 2023-07-19 02:03:48.000000 nids_transformers-0.0.6/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 02:16:10.739337 nids_transformers-0.0.7/
+-rw-r--r--   0 rdp        (501) staff       (20)      178 2023-07-19 01:47:15.000000 nids_transformers-0.0.7/MANIFEST.in
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 02:16:10.738883 nids_transformers-0.0.7/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-19 01:11:31.000000 nids_transformers-0.0.7/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 02:16:10.732861 nids_transformers-0.0.7/nids_transformers/
+-rw-r--r--   0 rdp        (501) staff       (20)  5495089 2023-07-06 03:59:04.000000 nids_transformers-0.0.7/nids_transformers/CORPUS.txt
+-rw-r--r--   0 rdp        (501) staff       (20)  1585280 2023-07-19 01:16:55.000000 nids_transformers-0.0.7/nids_transformers/KMEANS-CLUSTER-CENTERS.npy
+-rw-r--r--   0 rdp        (501) staff       (20)    10034 2023-07-19 02:03:37.000000 nids_transformers-0.0.7/nids_transformers/NIDSTransformers.py
+-rw-r--r--   0 rdp        (501) staff       (20)    23489 2023-07-19 01:14:48.000000 nids_transformers-0.0.7/nids_transformers/SCALER.pkl
+-rw-r--r--   0 rdp        (501) staff       (20)  3170432 2023-07-19 01:17:11.000000 nids_transformers-0.0.7/nids_transformers/TAGS-NAMES-EMBEDDINGS.npy
+-rw-r--r--   0 rdp        (501) staff       (20)       35 2023-07-19 00:52:36.000000 nids_transformers-0.0.7/nids_transformers/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 02:16:10.737927 nids_transformers-0.0.7/nids_transformers.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 02:16:10.000000 nids_transformers-0.0.7/nids_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      449 2023-07-19 02:16:10.000000 nids_transformers-0.0.7/nids_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-19 02:16:10.000000 nids_transformers-0.0.7/nids_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      212 2023-07-19 02:16:10.000000 nids_transformers-0.0.7/nids_transformers.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       18 2023-07-19 02:16:10.000000 nids_transformers-0.0.7/nids_transformers.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-19 02:16:10.739495 nids_transformers-0.0.7/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      924 2023-07-19 02:16:01.000000 nids_transformers-0.0.7/setup.py
```

### Comparing `nids_transformers-0.0.6/PKG-INFO` & `nids_transformers-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids_transformers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tag Generation and Text Generation for Network Packets using Transformers
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: NIDS Transformers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_transformers-0.0.6/nids_transformers/CORPUS.txt` & `nids_transformers-0.0.7/nids_transformers/CORPUS.txt`

 * *Files identical despite different names*

### Comparing `nids_transformers-0.0.6/nids_transformers/KMEANS-CLUSTER-CENTERS.npy` & `nids_transformers-0.0.7/nids_transformers/KMEANS-CLUSTER-CENTERS.npy`

 * *Files identical despite different names*

### Comparing `nids_transformers-0.0.6/nids_transformers/NIDSTransformers.py` & `nids_transformers-0.0.7/nids_transformers/NIDSTransformers.py`

 * *Files identical despite different names*

### Comparing `nids_transformers-0.0.6/nids_transformers/SCALER.pkl` & `nids_transformers-0.0.7/nids_transformers/SCALER.pkl`

 * *Files identical despite different names*

### Comparing `nids_transformers-0.0.6/nids_transformers/TAGS-NAMES-EMBEDDINGS.npy` & `nids_transformers-0.0.7/nids_transformers/TAGS-NAMES-EMBEDDINGS.npy`

 * *Files identical despite different names*

### Comparing `nids_transformers-0.0.6/nids_transformers.egg-info/PKG-INFO` & `nids_transformers-0.0.7/nids_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids-transformers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tag Generation and Text Generation for Network Packets using Transformers
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: NIDS Transformers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_transformers-0.0.6/setup.py` & `nids_transformers-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_transformers',
-    version='0.0.6',
+    version='0.0.7',
     description="Tag Generation and Text Generation for Network Packets using Transformers",
     keywords="NIDS Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

