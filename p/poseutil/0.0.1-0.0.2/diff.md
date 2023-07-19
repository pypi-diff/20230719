# Comparing `tmp/poseutil-0.0.1.tar.gz` & `tmp/poseutil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.0.1.tar", last modified: Wed Jul 19 01:39:03 2023, max compression
+gzip compressed data, was "poseutil-0.0.2.tar", last modified: Wed Jul 19 01:49:49 2023, max compression
```

## Comparing `poseutil-0.0.1.tar` & `poseutil-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,21 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:39:03.238329 poseutil-0.0.1/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 01:39:03.238169 poseutil-0.0.1/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:39:03.237973 poseutil-0.0.1/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 01:39:03.000000 poseutil-0.0.1/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      167 2023-07-19 01:39:03.000000 poseutil-0.0.1/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.1/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.1/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.1/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 01:39:03.238377 poseutil-0.0.1/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      590 2023-07-19 01:36:05.000000 poseutil-0.0.1/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:49:49.666290 poseutil-0.0.2/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 01:49:49.666144 poseutil-0.0.2/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:49:49.662973 poseutil-0.0.2/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      364 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 01:39:03.000000 poseutil-0.0.2/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 01:49:49.000000 poseutil-0.0.2/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 01:49:49.666333 poseutil-0.0.2/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 01:49:04.000000 poseutil-0.0.2/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 01:49:49.665771 poseutil-0.0.2/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.2/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.2/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.2/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6641 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6665 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    12688 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72838 2023-07-19 01:21:22.000000 poseutil-0.0.2/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     3512 2023-07-19 01:20:40.000000 poseutil-0.0.2/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11583 2023-07-19 01:17:51.000000 poseutil-0.0.2/utils/version.py
```

### Comparing `poseutil-0.0.1/setup.py` & `poseutil-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.0.1',
+    version='0.0.2',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle'],
-    packages=find_packages(exclude=[]),
+    py_modules=['utils'],
+    packages=['utils'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

