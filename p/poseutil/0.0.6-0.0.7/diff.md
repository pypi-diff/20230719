# Comparing `tmp/poseutil-0.0.6.tar.gz` & `tmp/poseutil-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.0.6.tar", last modified: Wed Jul 19 03:34:13 2023, max compression
+gzip compressed data, was "poseutil-0.0.7.tar", last modified: Wed Jul 19 03:36:51 2023, max compression
```

## Comparing `poseutil-0.0.6.tar` & `poseutil-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:34:13.286579 poseutil-0.0.6/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:34:13.286418 poseutil-0.0.6/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:34:13.283872 poseutil-0.0.6/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:34:13.000000 poseutil-0.0.6/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      436 2023-07-19 03:34:13.000000 poseutil-0.0.6/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:34:13.000000 poseutil-0.0.6/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:30:18.000000 poseutil-0.0.6/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 03:34:13.000000 poseutil-0.0.6/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 03:34:13.286626 poseutil-0.0.6/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 03:34:11.000000 poseutil-0.0.6/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:34:13.286205 poseutil-0.0.6/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.6/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8055 2023-07-19 03:32:22.000000 poseutil-0.0.6/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.6/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1067 2023-07-19 03:27:56.000000 poseutil-0.0.6/utils/csvHelper copy.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.6/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.6/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.6/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15114 2023-07-19 03:34:00.000000 poseutil-0.0.6/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.6/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.6/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-07-19 02:18:56.000000 poseutil-0.0.6/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.6/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.6/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:36:51.411017 poseutil-0.0.7/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:36:51.410876 poseutil-0.0.7/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:36:51.409260 poseutil-0.0.7/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 03:36:51.411058 poseutil-0.0.7/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 03:36:48.000000 poseutil-0.0.7/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:36:51.410708 poseutil-0.0.7/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.7/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8057 2023-07-19 03:35:52.000000 poseutil-0.0.7/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.7/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.7/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15122 2023-07-19 03:36:15.000000 poseutil-0.0.7/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.7/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-07-19 02:18:56.000000 poseutil-0.0.7/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.7/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/version.py
```

### Comparing `poseutil-0.0.6/setup.py` & `poseutil-0.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.0.6',
+    version='0.0.7',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.0.6/utils/ReadFrameData.py` & `poseutil-0.0.7/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/common_component.py` & `poseutil-0.0.7/utils/common_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import shutil
 import time
 import glob
 import gzip, pickle
-from utils.const import *
 import numpy as np
 import cv2
 import re, json
 import tensorflow as tf
+import struct, itertools
+import matplotlib.pyplot as plt
+
+from utils.const import *
 from utils.poseMeasure import PoseMeasure
 from utils.normarlize import getPoseEmbeddingList
 from utils.version import VersionCaster
-import struct, itertools
-import matplotlib.pyplot as plt
+
 
 def get_dance_audio_list():
     audio_list_path = DANCE_AUDIO_PATH
     sorted_list = sorted(os.listdir(audio_list_path))
     if 'common' in sorted_list:
         sorted_list.remove('common')
     return sorted(sorted_list)
```

### Comparing `poseutil-0.0.6/utils/const.py` & `poseutil-0.0.7/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/csvHelper copy.py` & `poseutil-0.0.7/utils/csvHelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import csv
-from pose_util import Coordinate
+from utils.pose_util import Coordinate
 
 
 def readCSV(filename, preifx =1):
     resultList = []
     with open(filename, "r", encoding="utf-8") as f:
         reader = csv.reader(f)
         for line in reader:
```

### Comparing `poseutil-0.0.6/utils/cv_util.py` & `poseutil-0.0.7/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/math_util.py` & `poseutil-0.0.7/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/normarlize.py` & `poseutil-0.0.7/utils/normarlize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import math
+import pickle, gzip
+
 from utils.pose_util import *
 from utils.const import *
 import utils.csvHelper as csvHelper
-from normarlize import getPoseEmbedding, roundRow
-import pickle, gzip
+from utils.normarlize import getPoseEmbedding, roundRow
 from utils.const import *
+
 STEP_1 = 'up'
 STEP_2 = 'down'
 
 LEFT = "LEFT"
 RIGHT = "RIGHT"
```

### Comparing `poseutil-0.0.6/utils/poseMeasure.py` & `poseutil-0.0.7/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/poseMeasureFormat.py` & `poseutil-0.0.7/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/pose_util.py` & `poseutil-0.0.7/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/qt_component.py` & `poseutil-0.0.7/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.6/utils/version.py` & `poseutil-0.0.7/utils/version.py`

 * *Files identical despite different names*

