# Comparing `tmp/pygod-0.4.0.tar.gz` & `tmp/pygod-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygod-0.4.0.tar", last modified: Tue May 16 06:56:29 2023, max compression
+gzip compressed data, was "pygod-1.0.0.tar", last modified: Wed Jul 19 06:34:24 2023, max compression
```

## Comparing `pygod-0.4.0.tar` & `pygod-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.603048 pygod-0.4.0/
--rw-r--r--   0 kayzliu    (501) staff       (20)     1320 2023-05-12 21:16:50.000000 pygod-0.4.0/LICENSE
--rw-r--r--   0 kayzliu    (501) staff       (20)      107 2023-05-12 21:16:50.000000 pygod-0.4.0/MANIFEST.in
--rw-r--r--   0 kayzliu    (501) staff       (20)    14042 2023-05-16 06:56:29.603136 pygod-0.4.0/PKG-INFO
--rw-r--r--   0 kayzliu    (501) staff       (20)    13013 2023-05-12 21:16:50.000000 pygod-0.4.0/README.rst
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.595928 pygod-0.4.0/pygod/
--rw-r--r--   0 kayzliu    (501) staff       (20)      139 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/__init__.py
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.599739 pygod-0.4.0/pygod/detector/
--rw-r--r--   0 kayzliu    (501) staff       (20)      601 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/__init__.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     8766 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/adone.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     4266 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/anomalous.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     7624 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/anomalydae.py
--rw-r--r--   0 kayzliu    (501) staff       (20)    23431 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/base.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     6033 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/cola.py
--rw-r--r--   0 kayzliu    (501) staff       (20)    10659 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/conad.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     6702 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/dominant.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     8574 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/done.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     7083 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/gaan.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     6345 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/gae.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     7843 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/guide.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     6278 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/ocgnn.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     5823 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/one.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     4221 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/radar.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     5354 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/scan.py
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.600062 pygod-0.4.0/pygod/generator/
--rw-r--r--   0 kayzliu    (501) staff       (20)       33 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/generator/__init__.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     5008 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/generator/outlier_generator.py
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.600369 pygod-0.4.0/pygod/metric/
--rw-r--r--   0 kayzliu    (501) staff       (20)       22 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/metric/__init__.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     3187 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/metric/metric.py
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.602545 pygod-0.4.0/pygod/nn/
--rw-r--r--   0 kayzliu    (501) staff       (20)      410 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/__init__.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     7221 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/adone.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     3543 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/anomalydae.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     2706 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/cola.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     2138 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/conv.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     2538 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/decoder.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     4568 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/dominant.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     7863 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/done.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     1509 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/encoder.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     3466 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/functional.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     4156 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/gaan.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     4341 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/gae.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     9378 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/guide.py
--rw-r--r--   0 kayzliu    (501) staff       (20)     3591 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/ocgnn.py
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.602926 pygod-0.4.0/pygod/utils/
--rw-r--r--   0 kayzliu    (501) staff       (20)       54 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/utils/__init__.py
--rw-r--r--   0 kayzliu    (501) staff       (20)      897 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/utils/score_converter.py
--rw-r--r--   0 kayzliu    (501) staff       (20)    11054 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/utils/utility.py
--rw-r--r--   0 kayzliu    (501) staff       (20)      556 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/version.py
-drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.596519 pygod-0.4.0/pygod.egg-info/
--rw-r--r--   0 kayzliu    (501) staff       (20)    14042 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/PKG-INFO
--rw-r--r--   0 kayzliu    (501) staff       (20)     1092 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/SOURCES.txt
--rw-r--r--   0 kayzliu    (501) staff       (20)        1 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/dependency_links.txt
--rw-r--r--   0 kayzliu    (501) staff       (20)       45 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/requires.txt
--rw-r--r--   0 kayzliu    (501) staff       (20)        6 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/top_level.txt
--rw-r--r--   0 kayzliu    (501) staff       (20)       44 2023-05-12 21:16:50.000000 pygod-0.4.0/requirements.txt
--rw-r--r--   0 kayzliu    (501) staff       (20)       80 2023-05-16 06:56:29.603371 pygod-0.4.0/setup.cfg
--rw-r--r--   0 kayzliu    (501) staff       (20)     1970 2023-05-12 21:16:50.000000 pygod-0.4.0/setup.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.727952 pygod-1.0.0/
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1320 2023-07-19 06:34:03.000000 pygod-1.0.0/LICENSE
+-rw-r--r--   0 kayzliu    (501) staff       (20)      107 2023-07-19 06:34:03.000000 pygod-1.0.0/MANIFEST.in
+-rw-r--r--   0 kayzliu    (501) staff       (20)    14281 2023-07-19 06:34:24.728028 pygod-1.0.0/PKG-INFO
+-rw-r--r--   0 kayzliu    (501) staff       (20)    13205 2023-07-19 06:34:03.000000 pygod-1.0.0/README.rst
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.721767 pygod-1.0.0/pygod/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      200 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/__init__.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.724994 pygod-1.0.0/pygod/detector/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      601 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     8766 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/adone.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4266 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/anomalous.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7624 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/anomalydae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)    23431 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/base.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6033 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/cola.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)    10659 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/conad.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6702 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/dominant.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     8574 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/done.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7083 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/gaan.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6345 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/gae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7843 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/guide.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6278 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/ocgnn.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     5823 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/one.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4221 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/radar.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     5354 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/detector/scan.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.725287 pygod-1.0.0/pygod/generator/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      172 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/generator/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     5008 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/generator/outlier_generator.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.725578 pygod-1.0.0/pygod/metric/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      300 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/metric/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3187 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/metric/metric.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.727441 pygod-1.0.0/pygod/nn/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      497 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7221 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/adone.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3543 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/anomalydae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2706 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/cola.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2138 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/conv.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2538 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/decoder.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4568 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/dominant.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7863 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/done.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1509 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/encoder.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3466 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/functional.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4156 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/gaan.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4341 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/gae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     9378 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/guide.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3591 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/nn/ocgnn.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.727829 pygod-1.0.0/pygod/utils/
+-rw-r--r--   0 kayzliu    (501) staff       (20)       82 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/utils/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)      897 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/utils/score_converter.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)    11054 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/utils/utility.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)      556 2023-07-19 06:34:03.000000 pygod-1.0.0/pygod/version.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-07-19 06:34:24.722478 pygod-1.0.0/pygod.egg-info/
+-rw-r--r--   0 kayzliu    (501) staff       (20)    14281 2023-07-19 06:34:24.000000 pygod-1.0.0/pygod.egg-info/PKG-INFO
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1092 2023-07-19 06:34:24.000000 pygod-1.0.0/pygod.egg-info/SOURCES.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)        1 2023-07-19 06:34:24.000000 pygod-1.0.0/pygod.egg-info/dependency_links.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)       45 2023-07-19 06:34:24.000000 pygod-1.0.0/pygod.egg-info/requires.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)        6 2023-07-19 06:34:24.000000 pygod-1.0.0/pygod.egg-info/top_level.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)       44 2023-07-19 06:34:03.000000 pygod-1.0.0/requirements.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)       80 2023-07-19 06:34:24.728273 pygod-1.0.0/setup.cfg
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2018 2023-07-19 06:34:03.000000 pygod-1.0.0/setup.py
```

### Comparing `pygod-0.4.0/LICENSE` & `pygod-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/PKG-INFO` & `pygod-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pygod
-Version: 0.4.0
+Version: 1.0.0
 Summary: A Python Library for Graph Outlier Detection (Anomaly Detection)
 Home-page: https://github.com/pygod-team/pygod/
 Download-URL: https://github.com/pygod-team/pygod/archive/main.zip
 Author: PyGOD Team
 Author-email: dev@pygod.org
 License: BSD-2
 Keywords: outlier detection,anomaly detection,graph mining,data mining,neural networks,graph neural networks
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/pygod-team/pygod/main/docs/pygod_logo.png
    :width: 1050
    :alt: PyGOD Logo
