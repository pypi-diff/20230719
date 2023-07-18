# Comparing `tmp/fitsviz-0.0.2.tar.gz` & `tmp/fitsviz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsviz-0.0.2.tar", last modified: Tue Jul 18 21:55:15 2023, max compression
+gzip compressed data, was "fitsviz-0.0.3.tar", last modified: Tue Jul 18 22:30:13 2023, max compression
```

## Comparing `fitsviz-0.0.2.tar` & `fitsviz-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.998581 fitsviz-0.0.2/
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 21:55:15.998581 fitsviz-0.0.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1888 2023-07-18 21:54:05.000000 fitsviz-0.0.2/README.md
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.996581 fitsviz-0.0.2/fitsviz/
--rw-r--r--   0 user      (1000) user      (1000)      203 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2829 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/__main__.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.997581 fitsviz-0.0.2/fitsviz/detection/
--rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/detection/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     8062 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/detection/ap_photometry.py
--rw-r--r--   0 user      (1000) user      (1000)     1485 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/detection/core.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.997581 fitsviz-0.0.2/fitsviz/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/tests/test_loading.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/tests/test_viz.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.998581 fitsviz-0.0.2/fitsviz/utils/
--rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/utils/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2392 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/utils/cutils.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.998581 fitsviz-0.0.2/fitsviz/viz/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/viz/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2315 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/viz/plot_bokeh.py
--rw-r--r--   0 user      (1000) user      (1000)     1226 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/viz/plot_matplotlib.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.997581 fitsviz-0.0.2/fitsviz.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      522 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      153 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      585 2023-07-18 21:54:05.000000 fitsviz-0.0.2/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-18 21:55:15.998581 fitsviz-0.0.2/setup.cfg
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.443905 fitsviz-0.0.3/
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 22:30:13.443905 fitsviz-0.0.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1888 2023-07-18 22:29:52.000000 fitsviz-0.0.3/README.md
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.441905 fitsviz-0.0.3/fitsviz/
+-rw-r--r--   0 user      (1000) user      (1000)      203 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2829 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/__main__.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.442905 fitsviz-0.0.3/fitsviz/detection/
+-rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/detection/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     8040 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/detection/ap_photometry.py
+-rw-r--r--   0 user      (1000) user      (1000)     1485 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/detection/core.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.442905 fitsviz-0.0.3/fitsviz/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/tests/test_loading.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/tests/test_viz.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.442905 fitsviz-0.0.3/fitsviz/utils/
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/utils/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2392 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/utils/cutils.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.443905 fitsviz-0.0.3/fitsviz/viz/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/viz/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2315 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/viz/plot_bokeh.py
+-rw-r--r--   0 user      (1000) user      (1000)     1226 2023-07-18 22:29:52.000000 fitsviz-0.0.3/fitsviz/viz/plot_matplotlib.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:30:13.441905 fitsviz-0.0.3/fitsviz.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 22:30:13.000000 fitsviz-0.0.3/fitsviz.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      522 2023-07-18 22:30:13.000000 fitsviz-0.0.3/fitsviz.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-18 22:30:13.000000 fitsviz-0.0.3/fitsviz.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      139 2023-07-18 22:30:13.000000 fitsviz-0.0.3/fitsviz.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-07-18 22:30:13.000000 fitsviz-0.0.3/fitsviz.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      564 2023-07-18 22:29:52.000000 fitsviz-0.0.3/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-18 22:30:13.443905 fitsviz-0.0.3/setup.cfg
```

### Comparing `fitsviz-0.0.2/PKG-INFO` & `fitsviz-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsviz
-Version: 0.0.2
+Version: 0.0.3
 Summary: Autodetection of sources and visualization of FITS files
 Author-email: Phani Velicheti <phaniv@arizona.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 
 # fitsviz
```

### Comparing `fitsviz-0.0.2/README.md` & `fitsviz-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/fitsviz/__main__.py` & `fitsviz-0.0.3/fitsviz/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/fitsviz/detection/ap_photometry.py` & `fitsviz-0.0.3/fitsviz/detection/ap_photometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import dask
 from astropy.io import fits
 from photutils.detection import DAOStarFinder
 from astropy.stats import sigma_clipped_stats
 from fitsviz.detection.core import DetectionBase
 import pandas as pd
 import numpy as np
-from numba import jit
 import concurrent.futures
 import dask.dataframe as dd
 from dask.distributed import Client
 import multiprocessing
 
 
 class ApertureDAO(DetectionBase):
```

### Comparing `fitsviz-0.0.2/fitsviz/detection/core.py` & `fitsviz-0.0.3/fitsviz/detection/core.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/fitsviz/utils/cutils.py` & `fitsviz-0.0.3/fitsviz/utils/cutils.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/fitsviz/viz/plot_bokeh.py` & `fitsviz-0.0.3/fitsviz/viz/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/fitsviz/viz/plot_matplotlib.py` & `fitsviz-0.0.3/fitsviz/viz/plot_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/fitsviz.egg-info/PKG-INFO` & `fitsviz-0.0.3/fitsviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsviz
-Version: 0.0.2
+Version: 0.0.3
 Summary: Autodetection of sources and visualization of FITS files
 Author-email: Phani Velicheti <phaniv@arizona.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 
 # fitsviz
```

### Comparing `fitsviz-0.0.2/fitsviz.egg-info/SOURCES.txt` & `fitsviz-0.0.3/fitsviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.2/pyproject.toml` & `fitsviz-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ['setuptools>=68.0.0']
 
 [project]
 
 name = "fitsviz"
-version = "0.0.2"
+version = "0.0.3"
 description = "Autodetection of sources and visualization of FITS files"
 
 authors = [
     {name="Phani Velicheti",email = "phaniv@arizona.edu"}
 ]
 
 readme = "README.md"
@@ -18,15 +18,14 @@
 dependencies = [
     'poetry-core>=1.1.0',
     'astropy==5.3.1',
     'bokeh==3.2.0',
     'click==8.0.4',
     'dask==2021.10.0',
     'matplotlib==3.4.3',
-    'numba==0.54.1',
     'numpy==1.22.3',
     'pandas==2.0.3',
     'photutils==1.8.0',
 ]
```

