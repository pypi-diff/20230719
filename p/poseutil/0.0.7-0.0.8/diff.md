# Comparing `tmp/poseutil-0.0.7.tar.gz` & `tmp/poseutil-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.0.7.tar", last modified: Wed Jul 19 03:36:51 2023, max compression
+gzip compressed data, was "poseutil-0.0.8.tar", last modified: Wed Jul 19 03:41:05 2023, max compression
```

## Comparing `poseutil-0.0.7.tar` & `poseutil-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:36:51.411017 poseutil-0.0.7/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:36:51.410876 poseutil-0.0.7/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:36:51.409260 poseutil-0.0.7/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 03:36:51.000000 poseutil-0.0.7/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 03:36:51.411058 poseutil-0.0.7/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 03:36:48.000000 poseutil-0.0.7/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:36:51.410708 poseutil-0.0.7/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.7/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8057 2023-07-19 03:35:52.000000 poseutil-0.0.7/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.7/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.7/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15122 2023-07-19 03:36:15.000000 poseutil-0.0.7/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.7/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-07-19 02:18:56.000000 poseutil-0.0.7/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.7/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.7/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:41:05.882167 poseutil-0.0.8/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:41:05.882026 poseutil-0.0.8/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:41:05.880235 poseutil-0.0.8/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 03:41:05.000000 poseutil-0.0.8/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-07-19 03:41:05.000000 poseutil-0.0.8/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:41:05.000000 poseutil-0.0.8/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 03:41:05.000000 poseutil-0.0.8/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 03:41:05.000000 poseutil-0.0.8/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 03:41:05.882226 poseutil-0.0.8/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 03:40:56.000000 poseutil-0.0.8/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 03:41:05.881857 poseutil-0.0.8/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.8/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8057 2023-07-19 03:35:52.000000 poseutil-0.0.8/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.8/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.8/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.8/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.8/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15066 2023-07-19 03:40:40.000000 poseutil-0.0.8/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.8/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.8/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-07-19 02:18:56.000000 poseutil-0.0.8/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.8/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.8/utils/version.py
```

### Comparing `poseutil-0.0.7/setup.py` & `poseutil-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.0.7',
+    version='0.0.8',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.0.7/utils/ReadFrameData.py` & `poseutil-0.0.8/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/common_component.py` & `poseutil-0.0.8/utils/common_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/const.py` & `poseutil-0.0.8/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/csvHelper.py` & `poseutil-0.0.8/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/cv_util.py` & `poseutil-0.0.8/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/math_util.py` & `poseutil-0.0.8/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/normarlize.py` & `poseutil-0.0.8/utils/normarlize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import math
 import pickle, gzip
 
 from utils.pose_util import *
 from utils.const import *
 import utils.csvHelper as csvHelper
-from utils.normarlize import getPoseEmbedding, roundRow
 from utils.const import *
 
 STEP_1 = 'up'
 STEP_2 = 'down'
 
 LEFT = "LEFT"
 RIGHT = "RIGHT"
```

### Comparing `poseutil-0.0.7/utils/poseMeasure.py` & `poseutil-0.0.8/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/poseMeasureFormat.py` & `poseutil-0.0.8/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/pose_util.py` & `poseutil-0.0.8/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/qt_component.py` & `poseutil-0.0.8/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.7/utils/version.py` & `poseutil-0.0.8/utils/version.py`

 * *Files identical despite different names*