@@ -125,20 +126,20 @@
 
 ----
 
 Installation
 ^^^^^^^^^^^^
 
 **Note on PyG and PyTorch Installation**\ :
-PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ and `PyTorch <https://pytorch.org/>`_.
+PyGOD depends on `torch <https://https://pytorch.org/get-started/locally/>`_ and `torch_geometric (including its optional dependencies) <https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#>`_.
 To streamline the installation, PyGOD does **NOT** install these libraries for you.
 Please install them from the above links for running PyGOD:
 
 * torch>=2.0.0
-* pytorch_geometric>=2.3.0
+* torch_geometric>=2.3.0
 
 It is recommended to use **pip** for installation.
 Please make sure **the latest version** is installed, as PyGOD is updated frequently:
 
 .. code-block:: bash
 
    pip install pygod            # normal install
@@ -150,42 +151,39 @@
 
    git clone https://github.com/pygod-team/pygod.git
    cd pygod
    pip install .
 
 **Required Dependencies**\ :
 
-* Python 3.8+
+* python>=3.8
 * numpy>=1.24.3
 * scikit-learn>=1.2.2
 * scipy>=1.10.1
 * networkx>=3.1
 
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Full API Reference: (https://docs.pygod.org). API cheatsheet for all detectors:
 
-* **fit(data)**\ : Fit detector.
-* **decision_function(data)**\ : Predict raw anomaly score of PyG data using the fitted detector.
+* **fit(data)**\ : Fit the detector with train data.
+* **predict(data)**\ : Predict on test data (train data if not provided) using the fitted detector.
 
 Key Attributes of a fitted detector:
 
 * **decision_score_**\ : The outlier scores of the input data. Outliers tend to have higher scores.
 * **label_**\ : The binary labels of the input data. 0 stands for inliers and 1 for outliers.
+* **threshold_**\ : The determined threshold for binary classification. Scores above the threshold are outliers.
 
-For the inductive setting:
-
-* **predict(data)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
-
-**Input of PyGOD**: Please pass in a `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ data object.
+**Input of PyGOD**: Please pass in a `PyG Data object <https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.data.Data.html#torch_geometric.data.Data>`_.
 See `PyG data processing examples <https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html#data-handling-of-graphs>`_.
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
 ==================  =====  ===========  ===========  ========================================
@@ -197,15 +195,15 @@
 ANOMALOUS           2018   MF           No           [#Peng2018Anomalous]_
 ONE                 2019   MF           No           [#Bandyopadhyay2019Outlier]_
 DOMINANT            2019   GNN+AE       Yes          [#Ding2019Deep]_
 DONE                2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
 AdONE               2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
 AnomalyDAE          2020   GNN+AE       Yes          [#Fan2020AnomalyDAE]_
 GAAN                2020   GAN          Yes          [#Chen2020Generative]_
-OCGNN               2021   GNN+AE       Yes          [#Wang2021One]_
+OCGNN               2021   GNN          Yes          [#Wang2021One]_
 CoLA                2021   GNN+AE+SSL   Yes          [#Liu2021Anomaly]_
 GUIDE               2021   GNN+AE       Yes          [#Yuan2021Higher]_
 CONAD               2022   GNN+AE+SSL   Yes          [#Xu2022Contrastive]_
 ==================  =====  ===========  ===========  ========================================
 
 
 ----
```

### Comparing `pygod-0.4.0/README.rst` & `pygod-1.0.0/pygod.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: pygod
+Version: 1.0.0
+Summary: A Python Library for Graph Outlier Detection (Anomaly Detection)
+Home-page: https://github.com/pygod-team/pygod/
+Download-URL: https://github.com/pygod-team/pygod/archive/main.zip
+Author: PyGOD Team
+Author-email: dev@pygod.org
+License: BSD-2
+Keywords: outlier detection,anomaly detection,graph mining,data mining,neural networks,graph neural networks
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/pygod-team/pygod/main/docs/pygod_logo.png
    :width: 1050
    :alt: PyGOD Logo
    :align: center
 
 .. image:: https://img.shields.io/pypi/v/pygod.svg?color=brightgreen
    :target: https://pypi.org/project/pygod/
@@ -101,20 +126,20 @@
 
 ----
 
 Installation
 ^^^^^^^^^^^^
 
 **Note on PyG and PyTorch Installation**\ :
-PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ and `PyTorch <https://pytorch.org/>`_.
+PyGOD depends on `torch <https://https://pytorch.org/get-started/locally/>`_ and `torch_geometric (including its optional dependencies) <https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#>`_.
 To streamline the installation, PyGOD does **NOT** install these libraries for you.
 Please install them from the above links for running PyGOD:
 
 * torch>=2.0.0
-* pytorch_geometric>=2.3.0
+* torch_geometric>=2.3.0
 
 It is recommended to use **pip** for installation.
 Please make sure **the latest version** is installed, as PyGOD is updated frequently:
 
 .. code-block:: bash
 
    pip install pygod            # normal install
@@ -126,42 +151,39 @@
 
    git clone https://github.com/pygod-team/pygod.git
    cd pygod
    pip install .
 
 **Required Dependencies**\ :
 
-* Python 3.8+
+* python>=3.8
 * numpy>=1.24.3
 * scikit-learn>=1.2.2
 * scipy>=1.10.1
 * networkx>=3.1
 
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Full API Reference: (https://docs.pygod.org). API cheatsheet for all detectors:
 
-* **fit(data)**\ : Fit detector.
-* **decision_function(data)**\ : Predict raw anomaly score of PyG data using the fitted detector.
+* **fit(data)**\ : Fit the detector with train data.
+* **predict(data)**\ : Predict on test data (train data if not provided) using the fitted detector.
 
 Key Attributes of a fitted detector:
 
 * **decision_score_**\ : The outlier scores of the input data. Outliers tend to have higher scores.
 * **label_**\ : The binary labels of the input data. 0 stands for inliers and 1 for outliers.
+* **threshold_**\ : The determined threshold for binary classification. Scores above the threshold are outliers.
 
-For the inductive setting:
-
-* **predict(data)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
-
-**Input of PyGOD**: Please pass in a `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ data object.
+**Input of PyGOD**: Please pass in a `PyG Data object <https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.data.Data.html#torch_geometric.data.Data>`_.
 See `PyG data processing examples <https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html#data-handling-of-graphs>`_.
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
 ==================  =====  ===========  ===========  ========================================
@@ -173,15 +195,15 @@
 ANOMALOUS           2018   MF           No           [#Peng2018Anomalous]_
 ONE                 2019   MF           No           [#Bandyopadhyay2019Outlier]_
 DOMINANT            2019   GNN+AE       Yes          [#Ding2019Deep]_
 DONE                2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
 AdONE               2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
 AnomalyDAE          2020   GNN+AE       Yes          [#Fan2020AnomalyDAE]_
 GAAN                2020   GAN          Yes          [#Chen2020Generative]_
-OCGNN               2021   GNN+AE       Yes          [#Wang2021One]_
+OCGNN               2021   GNN          Yes          [#Wang2021One]_
 CoLA                2021   GNN+AE+SSL   Yes          [#Liu2021Anomaly]_
 GUIDE               2021   GNN+AE       Yes          [#Yuan2021Higher]_
 CONAD               2022   GNN+AE+SSL   Yes          [#Xu2022Contrastive]_
 ==================  =====  ===========  ===========  ========================================
 
 
 ----
```

### Comparing `pygod-0.4.0/pygod/detector/__init__.py` & `pygod-1.0.0/pygod/detector/__init__.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/adone.py` & `pygod-1.0.0/pygod/detector/adone.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/anomalous.py` & `pygod-1.0.0/pygod/detector/anomalous.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/anomalydae.py` & `pygod-1.0.0/pygod/detector/anomalydae.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/base.py` & `pygod-1.0.0/pygod/detector/base.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/cola.py` & `pygod-1.0.0/pygod/detector/cola.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/conad.py` & `pygod-1.0.0/pygod/detector/conad.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/dominant.py` & `pygod-1.0.0/pygod/detector/dominant.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/done.py` & `pygod-1.0.0/pygod/detector/done.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/gaan.py` & `pygod-1.0.0/pygod/detector/gaan.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/gae.py` & `pygod-1.0.0/pygod/detector/gae.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/guide.py` & `pygod-1.0.0/pygod/detector/guide.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/ocgnn.py` & `pygod-1.0.0/pygod/detector/ocgnn.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/one.py` & `pygod-1.0.0/pygod/detector/one.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/radar.py` & `pygod-1.0.0/pygod/detector/radar.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/detector/scan.py` & `pygod-1.0.0/pygod/detector/scan.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/generator/outlier_generator.py` & `pygod-1.0.0/pygod/generator/outlier_generator.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/metric/metric.py` & `pygod-1.0.0/pygod/metric/metric.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/adone.py` & `pygod-1.0.0/pygod/nn/adone.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/anomalydae.py` & `pygod-1.0.0/pygod/nn/anomalydae.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/cola.py` & `pygod-1.0.0/pygod/nn/cola.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/conv.py` & `pygod-1.0.0/pygod/nn/conv.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/decoder.py` & `pygod-1.0.0/pygod/nn/decoder.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/dominant.py` & `pygod-1.0.0/pygod/nn/dominant.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/done.py` & `pygod-1.0.0/pygod/nn/done.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/encoder.py` & `pygod-1.0.0/pygod/nn/encoder.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/functional.py` & `pygod-1.0.0/pygod/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/gaan.py` & `pygod-1.0.0/pygod/nn/gaan.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/gae.py` & `pygod-1.0.0/pygod/nn/gae.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/guide.py` & `pygod-1.0.0/pygod/nn/guide.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/nn/ocgnn.py` & `pygod-1.0.0/pygod/nn/ocgnn.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/utils/score_converter.py` & `pygod-1.0.0/pygod/utils/score_converter.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/utils/utility.py` & `pygod-1.0.0/pygod/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/pygod/version.py` & `pygod-1.0.0/pygod/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 
-__version__ = '0.4.0'
+__version__ = '1.0.0'
```

### Comparing `pygod-0.4.0/pygod.egg-info/PKG-INFO` & `pygod-1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pygod
-Version: 0.4.0
-Summary: A Python Library for Graph Outlier Detection (Anomaly Detection)
-Home-page: https://github.com/pygod-team/pygod/
-Download-URL: https://github.com/pygod-team/pygod/archive/main.zip
-Author: PyGOD Team
-Author-email: dev@pygod.org
-License: BSD-2
-Keywords: outlier detection,anomaly detection,graph mining,data mining,neural networks,graph neural networks
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/pygod-team/pygod/main/docs/pygod_logo.png
    :width: 1050
    :alt: PyGOD Logo
    :align: center
 
 .. image:: https://img.shields.io/pypi/v/pygod.svg?color=brightgreen
    :target: https://pypi.org/project/pygod/
@@ -125,20 +101,20 @@
 
 ----
 
 Installation
 ^^^^^^^^^^^^
 
 **Note on PyG and PyTorch Installation**\ :
-PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ and `PyTorch <https://pytorch.org/>`_.
+PyGOD depends on `torch <https://https://pytorch.org/get-started/locally/>`_ and `torch_geometric (including its optional dependencies) <https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#>`_.
 To streamline the installation, PyGOD does **NOT** install these libraries for you.
 Please install them from the above links for running PyGOD:
 
 * torch>=2.0.0
-* pytorch_geometric>=2.3.0
+* torch_geometric>=2.3.0
 
 It is recommended to use **pip** for installation.
 Please make sure **the latest version** is installed, as PyGOD is updated frequently:
 
 .. code-block:: bash
 
    pip install pygod            # normal install
@@ -150,42 +126,39 @@
 
    git clone https://github.com/pygod-team/pygod.git
    cd pygod
    pip install .
 
 **Required Dependencies**\ :
 
-* Python 3.8+
+* python>=3.8
 * numpy>=1.24.3
 * scikit-learn>=1.2.2
 * scipy>=1.10.1
 * networkx>=3.1
 
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Full API Reference: (https://docs.pygod.org). API cheatsheet for all detectors:
 
-* **fit(data)**\ : Fit detector.
-* **decision_function(data)**\ : Predict raw anomaly score of PyG data using the fitted detector.
+* **fit(data)**\ : Fit the detector with train data.
+* **predict(data)**\ : Predict on test data (train data if not provided) using the fitted detector.
 
 Key Attributes of a fitted detector:
 
 * **decision_score_**\ : The outlier scores of the input data. Outliers tend to have higher scores.
 * **label_**\ : The binary labels of the input data. 0 stands for inliers and 1 for outliers.
+* **threshold_**\ : The determined threshold for binary classification. Scores above the threshold are outliers.
 
-For the inductive setting:
-
-* **predict(data)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
-
-**Input of PyGOD**: Please pass in a `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ data object.
+**Input of PyGOD**: Please pass in a `PyG Data object <https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.data.Data.html#torch_geometric.data.Data>`_.
 See `PyG data processing examples <https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html#data-handling-of-graphs>`_.
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
 ==================  =====  ===========  ===========  ========================================
@@ -197,15 +170,15 @@
 ANOMALOUS           2018   MF           No           [#Peng2018Anomalous]_
 ONE                 2019   MF           No           [#Bandyopadhyay2019Outlier]_
 DOMINANT            2019   GNN+AE       Yes          [#Ding2019Deep]_
 DONE                2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
 AdONE               2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
 AnomalyDAE          2020   GNN+AE       Yes          [#Fan2020AnomalyDAE]_
 GAAN                2020   GAN          Yes          [#Chen2020Generative]_
-OCGNN               2021   GNN+AE       Yes          [#Wang2021One]_
+OCGNN               2021   GNN          Yes          [#Wang2021One]_
 CoLA                2021   GNN+AE+SSL   Yes          [#Liu2021Anomaly]_
 GUIDE               2021   GNN+AE       Yes          [#Yuan2021Higher]_
 CONAD               2022   GNN+AE+SSL   Yes          [#Xu2022Contrastive]_
 ==================  =====  ===========  ===========  ========================================
 
 
 ----
```

### Comparing `pygod-0.4.0/pygod.egg-info/SOURCES.txt` & `pygod-1.0.0/pygod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygod-0.4.0/setup.py` & `pygod-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,20 +36,21 @@
                 'data mining', 'neural networks', 'graph neural networks'],
       packages=find_packages(exclude=['test']),
       include_package_data=True,
       install_requires=requirements,
       setup_requires=['setuptools>=38.6.0'],
       license='BSD-2',
       classifiers=[
-          'Development Status :: 2 - Pre-Alpha',
+          'Development Status :: 3 - Alpha',
           'Intended Audience :: Education',
           'Intended Audience :: Financial and Insurance Industry',
           'Intended Audience :: Science/Research',
           'Intended Audience :: Developers',
           'Intended Audience :: Information Technology',
           'License :: OSI Approved :: BSD License',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'License :: OSI Approved :: BSD License'
       ],
 )
```

