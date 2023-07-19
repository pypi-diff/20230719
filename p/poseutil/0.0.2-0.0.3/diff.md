# Comparing `tmp/poseutil-0.0.2.tar.gz` & `tmp/poseutil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.0.2.tar", last modified: Wed Jul 19 01:49:49 2023, max compression
+gzip compressed data, was "poseutil-0.0.3.tar", last modified: Wed Jul 19 02:09:53 2023, max compression
```

## Comparing `poseutil-0.0.2.tar` & `poseutil-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:49:49.666290 poseutil-0.0.2/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 01:49:49.666144 poseutil-0.0.2/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:49:49.662973 poseutil-0.0.2/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      364 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.2/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 01:49:49.666333 poseutil-0.0.2/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 01:49:04.000000 poseutil-0.0.2/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:49:49.665771 poseutil-0.0.2/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.2/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.2/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.2/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    12688 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.2/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     3512 2023-07-19 01:20:40.000000 poseutil-0.0.2/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 02:09:53.862319 poseutil-0.0.3/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 02:09:53.862144 poseutil-0.0.3/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 02:09:53.858178 poseutil-0.0.3/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.3/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 02:09:53.000000 poseutil-0.0.3/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 02:09:53.862366 poseutil-0.0.3/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 02:09:44.000000 poseutil-0.0.3/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 02:09:53.861824 poseutil-0.0.3/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.3/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8049 2023-07-19 02:08:21.000000 poseutil-0.0.3/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.3/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.3/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    12688 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.3/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     3512 2023-07-19 01:20:40.000000 poseutil-0.0.3/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.3/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.3/utils/version.py
```

### Comparing `poseutil-0.0.2/setup.py` & `poseutil-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.0.2',
+    version='0.0.3',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.0.2/utils/ReadFrameData.py` & `poseutil-0.0.3/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/const.py` & `poseutil-0.0.3/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/csvHelper.py` & `poseutil-0.0.3/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/cv_util.py` & `poseutil-0.0.3/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/math_util.py` & `poseutil-0.0.3/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/normarlize.py` & `poseutil-0.0.3/utils/normarlize.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/poseMeasure.py` & `poseutil-0.0.3/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/poseMeasureFormat.py` & `poseutil-0.0.3/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/pose_util.py` & `poseutil-0.0.3/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.2/utils/version.py` & `poseutil-0.0.3/utils/version.py`

 * *Files identical despite different names*

