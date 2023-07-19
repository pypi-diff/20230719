# Comparing `tmp/wafermap-clustering-0.3.1.tar.gz` & `tmp/wafermap-clustering-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.1.tar", last modified: Wed Jul 19 09:51:45 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.2.tar", last modified: Wed Jul 19 11:23:58 2023, max compression
```

## Comparing `wafermap-clustering-0.3.1.tar` & `wafermap-clustering-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.272672 wafermap-clustering-0.3.1/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-07-19 09:51:45.270732 wafermap-clustering-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 09:51:45.273460 wafermap-clustering-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-07-19 09:51:12.000000 wafermap-clustering-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.223244 wafermap-clustering-0.3.1/tests/
--rw-rw-rw-   0        0        0     9509 2023-07-19 09:46:50.000000 wafermap-clustering-0.3.1/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.227244 wafermap-clustering-0.3.1/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.251235 wafermap-clustering-0.3.1/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.1/wafermap_clustering/configs/config.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.255366 wafermap-clustering-0.3.1/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4479 2023-07-19 09:07:18.000000 wafermap-clustering-0.3.1/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.267732 wafermap-clustering-0.3.1/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.1/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.1/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.1/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5621 2023-07-19 09:43:06.000000 wafermap-clustering-0.3.1/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.247276 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.119009 wafermap-clustering-0.3.2/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-07-19 11:23:58.115833 wafermap-clustering-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 11:23:58.119509 wafermap-clustering-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-07-19 11:22:19.000000 wafermap-clustering-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.060281 wafermap-clustering-0.3.2/tests/
+-rw-rw-rw-   0        0        0     9509 2023-07-19 09:46:50.000000 wafermap-clustering-0.3.2/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.066882 wafermap-clustering-0.3.2/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.093060 wafermap-clustering-0.3.2/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.2/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.097368 wafermap-clustering-0.3.2/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4479 2023-07-19 09:07:18.000000 wafermap-clustering-0.3.2/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.109879 wafermap-clustering-0.3.2/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.2/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.2/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.2/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5621 2023-07-19 09:43:06.000000 wafermap-clustering-0.3.2/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:23:58.089196 wafermap-clustering-0.3.2/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-19 11:23:57.000000 wafermap-clustering-0.3.2/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-19 11:23:58.000000 wafermap-clustering-0.3.2/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 11:23:57.000000 wafermap-clustering-0.3.2/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-19 11:23:57.000000 wafermap-clustering-0.3.2/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-19 11:23:57.000000 wafermap-clustering-0.3.2/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.1/LICENSE.txt` & `wafermap-clustering-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.1/PKG-INFO` & `wafermap-clustering-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.1
+Version: 0.3.2
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.1.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.1/setup.py` & `wafermap-clustering-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.1"
+version = "0.3.2"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.1/tests/test_clustering.py` & `wafermap-clustering-0.3.2/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.1/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.2/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.1/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.3.2/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.1/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.2/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.1/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.2/wafermap_clustering/wafermap_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.1/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.2/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.1
+Version: 0.3.2
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.1.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.1/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.2/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

