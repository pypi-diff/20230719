# Comparing `tmp/annieslasso-0.2.93.tar.gz` & `tmp/annieslasso-0.2.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/annieslasso-0.2.93.tar", last modified: Wed Nov  9 05:08:04 2022, max compression
+gzip compressed data, was "dist/annieslasso-0.2.94.tar", last modified: Tue Jul 18 23:48:15 2023, max compression
```

## Comparing `annieslasso-0.2.93.tar` & `annieslasso-0.2.94.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-09 05:08:04.000000 annieslasso-0.2.93/
--rw-r--r--   0 nidever    (503) staff       (20)     1079 2022-11-09 05:05:07.000000 annieslasso-0.2.93/LICENSE
--rw-r--r--   0 nidever    (503) staff       (20)       34 2022-11-09 05:05:07.000000 annieslasso-0.2.93/MANIFEST.in
--rw-r--r--   0 nidever    (503) staff       (20)      699 2022-11-09 05:08:04.000000 annieslasso-0.2.93/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)     2838 2022-11-09 05:05:07.000000 annieslasso-0.2.93/README.md
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-09 05:08:04.000000 annieslasso-0.2.93/annieslasso.egg-info/
--rw-r--r--   0 nidever    (503) staff       (20)      699 2022-11-09 05:08:03.000000 annieslasso-0.2.93/annieslasso.egg-info/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      596 2022-11-09 05:08:04.000000 annieslasso-0.2.93/annieslasso.egg-info/SOURCES.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2022-11-09 05:08:03.000000 annieslasso-0.2.93/annieslasso.egg-info/dependency_links.txt
--rw-r--r--   0 nidever    (503) staff       (20)       47 2022-11-09 05:08:04.000000 annieslasso-0.2.93/annieslasso.egg-info/entry_points.txt
--rw-r--r--   0 nidever    (503) staff       (20)       33 2022-11-09 05:08:04.000000 annieslasso-0.2.93/annieslasso.egg-info/requires.txt
--rw-r--r--   0 nidever    (503) staff       (20)       10 2022-11-09 05:08:04.000000 annieslasso-0.2.93/annieslasso.egg-info/top_level.txt
--rw-r--r--   0 nidever    (503) staff       (20)       38 2022-11-09 05:08:04.000000 annieslasso-0.2.93/setup.cfg
--rw-r--r--   0 nidever    (503) staff       (20)     1789 2022-11-09 05:08:02.000000 annieslasso-0.2.93/setup.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-09 05:08:04.000000 annieslasso-0.2.93/thecannon/
--rw-r--r--   0 nidever    (503) staff       (20)     1059 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/__init__.py
--rw-r--r--   0 nidever    (503) staff       (20)    10721 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/__main__.py
--rw-r--r--   0 nidever    (503) staff       (20)     5468 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/censoring.py
--rw-r--r--   0 nidever    (503) staff       (20)     8926 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/continuum.py
--rw-r--r--   0 nidever    (503) staff       (20)    17407 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/fitting.py
--rw-r--r--   0 nidever    (503) staff       (20)    27135 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/model.py
--rw-r--r--   0 nidever    (503) staff       (20)     9615 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/plot.py
--rw-r--r--   0 nidever    (503) staff       (20)     5616 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/restricted.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-09 05:08:04.000000 annieslasso-0.2.93/thecannon/tests/
--rw-r--r--   0 nidever    (503) staff       (20)        0 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/tests/__init__.py
--rw-r--r--   0 nidever    (503) staff       (20)      499 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/tests/test_utils.py
--rw-r--r--   0 nidever    (503) staff       (20)     5379 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/utils.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-09 05:08:04.000000 annieslasso-0.2.93/thecannon/vectorizer/
--rw-r--r--   0 nidever    (503) staff       (20)       97 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/vectorizer/__init__.py
--rw-r--r--   0 nidever    (503) staff       (20)     2912 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/vectorizer/base.py
--rw-r--r--   0 nidever    (503) staff       (20)    13846 2022-11-09 05:05:07.000000 annieslasso-0.2.93/thecannon/vectorizer/polynomial.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-07-18 23:48:15.000000 annieslasso-0.2.94/
+-rw-r--r--   0 nidever    (503) staff       (20)     1079 2022-11-09 05:05:07.000000 annieslasso-0.2.94/LICENSE
+-rw-r--r--   0 nidever    (503) staff       (20)       34 2022-11-09 05:05:07.000000 annieslasso-0.2.94/MANIFEST.in
+-rw-r--r--   0 nidever    (503) staff       (20)      671 2023-07-18 23:48:15.000000 annieslasso-0.2.94/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)     2838 2022-11-09 05:05:07.000000 annieslasso-0.2.94/README.md
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/
+-rw-r--r--   0 nidever    (503) staff       (20)      671 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)      596 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/SOURCES.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/dependency_links.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       47 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/entry_points.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       33 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/requires.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       10 2023-07-18 23:48:15.000000 annieslasso-0.2.94/annieslasso.egg-info/top_level.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       38 2023-07-18 23:48:15.000000 annieslasso-0.2.94/setup.cfg
+-rw-r--r--   0 nidever    (503) staff       (20)     1789 2023-07-18 23:48:14.000000 annieslasso-0.2.94/setup.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-07-18 23:48:15.000000 annieslasso-0.2.94/thecannon/
+-rw-r--r--   0 nidever    (503) staff       (20)     1059 2023-07-18 23:47:57.000000 annieslasso-0.2.94/thecannon/__init__.py
+-rw-r--r--   0 nidever    (503) staff       (20)    10721 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/__main__.py
+-rw-r--r--   0 nidever    (503) staff       (20)     5468 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/censoring.py
+-rw-r--r--   0 nidever    (503) staff       (20)     8926 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/continuum.py
+-rw-r--r--   0 nidever    (503) staff       (20)    17407 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/fitting.py
+-rw-r--r--   0 nidever    (503) staff       (20)    27135 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/model.py
+-rw-r--r--   0 nidever    (503) staff       (20)     9615 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/plot.py
+-rw-r--r--   0 nidever    (503) staff       (20)     5616 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/restricted.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-07-18 23:48:15.000000 annieslasso-0.2.94/thecannon/tests/
+-rw-r--r--   0 nidever    (503) staff       (20)        0 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/tests/__init__.py
+-rw-r--r--   0 nidever    (503) staff       (20)      499 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/tests/test_utils.py
+-rw-r--r--   0 nidever    (503) staff       (20)     5437 2023-07-18 23:32:08.000000 annieslasso-0.2.94/thecannon/utils.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-07-18 23:48:15.000000 annieslasso-0.2.94/thecannon/vectorizer/
+-rw-r--r--   0 nidever    (503) staff       (20)       97 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/vectorizer/__init__.py
+-rw-r--r--   0 nidever    (503) staff       (20)     2912 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/vectorizer/base.py
+-rw-r--r--   0 nidever    (503) staff       (20)    13846 2022-11-09 05:05:07.000000 annieslasso-0.2.94/thecannon/vectorizer/polynomial.py
```

### Comparing `annieslasso-0.2.93/LICENSE` & `annieslasso-0.2.94/LICENSE`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/PKG-INFO` & `annieslasso-0.2.94/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: annieslasso
-Version: 0.2.93
+Version: 0.2.94
 Summary: A data-driven approach to stellar spectroscopy
 Home-page: http://thecannon.io
 Author: Andrew R. Casey, David W. Hogg, Melissa Ness
 Author-email: andrew.casey@monash.edu
 License: MIT
 Keywords: The Cannon
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: test
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `annieslasso-0.2.93/README.md` & `annieslasso-0.2.94/README.md`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/annieslasso.egg-info/PKG-INFO` & `annieslasso-0.2.94/annieslasso.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: annieslasso
-Version: 0.2.93
+Version: 0.2.94
 Summary: A data-driven approach to stellar spectroscopy
 Home-page: http://thecannon.io
 Author: Andrew R. Casey, David W. Hogg, Melissa Ness
 Author-email: andrew.casey@monash.edu
 License: MIT
 Keywords: The Cannon
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: test
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `annieslasso-0.2.93/annieslasso.egg-info/SOURCES.txt` & `annieslasso-0.2.94/annieslasso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/setup.py` & `annieslasso-0.2.94/setup.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/__init__.py` & `annieslasso-0.2.94/thecannon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = "0.2.93"
+__version__ = "0.2.94"
 
 import logging
 from numpy import RankWarning
 from warnings import simplefilter
 
 from .model import CannonModel
 from . import (censoring, fitting, plot, utils, vectorizer)
