# Comparing `tmp/modnet-0.3.0.tar.gz` & `tmp/modnet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modnet-0.3.0.tar", last modified: Thu Jun  1 14:29:47 2023, max compression
+gzip compressed data, was "dist/modnet-0.4.0.tar", last modified: Wed Jul 19 13:06:53 2023, max compression
```

## Comparing `modnet-0.3.0.tar` & `modnet-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.3.0/LICENSE.md
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.3.0/MANIFEST.in
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6122 2023-06-01 14:29:47.000000 modnet-0.3.0/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4238 2023-05-08 13:57:20.000000 modnet-0.3.0/README.md
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-06-01 14:27:20.000000 modnet-0.3.0/modnet/__init__.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/data/
--rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.3.0/modnet/data/Features_cross
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.3.0/modnet/ext_data.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/featurizers/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.3.0/modnet/featurizers/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    12289 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/featurizers.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/featurizers/presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9990 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/featurizers/presets/debreuck_2020.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9213 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/presets/matminer_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    15893 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/featurizers/presets/matminer_all_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      492 2021-09-08 13:24:57.000000 modnet-0.3.0/modnet/featurizers/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/hyper_opt/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.3.0/modnet/hyper_opt/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    27252 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/hyper_opt/fit_genetic.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/matbench/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.3.0/modnet/matbench/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-06-01 13:18:02.000000 modnet-0.3.0/modnet/matbench/benchmark.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/model_presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.3.0/modnet/model_presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.3.0/modnet/model_presets/presets.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/models/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.3.0/modnet/models/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    15042 2022-08-30 16:25:35.000000 modnet-0.3.0/modnet/models/bayesian.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17880 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/models/ensemble.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    39117 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/models/vanilla.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    41703 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.3.0/modnet/sklearn.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet/tests/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.3.0/modnet/tests/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/tests/conftest.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/tests/test_benchmark.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.3.0/modnet/tests/test_ext_data.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2023-06-01 14:25:56.000000 modnet-0.3.0/modnet/tests/test_hyper_opt.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-01-23 13:07:39.000000 modnet-0.3.0/modnet/tests/test_model.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    18202 2023-06-01 13:18:02.000000 modnet-0.3.0/modnet/tests/test_preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.3.0/modnet/tests/test_sklearn.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.3.0/modnet/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6122 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/SOURCES.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/dependency_links.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      192 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/requires.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-06-01 14:29:47.000000 modnet-0.3.0/modnet.egg-info/top_level.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-06-01 14:29:47.000000 modnet-0.3.0/setup.cfg
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1961 2023-02-09 15:34:41.000000 modnet-0.3.0/setup.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.0/LICENSE.md
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.0/MANIFEST.in
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-19 13:06:53.000000 modnet-0.4.0/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.0/README.md
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-07-13 18:46:04.000000 modnet-0.4.0/modnet/__init__.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/data/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.0/modnet/data/Features_cross
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.0/modnet/ext_data.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/featurizers/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.0/modnet/featurizers/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    12289 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/featurizers.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/featurizers/presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9990 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/debreuck_2020.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9213 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/matminer_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    15893 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/matminer_all_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      492 2021-09-08 13:24:57.000000 modnet-0.4.0/modnet/featurizers/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/hyper_opt/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.0/modnet/hyper_opt/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    27253 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/hyper_opt/fit_genetic.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/matbench/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.0/modnet/matbench/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/matbench/benchmark.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/model_presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.0/modnet/model_presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.0/modnet/model_presets/presets.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/models/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.4.0/modnet/models/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    14851 2023-07-11 14:46:35.000000 modnet-0.4.0/modnet/models/bayesian.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17885 2023-07-13 18:28:15.000000 modnet-0.4.0/modnet/models/ensemble.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    59819 2023-07-14 09:39:48.000000 modnet-0.4.0/modnet/models/vanilla.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    41703 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.4.0/modnet/sklearn.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/tests/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.0/modnet/tests/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/conftest.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/test_benchmark.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.0/modnet/tests/test_ext_data.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/test_hyper_opt.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/test_model.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    18202 2023-07-11 13:24:52.000000 modnet-0.4.0/modnet/tests/test_preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.0/modnet/tests/test_sklearn.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.0/modnet/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet.egg-info/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/SOURCES.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/dependency_links.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      223 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/requires.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/top_level.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-07-19 13:06:53.000000 modnet-0.4.0/setup.cfg
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2085 2023-07-11 13:21:01.000000 modnet-0.4.0/setup.py
```

### Comparing `modnet-0.3.0/LICENSE.md` & `modnet-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/PKG-INFO` & `modnet-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.3.0
+Version: 0.4.0
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
-Description: # MODNet: Material Optimal Descriptor Network
+Description: <div align="center">
+            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+            <br>
+        
+        # MODNet: Material Optimal Descriptor Network
         
         [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
         
-        <p align="center">
-            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
-            <br>
-        </p>
+        </div>
         
         <a name="introduction"></a>
         ## Introduction
         This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
         It is a supervised machine learning framework for **learning material properties** from
         either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
         and can be used for learning *multiple* properties together by using **joint learning**.
```

### Comparing `modnet-0.3.0/README.md` & `modnet-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+<div align="center">
+    <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+    <br>
+
 # MODNet: Material Optimal Descriptor Network
 
 [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
 
-<p align="center">
-    <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
-    <br>
-</p>
+</div>
 
 <a name="introduction"></a>
 ## Introduction
 This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
 It is a supervised machine learning framework for **learning material properties** from
 either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
 and can be used for learning *multiple* properties together by using **joint learning**.
```

### Comparing `modnet-0.3.0/modnet/data/Features_cross` & `modnet-0.4.0/modnet/data/Features_cross`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/ext_data.py` & `modnet-0.4.0/modnet/ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/featurizers/featurizers.py` & `modnet-0.4.0/modnet/featurizers/featurizers.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/featurizers/presets/__init__.py` & `modnet-0.4.0/modnet/featurizers/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/featurizers/presets/debreuck_2020.py` & `modnet-0.4.0/modnet/featurizers/presets/debreuck_2020.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/featurizers/presets/matminer_2023.py` & `modnet-0.4.0/modnet/featurizers/presets/matminer_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/featurizers/presets/matminer_all_2023.py` & `modnet-0.4.0/modnet/featurizers/presets/matminer_all_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/hyper_opt/fit_genetic.py` & `modnet-0.4.0/modnet/hyper_opt/fit_genetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,15 +655,15 @@
             self.best_model = self.best_individual.refit_model(
                 self.data, n_models=refit, n_jobs=n_jobs or 1, fast=fast
             )
 
         else:
             ensemble = []
             for m in models[ranking[:refit]]:
-                ensemble += m.model
+                ensemble += m.models
             self.best_model = EnsembleMODNetModel(models=ensemble)
 
         self.results = self.best_individual.genes
 
         return self.best_model
```

### Comparing `modnet-0.3.0/modnet/matbench/benchmark.py` & `modnet-0.4.0/modnet/matbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/model_presets/presets.py` & `modnet-0.4.0/modnet/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/models/bayesian.py` & `modnet-0.4.0/modnet/models/bayesian.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,16 +90,16 @@
 
         self._scaler = None
         self.optimal_descriptors = None
         self.target_names = None
         self.targets = targets
         self.model = None
 
-        f_temp = [x for subl in targets for x in subl]
-        self.targets_flatten = [x for subl in f_temp for x in subl]
+        self.targets_groups = [x for subl in targets for x in subl]
+        self.targets_flatten = [x for subl in self.targets_groups for x in subl]
         self.num_classes = {name: 0 for name in self.targets_flatten}
         if num_classes is not None:
             self.num_classes.update(num_classes)
         self._multi_target = len(self.targets_flatten) > 1
         self.multi_label = False  # forced for compatibility with vanilla
 
         self.model = self.build_model(
@@ -225,60 +225,57 @@
                     previous_layer = tf.keras.layers.BatchNormalization()(
                         previous_layer
                     )
             intermediate_models_out.append(previous_layer)
 
         # Build outputs
         final_out = []
+        output_names = []
         for group_idx, group in enumerate(targets):
             for prop_idx in range(len(group)):
                 previous_layer = intermediate_models_out[group_idx]
                 for k in range(num_layers[2]):
                     if bayesian_layers[2][k]:
                         previous_layer = bayesian_layer(num_neurons[2][k])(
                             previous_layer
                         )
                     else:
                         previous_layer = dense_layer(num_neurons[2][k])(previous_layer)
                     if self._multi_target:
                         previous_layer = tf.keras.layers.BatchNormalization()(
                             previous_layer
                         )
-                clayer = previous_layer
-                for pi in range(len(group[prop_idx])):
-                    previous_layer = clayer
-                    for li in range(num_layers[3]):
-                        if bayesian_layers[3][li]:
-                            previous_layer = bayesian_layer(num_neurons[3][li])(
-                                previous_layer
-                            )
-                        else:
-                            previous_layer = dense_layer(num_neurons[3][li])(
-                                previous_layer
-                            )
-                    n = num_classes[group[prop_idx][pi]]
-                    if n >= 2:
-                        out = tfp.layers.DenseVariational(
-                            n,
-                            make_posterior_fn=posterior,
-                            make_prior_fn=prior,
-                            kl_weight=kl_weight,
-                            activation="softmax",
-                            name=group[prop_idx][pi],
-                        )(previous_layer)
-                    else:
-                        out = tfp.layers.DenseVariational(
-                            1,
-                            make_posterior_fn=posterior,
-                            make_prior_fn=prior,
-                            kl_weight=kl_weight,
-                            activation=out_act,
-                            name=group[prop_idx][pi],
-                        )(previous_layer)
-                    final_out.append(out)
+                n = num_classes[group[prop_idx][0]]
+                name = group[prop_idx][0]
+                if n >= 2:
+                    out = tfp.layers.DenseVariational(
+                        n,
+                        make_posterior_fn=posterior,
+                        make_prior_fn=prior,
+                        kl_weight=kl_weight,
+                        activation="softmax",
+                        name=name,
+                    )(previous_layer)
+                else:
+                    out = tfp.layers.DenseVariational(
+                        len(group[prop_idx]),
+                        make_posterior_fn=posterior,
+                        make_prior_fn=prior,
+                        kl_weight=kl_weight,
+                        activation=out_act,
+                        name=name,
+                    )(previous_layer)
+                final_out.append(out)
+                output_names.append(name)
+
+        new_weights = dict()
+        for n in output_names:
+            w = self.weights.get(n, 1)
+            new_weights[n] = w
+        self.weights = new_weights
 
         return tf.keras.models.Model(inputs=f_input, outputs=final_out)
 
     def predict(
         self, test_data: MODData, return_prob=False, return_unc=False
     ) -> pd.DataFrame:
         """Predict the target values for the passed MODData.
@@ -312,21 +309,22 @@
             x = self._scaler.transform(x)
             x = np.nan_to_num(x)
 
         all_predictions = []
 
         for i in range(1000):
             p = self.model.predict(x)
-            if len(self.targets_flatten) == 1:
+            if len(self.targets_groups) == 1:
                 p = np.array([p])
             all_predictions.append(p)
 
         p_dic = {}
         unc_dic = {}
-        for i, name in enumerate(self.targets_flatten):
+        for i, props in enumerate(self.targets_groups):
+            name = props[0]
             if self.num_classes[name] >= 2:
                 if return_prob:
                     preds = np.array([pred[i] for pred in all_predictions])
                     probs = preds / (preds.sum(axis=-1)).reshape((-1, 1))
                     mean_prob = probs.mean()
                     std_prob = probs.std()
                     for j in range(mean_prob.shape[-1]):
@@ -338,18 +336,23 @@
                         axis=1,
                     )
                     unc_dic[name] = np.max(
                         np.array([pred[i] for pred in all_predictions]).mean(axis=0),
                         axis=1,
                     )
             else:
-                mean_p = np.array([pred[i] for pred in all_predictions]).mean(axis=0)
-                std_p = np.array([pred[i] for pred in all_predictions]).std(axis=0)
-                p_dic[name] = mean_p[:, 0]
-                unc_dic[name] = std_p[:, 0]
+                for j, name in enumerate(props):
+                    mean_p = np.array([pred[i][:, j] for pred in all_predictions]).mean(
+                        axis=0
+                    )
+                    std_p = np.array([pred[i][:, j] for pred in all_predictions]).std(
+                        axis=0
+                    )
+                    p_dic[name] = mean_p
+                    unc_dic[name] = std_p
 
         predictions = pd.DataFrame(p_dic)
         unc = pd.DataFrame(unc_dic)
 
         predictions.index = test_data.structure_ids
         unc.index = test_data.structure_ids
```

### Comparing `modnet-0.3.0/modnet/models/ensemble.py` & `modnet-0.4.0/modnet/models/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,30 +428,29 @@
             m._make_picklable()
 
     def _restore_model(self):
         """
         restore inner keras model after running make_picklable
         """
 
+        # backward compatibility for loading models saved <v0.3
+        if not hasattr(self, "models") and hasattr(self, "model"):
+            self.models = self.model
+
         for m in self.models:
             m._restore_model()
 
     def _get_param_names(self):
         possible_params = [
             "n_models",
             "bootstrap",
             "models",
         ]
         return possible_params
 
-    @property
-    def model(self) -> List[MODNetModel]:
-        """Returns the inner MODNet models. For Backward compatability only."""
-        return self.models
-
 
 def _validate_ensemble_model(
     train_data=None,
     val_data=None,
     targets=None,
     weights=None,
     n_models=5,
```

### Comparing `modnet-0.3.0/modnet/models/vanilla.py` & `modnet-0.4.0/modnet/models/vanilla.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         self.impute_missing = None
         self._scale_impute = None
         self.optimal_descriptors = None
         self.target_names = None
         self.targets = targets
         self.model = None
 
-        f_temp = [x for subl in targets for x in subl]
-        self.targets_flatten = [x for subl in f_temp for x in subl]
+        self.targets_groups = [x for subl in targets for x in subl]
+        self.targets_flatten = [x for subl in self.targets_groups for x in subl]
         self.num_classes = {name: 0 for name in self.targets_flatten}
         if num_classes is not None:
             self.num_classes.update(num_classes)
         self._multi_target = len(self.targets_flatten) > 1
 
         self.model = self.build_model(
             targets,
@@ -175,47 +175,97 @@
                     previous_layer = tf.keras.layers.BatchNormalization()(
                         previous_layer
                     )
             intermediate_models_out.append(previous_layer)
 
         # Build outputs
         final_out = []
+        output_names = []
         for group_idx, group in enumerate(targets):
             for prop_idx in range(len(group)):
                 previous_layer = intermediate_models_out[group_idx]
                 for k in range(num_layers[2]):
                     previous_layer = tf.keras.layers.Dense(
                         num_neurons[2][k], activation=act
                     )(previous_layer)
                     if self._multi_target:
                         previous_layer = tf.keras.layers.BatchNormalization()(
                             previous_layer
                         )
-                clayer = previous_layer
-                for pi in range(len(group[prop_idx])):
-                    previous_layer = clayer
-                    for li in range(num_layers[3]):
-                        previous_layer = tf.keras.layers.Dense(num_neurons[3][li])(
-                            previous_layer
-                        )
-                    n = num_classes[group[prop_idx][pi]]
-                    if n >= 2:
-                        out = tf.keras.layers.Dense(
-                            n,
-                            activation="sigmoid" if multi_label else "softmax",
-                            name=group[prop_idx][pi],
-                        )(previous_layer)
-                    else:
-                        out = tf.keras.layers.Dense(
-                            1, activation=out_act, name=group[prop_idx][pi]
-                        )(previous_layer)
-                    final_out.append(out)
+
+                n = num_classes[group[prop_idx][0]]
+                name = group[prop_idx][0]
+                if n >= 2:
+                    out = tf.keras.layers.Dense(
+                        n,
+                        activation="sigmoid" if multi_label else "softmax",
+                        name=name,
+                    )(previous_layer)
+                else:
+                    out = tf.keras.layers.Dense(
+                        len(group[prop_idx]),
+                        activation=out_act,
+                        name=name,
+                    )(previous_layer)
+                final_out.append(out)
+                output_names.append(name)
+
+        new_weights = dict()
+        for n in output_names:
+            w = self.weights.get(n, 1)
+            new_weights[n] = w
+        self.weights = new_weights
 
         return tf.keras.models.Model(inputs=f_input, outputs=final_out)
 
+    def _set_scale_impute(
+        self, impute_missing, xscale_before_impute, scaler=None, imputer=None
+    ):
+        """
+        Sets the inner scaling and imputer mechanism.
+        impute_missing: Determines how the NaN features are treated.
+                If str, defines the strategy used in the scikit-learn SimpleImputer,
+                e.g., "mean" sets the NaNs to the mean of their feature column.
+                If a float is provided, this float is used to replace NaNs in the original dataset.
+        xscale_before_impute: whether to first scale the input and then impute values, or
+                first impute values and then scale the inputs.
+        scaler: optional sklearn scaler to use
+        imputer: optional sklearn imputer to use
+        """
+        # Define the scaler
+        if scaler is not None:
+            self._scaler = scaler
+        elif self.xscale == "minmax":
+            self._scaler = MinMaxScaler(feature_range=(-0.5, 0.5))
+
+        elif self.xscale == "standard":
+            self._scaler = StandardScaler()
+
+        # Define the imputer
+        if imputer is not None:
+            self._imputer = imputer
+        elif isinstance(impute_missing, str):
+            self._imputer = SimpleImputer(
+                missing_values=np.nan, strategy=impute_missing
+            )
+        else:
+            self._imputer = SimpleImputer(
+                missing_values=np.nan, strategy="constant", fill_value=impute_missing
+            )
+
+        # Scale and impute input features in the desired order
+        if xscale_before_impute:
+            self._scale_impute = Pipeline(
+                [("scaler", self._scaler), ("imputer", self._imputer)]
+            )
+        else:
+            self._scale_impute = Pipeline(
+                [("imputer", self._imputer), ("scaler", self._scaler)]
+            )
+
     def fit(
         self,
         training_data: MODData,
         custom_data: Optional[np.ndarray] = None,
         val_fraction: float = 0.0,
         val_key: Optional[str] = None,
         val_data: Optional[MODData] = None,
@@ -289,112 +339,95 @@
         if (
             len(self.targets_flatten) == 1
             and len(training_data.df_targets.columns) == 1
         ):
             self.targets_flatten = list(training_data.df_targets.columns)
 
         y = []
-        for targ in self.targets_flatten:
-            if self.num_classes[targ] >= 2:  # Classification
+        for prop in self.targets_groups:
+            if self.num_classes[prop[0]] >= 2:  # Classification
+                targ = prop[0]
                 if self.multi_label:
                     y_inner = np.stack(training_data.df_targets[targ].values)
                     if loss is None:
                         loss = "binary_crossentropy"
                 else:
                     y_inner = tf.keras.utils.to_categorical(
                         training_data.df_targets[targ].values,
                         num_classes=self.num_classes[targ],
                     )
                     if loss is None:
                         loss = "categorical_crossentropy"
             else:
-                y_inner = training_data.df_targets[targ].values.astype(
+
+                y_inner = training_data.df_targets[prop].values.astype(
                     np.float64, copy=False
                 )
             if custom_data is not None:
                 val_data = None
                 val_fraction = 0
                 metrics = []
                 y_inner = np.hstack(
                     (
                         np.reshape(y_inner, (len(y_inner), -1)),
                         custom_data.reshape((len(custom_data), -1)),
                     )
                 )
             y.append(y_inner)
 
-        # Define the scaler
+        # set scaler and imputer
         if self.xscale == "minmax":
-            self._scaler = MinMaxScaler(feature_range=(-0.5, 0.5))
-
+            impute_missing = -1 if xscale_before_impute else impute_missing
         elif self.xscale == "standard":
-            self._scaler = StandardScaler()
-
-        # Define the imputer
-        if isinstance(impute_missing, str):
-            self._imputer = SimpleImputer(
-                missing_values=np.nan, strategy=impute_missing
-            )
-        else:
-            if self.xscale == "minmax":
-                impute_missing = -1 if xscale_before_impute else impute_missing
-            elif self.xscale == "standard":
-                impute_missing = (
-                    10 * np.max(np.nan_to_num(StandardScaler().fit_transform(x)))
-                    if xscale_before_impute
-                    else impute_missing
-                )
-            self.impute_missing = impute_missing
-
-            self._imputer = SimpleImputer(
-                missing_values=np.nan, strategy="constant", fill_value=impute_missing
-            )
-
-        # Scale and impute input features in the desired order
-        if xscale_before_impute:
-            self._scale_impute = Pipeline(
-                [("scaler", self._scaler), ("imputer", self._imputer)]
-            )
-        else:
-            self._scale_impute = Pipeline(
-                [("imputer", self._imputer), ("scaler", self._scaler)]
+            impute_missing = (
+                10 * np.max(np.nan_to_num(StandardScaler().fit_transform(x)))
+                if xscale_before_impute
+                else impute_missing
             )
+        self.impute_missing = impute_missing
+        self._set_scale_impute(
+            impute_missing=impute_missing, xscale_before_impute=xscale_before_impute
+        )
 
         x = self._scale_impute.fit_transform(x)
 
         if val_data is not None:
             val_x = val_data.get_featurized_df()[
                 self.optimal_descriptors[: self.n_feat]
             ].values
             val_x = self._scale_impute.transform(val_x)
             val_y = []
-            for targ in self.targets_flatten:
-                if self.num_classes[targ] >= 2:  # Classification
+            for prop in self.targets_groups:
+                if self.num_classes[prop[0]] >= 2:  # Classification
+                    targ = prop[0]
                     if self.multi_label:
                         y_inner = np.stack(val_data.df_targets[targ].values)
                         if loss is None:
                             loss = "binary_crossentropy"
                     else:
                         y_inner = tf.keras.utils.to_categorical(
                             val_data.df_targets[targ].values,
                             num_classes=self.num_classes[targ],
                         )
+                        loss = "categorical_crossentropy"
                 else:
-                    y_inner = val_data.df_targets[targ].values.astype(
+                    y_inner = val_data.df_targets[prop].values.astype(
                         np.float64, copy=False
                     )
                 val_y.append(y_inner)
             validation_data = (val_x, val_y)
         else:
             validation_data = None
 
         # set up bounds for postprocessing
-        if max(self.num_classes.values()) <= 2:  # regression
-            self.min_y = training_data.df_targets.values.min(axis=0)
-            self.max_y = training_data.df_targets.values.max(axis=0)
+        self.min_y = []
+        self.max_y = []
+        for prop in self.targets_groups:
+            self.min_y.append(training_data.df_targets[prop].values.min(axis=0))
+            self.max_y.append(training_data.df_targets[prop].values.max(axis=0))
 
         # Optionally set up print callback
         if verbose:
             if val_fraction > 0 or validation_data:
                 if self._multi_target and val_key is not None:
                     val_metric_key = f"val_{val_key}_mae"
                 else:
@@ -637,15 +670,15 @@
                 out_act=self.out_act,
                 num_classes=self.num_classes,
             ).model
             self.n_feat = n_feat
             self.fit(
                 data,
                 val_fraction=0,
-                lr=best_preset["lr"],
+                learning_rate=best_preset["lr"],
                 epochs=best_preset["epochs"],
                 batch_size=best_preset["batch_size"],
                 loss=best_preset["loss"],
                 callbacks=callbacks,
                 verbose=verbose,
                 **fit_params,
             )
@@ -681,46 +714,49 @@
             .values
         )
 
         # Scale and impute input features:
         if self._scale_impute is not None:
             x = self._scale_impute.transform(x)
 
-        p = np.array(self.model.predict(x))
+        p = self.model.predict(x)
 
-        if len(p.shape) == 2:
-            p = np.array([p])
+        if len(self.targets_groups) == 1:
+            p = [p]
 
         # post-process based on training data
         if max(self.num_classes.values()) <= 2:  # regression
-            yrange = self.max_y - self.min_y
-            upper_bound = self.max_y + 0.25 * yrange
-            lower_bound = self.min_y - 0.25 * yrange
             for i, vals in enumerate(p):
-                out_of_range_idxs = np.where(
-                    (vals < lower_bound[i]) | (vals > upper_bound[i])
-                )
-                vals[out_of_range_idxs] = (
-                    np.random.uniform(0, 1, size=len(out_of_range_idxs[0]))
-                    * (self.max_y[i] - self.min_y[i])
-                    + self.min_y[i]
-                )
+                yrange = self.max_y[i] - self.min_y[i]
+                upper_bound = self.max_y[i] + 0.25 * yrange
+                lower_bound = self.min_y[i] - 0.25 * yrange
+                for j in range(len(self.targets_groups[i])):
+                    out_of_range_idxs = np.where(
+                        (vals[:, j] < lower_bound[j]) | (vals[:, j] > upper_bound[j])
+                    )
+                    vals[out_of_range_idxs, j] = (
+                        np.random.uniform(0, 1, size=len(out_of_range_idxs[0]))
+                        * (yrange[j])
+                        + self.min_y[i][j]
+                    )
 
         p_dic = {}
-        for i, name in enumerate(self.targets_flatten):
+
+        for i, props in enumerate(self.targets_groups):
+            name = props[0]
             if self.num_classes[name] >= 2:
                 if return_prob:
-                    # temp = p[i, :, :] / (p[i, :, :].sum(axis=1)).reshape((-1, 1))
-                    temp = p[i, :, :]
+                    temp = p[i]
                     for j in range(temp.shape[-1]):
                         p_dic["{}_prob_{}".format(name, j)] = temp[:, j]
                 else:
-                    p_dic[name] = np.argmax(p[i, :, :], axis=1)
+                    p_dic[name] = np.argmax(p[i], axis=1)
             else:
-                p_dic[name] = p[i, :, 0]
+                for j, name in enumerate(props):
+                    p_dic[name] = p[i][:, j]
         predictions = pd.DataFrame(p_dic)
         predictions.index = test_data.structure_ids
 
         return predictions
 
     def evaluate(self, test_data: MODData) -> pd.DataFrame:
         """Evaluates predictions on the passed MODData by returning the corresponding score:
@@ -743,20 +779,22 @@
             .values
         )
 
         # Scale and impute input features:
         if self._scale_impute is not None:
             x = self._scale_impute.transform(x)
 
-        y_pred = np.array(self.model.predict(x))
-        if len(y_pred.shape) == 2:
-            y_pred = np.array([y_pred])
+        y_pred = self.model.predict(x)
+        if len(self.targets_groups) == 1:
+            y_pred = [y_pred]
+
         score = []
-        for i, targ in enumerate(self.targets_flatten):
-            if self.num_classes[targ] >= 2:  # Classification
+        for i, prop in enumerate(self.targets_groups):
+            if self.num_classes[prop[0]] >= 2:  # Classification
+                targ = prop[0]
                 if self.multi_label:
                     y_true = np.stack(test_data.df_targets[targ].values)
                 else:
                     y_true = tf.keras.utils.to_categorical(
                         test_data.df_targets[targ].values,
                         num_classes=self.num_classes[targ],
                     )
@@ -767,15 +805,15 @@
                     for j in range(y_true.shape[1]):
                         try:
                             scores.append(-roc_auc_score(y_true[:, j], y_pred[i][:, j]))
                         except ValueError:
                             scores.append(float("nan"))
                     score.append(np.nanmean(scores))
             else:
-                y_true = test_data.df_targets[targ].values.astype(
+                y_true = test_data.df_targets[prop].values.astype(
                     np.float64, copy=False
                 )
                 score.append(mean_absolute_error(y_true, y_pred[i]))
 
         return np.mean(score)
 
     def _make_picklable(self):
@@ -792,14 +830,26 @@
         """
         restore inner keras model after running make_picklable
         """
 
         model_json, model_weights = self.model
         self.model = tf.keras.models.model_from_json(model_json)
         self.model.set_weights(model_weights)
+        if not hasattr(self, "_scale_impute"):
+            self.xscale = "minmax"
+            self._set_scale_impute(
+                impute_missing=-1,
+                xscale_before_impute=True,
+                scaler=self._scaler,
+                imputer=SimpleImputer(
+                    missing_values=np.nan,
+                    strategy="constant",
+                    fill_value=-1,
+                ).fit(np.zeros((1, self.n_feat))),
+            )
 
     def save(self, filename: str) -> None:
         """Save the `MODNetModel` to filename:
 
         If the filename ends in "tgz", "bz2" or "zip", the pickle
         will be compressed accordingly by :meth:`pandas.DataFrame.to_pickle`.
 
@@ -849,14 +899,31 @@
         if isinstance(pickled_data, MODNetModel):
             if not hasattr(pickled_data, "__modnet_version__"):
                 pickled_data.__modnet_version__ = "unknown"
             pickled_data._restore_model()
             LOG.info(
                 f"Loaded {pickled_data} object, created with modnet version {pickled_data.__modnet_version__}"
             )
+            if hasattr(pickled_data, "models"):
+                for i, m in enumerate(pickled_data.models):  # ensemble
+                    if not hasattr(m, "targets_groups"):
+                        LOG.warning(
+                            "Loaded model is old (v<0.4.0) and will not be supported in the future (v1.0.0 onward). Please consider retraining your model!\nLoaded with DepractedMODNetModel."
+                        )
+                        recovered_data = DeprecatedMODNetModel(targets=[], weights={})
+                        recovered_data.__dict__ = m.__dict__.copy()
+                        pickled_data.models[i] = recovered_data
+            else:
+                if not hasattr(pickled_data, "targets_groups"):  # single model
+                    LOG.warning(
+                        "Loaded model is old (v<0.4.0) and will not be supported in the future (v1.0.0 onward). Please consider retraining your model!\nLoaded with DepractedMODNetModel."
+                    )
+                    recovered_data = DeprecatedMODNetModel(targets=[], weights={})
+                    recovered_data.__dict__ = pickled_data.__dict__.copy()
+                    pickled_data.model = recovered_data
             return pickled_data
 
         raise ValueError(
             f"File {filename} did not contain compatible data to create a MODNetModel object, "
             f"instead found {pickled_data.__class__.__name__}."
         )
 
@@ -960,14 +1027,435 @@
                 )
                 key = "estimator"
             valid_params[key].set_params(**sub_params)
 
         return self
 
 
+class DeprecatedMODNetModel(MODNetModel):
+    def build_model(
+        self,
+        targets: List,
+        n_feat: int,
+        num_neurons: Tuple[List[int], List[int], List[int], List[int]],
+        num_classes: Optional[Dict[str, int]] = None,
+        multi_label: Optional[bool] = False,
+        act: str = "relu",
+        out_act: str = "linear",
+    ):
+        """Builds the tf.keras model and sets the `self.model` attribute.
+
+        Parameters:
+            targets: A nested list of targets names that defines the hierarchy
+                of the output layers.
+            n_feat: The number of features to use as model inputs.
+            num_neurons: A specification of the model layers, as a 4-tuple
+                of lists of integers. Hidden layers are split into four
+                blocks of `tf.keras.layers.Dense`, with neuron count specified
+                by the elements of the `num_neurons` argument.
+            num_classes: Dictionary defining the target types (classification or regression).
+                Should be constructed as follows: key: string giving the target name; value: integer n,
+                with n=0 for regression and n>=2 for classification with n the number of classes.
+            multi_label: Whether the problem (if classification) is multi-label.
+                In this case the softmax output-activation is replaced by a sigmoid.
+            act: A string defining a tf.keras activation function to pass to use
+                in the `tf.keras.layers.Dense` layers.
+            out_act: A string defining a tf.keras activation function to pass to use
+                for the last output layer (regression only)
+
+        """
+
+        num_layers = [len(x) for x in num_neurons]
+
+        # Build first common block
+        f_input = tf.keras.layers.Input(shape=(n_feat,))
+        previous_layer = f_input
+        for i in range(num_layers[0]):
+            previous_layer = tf.keras.layers.Dense(num_neurons[0][i], activation=act)(
+                previous_layer
+            )
+            if self._multi_target:
+                previous_layer = tf.keras.layers.BatchNormalization()(previous_layer)
+        common_out = previous_layer
+
+        # Build intermediate representations
+        intermediate_models_out = []
+        for _ in range(len(targets)):
+            previous_layer = common_out
+            for j in range(num_layers[1]):
+                previous_layer = tf.keras.layers.Dense(
+                    num_neurons[1][j], activation=act
+                )(previous_layer)
+                if self._multi_target:
+                    previous_layer = tf.keras.layers.BatchNormalization()(
+                        previous_layer
+                    )
+            intermediate_models_out.append(previous_layer)
+
+        # Build outputs
+        final_out = []
+        for group_idx, group in enumerate(targets):
+            for prop_idx in range(len(group)):
+                previous_layer = intermediate_models_out[group_idx]
+                for k in range(num_layers[2]):
+                    previous_layer = tf.keras.layers.Dense(
+                        num_neurons[2][k], activation=act
+                    )(previous_layer)
+                    if self._multi_target:
+                        previous_layer = tf.keras.layers.BatchNormalization()(
+                            previous_layer
+                        )
+                clayer = previous_layer
+                for pi in range(len(group[prop_idx])):
+                    previous_layer = clayer
+                    for li in range(num_layers[3]):
+                        previous_layer = tf.keras.layers.Dense(num_neurons[3][li])(
+                            previous_layer
+                        )
+                    n = num_classes[group[prop_idx][pi]]
+                    if n >= 2:
+                        out = tf.keras.layers.Dense(
+                            n,
+                            activation="sigmoid" if multi_label else "softmax",
+                            name=group[prop_idx][pi],
+                        )(previous_layer)
+                    else:
+                        out = tf.keras.layers.Dense(
+                            1, activation=out_act, name=group[prop_idx][pi]
+                        )(previous_layer)
+                    final_out.append(out)
+
+        return tf.keras.models.Model(inputs=f_input, outputs=final_out)
+
+    def fit(
+        self,
+        training_data: MODData,
+        custom_data: Optional[np.ndarray] = None,
+        val_fraction: float = 0.0,
+        val_key: Optional[str] = None,
+        val_data: Optional[MODData] = None,
+        lr: float = 0.001,
+        epochs: int = 200,
+        batch_size: int = 128,
+        xscale: Optional[str] = "minmax",
+        impute_missing: Optional[Union[float, str]] = 0,
+        xscale_before_impute: bool = True,
+        metrics: List[str] = ["mae"],
+        callbacks: List[Callable] = None,
+        verbose: int = 0,
+        loss: str = None,
+        **fit_params,
+    ) -> None:
+        """Train the model on the passed training `MODData` object.
+
+        Parameters:
+            training_data: A `MODData` that has been featurized and
+                feature selected. The first `self.n_feat` entries in
+                `training_data.get_optimal_descriptors()` will be used
+                for training.
+            custom_data (np.ndarray): Optional array of shape (n_sampels, n_custom_props) that will be appended to the targets (columns wise).
+                This can be useful for defining custom loss functions.
+            val_fraction: The fraction of the training data to use as a
+                validation set for tracking model performance during
+                training.
+            val_key: The target name to track on the validation set
+                during training, if performing multi-target learning.
+            lr: The learning rate.
+            epochs: The maximum number of epochs to train for.
+            batch_size: The batch size to use for training.
+            xscale: The feature scaler to use, either `None`,
+                `'minmax'` or `'standard'`.
+            impute_missing: Determines how the NaN features are treated.
+                If str, defines the strategy used in the scikit-learn SimpleImputer,
+                e.g., "mean" sets the NaNs to the mean of their feature column.
+                If a float is provided, and if xscale_before_impute is False, this
+                float is used to replace NaNs in the original dataset.
+                If a float is provided but xscale_before_impute is True, the float
+                is not used and standard values are used.
+                If you want to do something more sophisticated, make your own
+                modifications to MODData.df_featurized before fitting the model.
+            xscale_before_impute: whether to first scale the input and then impute values, or
+                first impute values and then scale the inputs.
+            metrics: A list of tf.keras metrics to pass to `compile(...)`.
+            loss: The built-in tf.keras loss to pass to `compile(...)`.
+            fit_params: Any additional parameters to pass to `fit(...)`,
+                these will be overwritten by the explicit keyword
+                arguments above.
+
+        """
+
+        if self.n_feat > len(training_data.get_optimal_descriptors()):
+            raise RuntimeError(
+                "The model requires more features than computed in data. "
+                f"Please reduce n_feat below or equal to {len(training_data.get_optimal_descriptors())}"
+            )
+
+        self.xscale = xscale
+        self.impute_missing = impute_missing
+        self.target_names = list(self.weights.keys())
+        self.optimal_descriptors = training_data.get_optimal_descriptors()
+
+        x = training_data.get_featurized_df()[
+            self.optimal_descriptors[: self.n_feat]
+        ].values
+
+        # For compatibility with MODNet 0.1.7; if there is only one target in the training data,
+        # use that for the name of the target too.
+        if (
+            len(self.targets_flatten) == 1
+            and len(training_data.df_targets.columns) == 1
+        ):
+            self.targets_flatten = list(training_data.df_targets.columns)
+
+        y = []
+        for targ in self.targets_flatten:
+            if self.num_classes[targ] >= 2:  # Classification
+                if self.multi_label:
+                    y_inner = np.stack(training_data.df_targets[targ].values)
+                    if loss is None:
+                        loss = "binary_crossentropy"
+                else:
+                    y_inner = tf.keras.utils.to_categorical(
+                        training_data.df_targets[targ].values,
+                        num_classes=self.num_classes[targ],
+                    )
+                    if loss is None:
+                        loss = "categorical_crossentropy"
+            else:
+                y_inner = training_data.df_targets[targ].values.astype(
+                    np.float64, copy=False
+                )
+            if custom_data is not None:
+                val_data = None
+                val_fraction = 0
+                metrics = []
+                y_inner = np.hstack(
+                    (
+                        np.reshape(y_inner, (len(y_inner), -1)),
+                        custom_data.reshape((len(custom_data), -1)),
+                    )
+                )
+            y.append(y_inner)
+
+        # set scaler and imputer
+        if self.xscale == "minmax":
+            impute_missing = -1 if xscale_before_impute else impute_missing
+        elif self.xscale == "standard":
+            impute_missing = (
+                10 * np.max(np.nan_to_num(StandardScaler().fit_transform(x)))
+                if xscale_before_impute
+                else impute_missing
+            )
+        self.impute_missing = impute_missing
+        self._set_scale_impute(
+            impute_missing=impute_missing, xscale_before_impute=xscale_before_impute
+        )
+
+        x = self._scale_impute.fit_transform(x)
+
+        if val_data is not None:
+            val_x = val_data.get_featurized_df()[
+                self.optimal_descriptors[: self.n_feat]
+            ].values
+            val_x = self._scale_impute.transform(val_x)
+            val_y = []
+            for targ in self.targets_flatten:
+                if self.num_classes[targ] >= 2:  # Classification
+                    if self.multi_label:
+                        y_inner = np.stack(val_data.df_targets[targ].values)
+                        if loss is None:
+                            loss = "binary_crossentropy"
+                    else:
+                        y_inner = tf.keras.utils.to_categorical(
+                            val_data.df_targets[targ].values,
+                            num_classes=self.num_classes[targ],
+                        )
+                else:
+                    y_inner = val_data.df_targets[targ].values.astype(
+                        np.float64, copy=False
+                    )
+                val_y.append(y_inner)
+            validation_data = (val_x, val_y)
+        else:
+            validation_data = None
+
+        # set up bounds for postprocessing
+        if max(self.num_classes.values()) <= 2:  # regression
+            self.min_y = training_data.df_targets.values.min(axis=0)
+            self.max_y = training_data.df_targets.values.max(axis=0)
+
+        # Optionally set up print callback
+        if verbose:
+            if val_fraction > 0 or validation_data:
+                if self._multi_target and val_key is not None:
+                    val_metric_key = f"val_{val_key}_mae"
+                else:
+                    val_metric_key = "val_mae"
+                print_callback = tf.keras.callbacks.LambdaCallback(
+                    on_epoch_end=lambda epoch, logs: print(
+                        f"epoch {epoch}: loss: {logs['loss']:.3f}, "
+                        f"val_loss:{logs['val_loss']:.3f} {val_metric_key}:{logs[val_metric_key]:.3f}"
+                    )
+                )
+
+            else:
+                print_callback = tf.keras.callbacks.LambdaCallback(
+                    on_epoch_end=lambda epoch, logs: print(
+                        f"epoch {epoch}: loss: {logs['loss']:.3f}"
+                    )
+                )
+
+            if callbacks is None:
+                callbacks = [print_callback]
+            else:
+                callbacks.append(print_callback)
+
+        fit_params_kw = {
+            "x": x,
+            "y": y,
+            "epochs": epochs,
+            "batch_size": batch_size,
+            "verbose": 0,
+            "validation_split": val_fraction,
+            "validation_data": validation_data,
+            "callbacks": callbacks,
+        }
+
+        fit_params.update(fit_params_kw)
+
+        if loss is None:
+            loss = "mse"
+        self.model.compile(
+            loss=loss,
+            optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=lr),
+            metrics=metrics,
+            loss_weights=self.weights,
+        )
+        history = self.model.fit(**fit_params)
+        self.history = history.history
+
+    def predict(self, test_data: MODData, return_prob=False) -> pd.DataFrame:
+        """Predict the target values for the passed MODData.
+
+        Parameters:
+            test_data: A featurized and feature-selected `MODData`
+                object containing the descriptors used in training.
+            return_prob: For a classification tasks only: whether to return the probability of each
+                class OR only return the most probable class.
+
+        Returns:
+            A `pandas.DataFrame` containing the predicted values of the targets.
+
+
+        """
+        # prevents Nan predictions if some features are inf
+        x = (
+            test_data.get_featurized_df()
+            .replace([np.inf, -np.inf], np.nan)[self.optimal_descriptors[: self.n_feat]]
+            .values
+        )
+
+        # Scale and impute input features:
+        if self._scale_impute is not None:
+            x = self._scale_impute.transform(x)
+
+        p = np.array(self.model.predict(x))
+
+        if len(p.shape) == 2:
+            p = np.array([p])
+
+        # post-process based on training data
+        if max(self.num_classes.values()) <= 2:  # regression
+            yrange = self.max_y - self.min_y
+            upper_bound = self.max_y + 0.25 * yrange
+            lower_bound = self.min_y - 0.25 * yrange
+            for i, vals in enumerate(p):
+                out_of_range_idxs = np.where(
+                    (vals < lower_bound[i]) | (vals > upper_bound[i])
+                )
+                vals[out_of_range_idxs] = (
+                    np.random.uniform(0, 1, size=len(out_of_range_idxs[0]))
+                    * (self.max_y[i] - self.min_y[i])
+                    + self.min_y[i]
+                )
+
+        p_dic = {}
+        for i, name in enumerate(self.targets_flatten):
+            if self.num_classes[name] >= 2:
+                if return_prob:
+                    # temp = p[i, :, :] / (p[i, :, :].sum(axis=1)).reshape((-1, 1))
+                    temp = p[i, :, :]
+                    for j in range(temp.shape[-1]):
+                        p_dic["{}_prob_{}".format(name, j)] = temp[:, j]
+                else:
+                    p_dic[name] = np.argmax(p[i, :, :], axis=1)
+            else:
+                p_dic[name] = p[i, :, 0]
+        predictions = pd.DataFrame(p_dic)
+        predictions.index = test_data.structure_ids
+
+        return predictions
+
+    def evaluate(self, test_data: MODData) -> pd.DataFrame:
+        """Evaluates predictions on the passed MODData by returning the corresponding score:
+            - for regression: MAE
+            - for classification: negative ROC AUC.
+            averaged over the targets when multi-target.
+
+        Parameters:
+            test_data: A featurized and feature-selected `MODData`
+                object containing the descriptors used in training.
+
+
+        Returns:
+            Score defined hereabove.
+        """
+        # prevents Nan predictions if some features are inf
+        x = (
+            test_data.get_featurized_df()
+            .replace([np.inf, -np.inf], np.nan)[self.optimal_descriptors[: self.n_feat]]
+            .values
+        )
+
+        # Scale and impute input features:
+        if self._scale_impute is not None:
+            x = self._scale_impute.transform(x)
+
+        y_pred = np.array(self.model.predict(x))
+        if len(y_pred.shape) == 2:
+            y_pred = np.array([y_pred])
+        score = []
+        for i, targ in enumerate(self.targets_flatten):
+            if self.num_classes[targ] >= 2:  # Classification
+                if self.multi_label:
+                    y_true = np.stack(test_data.df_targets[targ].values)
+                else:
+                    y_true = tf.keras.utils.to_categorical(
+                        test_data.df_targets[targ].values,
+                        num_classes=self.num_classes[targ],
+                    )
+                try:
+                    score.append(-roc_auc_score(y_true, y_pred[i], multi_class="ovr"))
+                except ValueError:
+                    scores = []
+                    for j in range(y_true.shape[1]):
+                        try:
+                            scores.append(-roc_auc_score(y_true[:, j], y_pred[i][:, j]))
+                        except ValueError:
+                            scores.append(float("nan"))
+                    score.append(np.nanmean(scores))
+            else:
+                y_true = test_data.df_targets[targ].values.astype(
+                    np.float64, copy=False
+                )
+                score.append(mean_absolute_error(y_true, y_pred[i]))
+
+        return np.mean(score)
+
+
 def validate_model(
     train_data=None,
     val_data=None,
     targets=None,
     weights=None,
     num_classes=None,
     n_feat=100,
```

### Comparing `modnet-0.3.0/modnet/preprocessing.py` & `modnet-0.4.0/modnet/preprocessing.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/sklearn.py` & `modnet-0.4.0/modnet/sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/conftest.py` & `modnet-0.4.0/modnet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/test_benchmark.py` & `modnet-0.4.0/modnet/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/test_ext_data.py` & `modnet-0.4.0/modnet/tests/test_ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/test_hyper_opt.py` & `modnet-0.4.0/modnet/tests/test_hyper_opt.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/test_model.py` & `modnet-0.4.0/modnet/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/test_preprocessing.py` & `modnet-0.4.0/modnet/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/tests/test_sklearn.py` & `modnet-0.4.0/modnet/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet/utils.py` & `modnet-0.4.0/modnet/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/modnet.egg-info/PKG-INFO` & `modnet-0.4.0/modnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.3.0
+Version: 0.4.0
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
-Description: # MODNet: Material Optimal Descriptor Network
+Description: <div align="center">
+            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
+            <br>
+        
+        # MODNet: Material Optimal Descriptor Network
         
         [![arXiv](https://img.shields.io/badge/arXiv-2004.14766-brightgreen)](https://arxiv.org/abs/2004.14766) [![Build Status](https://img.shields.io/github/actions/workflow/status/ppdebreuck/modnet/ci.yml?logo=github&branch=main)](https://github.com/ppdebreuck/modnet/actions?query=branch%3Amaster+) [![Read the Docs](https://img.shields.io/readthedocs/modnet)](https://modnet.readthedocs.io/en/latest/)
         
-        <p align="center">
-            <img src="img/modnet_logo.svg" alt="modnet-logo"  width=200>
-            <br>
-        </p>
+        </div>
         
         <a name="introduction"></a>
         ## Introduction
         This repository contains the Python (3.8+) package implementing the Material Optimal Descriptor Network (MODNet).
         It is a supervised machine learning framework for **learning material properties** from
         either the **composition** or  **crystal structure**. The framework is well suited for **limited datasets**
         and can be used for learning *multiple* properties together by using **joint learning**.
```

### Comparing `modnet-0.3.0/modnet.egg-info/SOURCES.txt` & `modnet-0.4.0/modnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modnet-0.3.0/setup.py` & `modnet-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         "pandas~=1.5",
         "tensorflow~=2.10",
         "tensorflow-probability~=0.18",
         "pymatgen>=2022.9",
         "matminer~=0.8",
         "numpy>=1.20",
         "scikit-learn~=1.1",
+        "emmet-core<0.57",  # Can remove after https://github.com/materialsproject/api/issues/819
+        "pydantic~=1.10",
     ],
     tests_require=tests_require,
     test_suite="modnet.tests",
     extras_require={
         "test": tests_require,
         "dev": dev_require,
     },
```

