# Comparing `tmp/poseutil-0.0.3.tar.gz` & `tmp/poseutil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.0.3.tar", last modified: Wed Jul 19 02:09:53 2023, max compression
+gzip compressed data, was "poseutil-0.0.4.tar", last modified: Wed Jul 19 03:30:18 2023, max compression
```

## Comparing `poseutil-0.0.3.tar` & `poseutil-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 02:09:53.862319 poseutil-0.0.3/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 02:09:53.862144 poseutil-0.0.3/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 02:09:53.858178 poseutil-0.0.3/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.3/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 02:09:53.862366 poseutil-0.0.3/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 02:09:44.000000 poseutil-0.0.3/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 02:09:53.861824 poseutil-0.0.3/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.3/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8049 2023-07-19 02:08:21.000000 poseutil-0.0.3/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.3/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.3/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    12688 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.3/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     3512 2023-07-19 01:20:40.000000 poseutil-0.0.3/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.3/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:30:18.640548 poseutil-0.0.4/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:30:18.640355 poseutil-0.0.4/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:30:18.636003 poseutil-0.0.4/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:30:18.000000 poseutil-0.0.4/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      436 2023-07-19 03:30:18.000000 poseutil-0.0.4/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:30:18.000000 poseutil-0.0.4/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:30:18.000000 poseutil-0.0.4/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 03:30:18.000000 poseutil-0.0.4/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 03:30:18.640598 poseutil-0.0.4/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 03:30:18.000000 poseutil-0.0.4/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:30:18.639991 poseutil-0.0.4/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.4/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8049 2023-07-19 02:08:21.000000 poseutil-0.0.4/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.4/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1067 2023-07-19 03:27:56.000000 poseutil-0.0.4/utils/csvHelper copy.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.4/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.4/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.4/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15169 2023-07-19 03:28:44.000000 poseutil-0.0.4/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.4/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.4/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-07-19 02:18:56.000000 poseutil-0.0.4/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.4/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.4/utils/version.py
```

### Comparing `poseutil-0.0.3/setup.py` & `poseutil-0.0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.0.3',
+    version='0.0.4',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.0.3/utils/ReadFrameData.py` & `poseutil-0.0.4/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/common_component.py` & `poseutil-0.0.4/utils/common_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/const.py` & `poseutil-0.0.4/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/csvHelper.py` & `poseutil-0.0.4/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/cv_util.py` & `poseutil-0.0.4/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/math_util.py` & `poseutil-0.0.4/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/normarlize.py` & `poseutil-0.0.4/utils/normarlize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,81 @@
 import math
 from utils.pose_util import *
 from utils.const import *
+from lib2to3.pytree import convert
+import csvHelper
+from normarlize import getPoseEmbedding, roundRow
+import argparse
+import os, pickle, gzip
+import numpy as np
+from utils.const import *
+STEP_1 = 'up'
+STEP_2 = 'down'
+
+LEFT = "LEFT"
+RIGHT = "RIGHT"
+
+
+def preProcessing(filePath, exerciseType):
+    labeling = csvHelper.readCSV(filePath)
+    result = []
+    for row in labeling:
+        embedding = getPoseEmbedding(row[1:], exerciseType)
+        roundEmbedding = roundRow(embedding)
+        roundEmbedding.insert(0, row[0])
+        result.append(roundEmbedding)
+
+    convertPath = filePath.replace("_exerciseState", "").replace(".csv", "")
+    if "LEFT" in exerciseType:
+        convertPath += "L.csv"
+    elif "RIGHT" in exerciseType:
+        convertPath += "R.csv"
+    else:
+        convertPath += ".csv"
+    csvHelper.writeCSV(convertPath, result)
+
+def preProcessingNew(exercise, filePath, exerciseType, sideViserblity):
+    with gzip.open(filePath, "rb") as f:
+        pickle_data = pickle.load(f)
+    labels = pickle_data["knn_label"]
+    poses = pickle_data["pose"]
+    all = embeddingConvert(labels, poses, exerciseType)
+    if sideViserblity == LEFT:
+        left = embeddingConvert(labels, poses, exerciseType + LEFT)
+        right = embeddingConvert(labels, poses, exerciseType + RIGHT)
+        print(f'sideViserblity : {sideViserblity}, copy left')
+    elif sideViserblity == RIGHT:
+        left = embeddingConvert(labels, poses, exerciseType + LEFT)
+        right = embeddingConvert(labels, poses, exerciseType + RIGHT)
+        print(f'sideViserblity : {sideViserblity}, copy right')
+    else:
+        left = embeddingConvert(labels, poses, exerciseType + LEFT)
+        right = embeddingConvert(labels, poses, exerciseType + RIGHT)
+        print(f'sideViserblity : {sideViserblity}')
+
+    
+    savePath = f"{KNN_PATH}/{exercise}/{exerciseType}/{exercise}"
+    createFile(all, savePath, ".csv")
+    createFile(left, savePath, 'L.csv')
+    createFile(right, savePath, 'R.csv')
+    createFile(left+right, savePath, 'Side.csv')
+
+
+def embeddingConvert(labels, poses, exerciseType):
+    result = []
+    for label, pose in zip(labels, poses):
+        embedding = getPoseEmbedding(pose, exerciseType)
+        roundEmbedding = roundRow(embedding)
+        roundEmbedding.insert(0, label)
+        result.append(roundEmbedding)
+    return result
+
+def createFile(data, convertPath, exerciseTypeDetail):
+    convertPath += exerciseTypeDetail
+    csvHelper.writeCSV(convertPath, data)
 
 def roundRow(row):
     result = []
     for cell in row:
         result.append(Coordinate(round(cell.x, 3), round(cell.y, 3), round(cell.z, 3)))
     return result
```

### Comparing `poseutil-0.0.3/utils/poseMeasure.py` & `poseutil-0.0.4/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/poseMeasureFormat.py` & `poseutil-0.0.4/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/qt_component.py` & `poseutil-0.0.4/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.3/utils/version.py` & `poseutil-0.0.4/utils/version.py`

 * *Files identical despite different names*