```

### Comparing `annieslasso-0.2.93/thecannon/__main__.py` & `annieslasso-0.2.94/thecannon/__main__.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/censoring.py` & `annieslasso-0.2.94/thecannon/censoring.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/continuum.py` & `annieslasso-0.2.94/thecannon/continuum.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/fitting.py` & `annieslasso-0.2.94/thecannon/fitting.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/model.py` & `annieslasso-0.2.94/thecannon/model.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/plot.py` & `annieslasso-0.2.94/thecannon/plot.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/restricted.py` & `annieslasso-0.2.94/thecannon/restricted.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/utils.py` & `annieslasso-0.2.94/thecannon/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import os
 import pickle
 import signal
 import sys
 from six import string_types
 from tempfile import mkstemp
 from time import time
-from collections import Iterable
+try:
+    from collections import Iterable
+except:
+    from collections.abc import Iterable
 from hashlib import md5
 from multiprocessing.pool import Pool
 from multiprocessing import Lock, TimeoutError, Value
 
 logger = logging.getLogger(__name__)
```

### Comparing `annieslasso-0.2.93/thecannon/vectorizer/base.py` & `annieslasso-0.2.94/thecannon/vectorizer/base.py`

 * *Files identical despite different names*

### Comparing `annieslasso-0.2.93/thecannon/vectorizer/polynomial.py` & `annieslasso-0.2.94/thecannon/vectorizer/polynomial.py`

 * *Files identical despite different names*

