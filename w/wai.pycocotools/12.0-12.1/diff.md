# Comparing `tmp/wai.pycocotools-12.0.tar.gz` & `tmp/wai.pycocotools-12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wai.pycocotools-12.0.tar", last modified: Mon Jul 27 03:14:46 2020, max compression
+gzip compressed data, was "wai.pycocotools-12.1.tar", last modified: Tue Jul 18 22:29:48 2023, max compression
```

## Comparing `wai.pycocotools-12.0.tar` & `wai.pycocotools-12.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 csterlin (188385) csterlin (188385)        0 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/
--rw-r--r--   0 csterlin (188385) csterlin (188385)       93 2020-07-27 03:01:10.000000 wai.pycocotools-12.0/MANIFEST.in
--rw-rw-r--   0 csterlin (188385) csterlin (188385)      312 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/PKG-INFO
-drwxrwxr-x   0 csterlin (188385) csterlin (188385)        0 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/common/
--rw-r--r--   0 csterlin (188385) csterlin (188385)     9540 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/common/gason.cpp
--rw-r--r--   0 csterlin (188385) csterlin (188385)     3483 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/common/gason.h
--rw-r--r--   0 csterlin (188385) csterlin (188385)     8308 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/common/maskApi.c
--rw-r--r--   0 csterlin (188385) csterlin (188385)     2176 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/common/maskApi.h
--rw-r--r--   0 csterlin (188385) csterlin (188385)     1529 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/license.txt
-drwxrwxr-x   0 csterlin (188385) csterlin (188385)        0 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/pycocotools/
--rw-r--r--   0 csterlin (188385) csterlin (188385)       44 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/pycocotools/__init__.py
--rw-r--r--   0 csterlin (188385) csterlin (188385)    11440 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/pycocotools/_mask.pyx
--rw-r--r--   0 csterlin (188385) csterlin (188385)    20662 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/pycocotools/coco.py
--rw-r--r--   0 csterlin (188385) csterlin (188385)    25707 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/pycocotools/cocoeval.py
--rw-r--r--   0 csterlin (188385) csterlin (188385)     4630 2020-07-27 02:43:19.000000 wai.pycocotools-12.0/pycocotools/mask.py
--rw-rw-r--   0 csterlin (188385) csterlin (188385)       38 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/setup.cfg
--rw-r--r--   0 csterlin (188385) csterlin (188385)     1150 2020-07-27 03:10:11.000000 wai.pycocotools-12.0/setup.py
-drwxrwxr-x   0 csterlin (188385) csterlin (188385)        0 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/wai.pycocotools.egg-info/
--rw-rw-r--   0 csterlin (188385) csterlin (188385)      312 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/wai.pycocotools.egg-info/PKG-INFO
--rw-rw-r--   0 csterlin (188385) csterlin (188385)      402 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/wai.pycocotools.egg-info/SOURCES.txt
--rw-rw-r--   0 csterlin (188385) csterlin (188385)        1 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/wai.pycocotools.egg-info/dependency_links.txt
--rw-rw-r--   0 csterlin (188385) csterlin (188385)       50 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/wai.pycocotools.egg-info/requires.txt
--rw-rw-r--   0 csterlin (188385) csterlin (188385)       12 2020-07-27 03:14:46.000000 wai.pycocotools-12.0/wai.pycocotools.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-18 22:29:48.177456 wai.pycocotools-12.1/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       93 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      312 2023-07-18 22:29:48.177456 wai.pycocotools-12.1/PKG-INFO
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-18 22:29:48.177456 wai.pycocotools-12.1/common/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     9540 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/common/gason.cpp
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3483 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/common/gason.h
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8308 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/common/maskApi.c
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2176 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/common/maskApi.h
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1529 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/license.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-18 22:29:48.177456 wai.pycocotools-12.1/pycocotools/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/pycocotools/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11440 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/pycocotools/_mask.pyx
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    20662 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/pycocotools/coco.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    25707 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/pycocotools/cocoeval.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4630 2022-05-17 03:15:38.000000 wai.pycocotools-12.1/pycocotools/mask.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-18 22:29:48.177456 wai.pycocotools-12.1/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1158 2023-07-18 22:02:28.000000 wai.pycocotools-12.1/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-18 22:29:48.177456 wai.pycocotools-12.1/wai.pycocotools.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      312 2023-07-18 22:29:48.000000 wai.pycocotools-12.1/wai.pycocotools.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      402 2023-07-18 22:29:48.000000 wai.pycocotools-12.1/wai.pycocotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-18 22:29:48.000000 wai.pycocotools-12.1/wai.pycocotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       57 2023-07-18 22:29:48.000000 wai.pycocotools-12.1/wai.pycocotools.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       12 2023-07-18 22:29:48.000000 wai.pycocotools-12.1/wai.pycocotools.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wai.pycocotools-12.0/common/gason.cpp` & `wai.pycocotools-12.1/common/gason.cpp`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/common/gason.h` & `wai.pycocotools-12.1/common/gason.h`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/common/maskApi.c` & `wai.pycocotools-12.1/common/maskApi.c`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/common/maskApi.h` & `wai.pycocotools-12.1/common/maskApi.h`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/license.txt` & `wai.pycocotools-12.1/license.txt`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/pycocotools/_mask.pyx` & `wai.pycocotools-12.1/pycocotools/_mask.pyx`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/pycocotools/coco.py` & `wai.pycocotools-12.1/pycocotools/coco.py`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/pycocotools/cocoeval.py` & `wai.pycocotools-12.1/pycocotools/cocoeval.py`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/pycocotools/mask.py` & `wai.pycocotools-12.1/pycocotools/mask.py`

 * *Files identical despite different names*

### Comparing `wai.pycocotools-12.0/setup.py` & `wai.pycocotools-12.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
       classifiers=[
           'License :: OSI Approved :: BSD License'
       ],
       license='BSD License',
       packages=['pycocotools'],
       package_dir={'pycocotools': 'pycocotools'},
       install_requires=[
-          'setuptools>=18.0', 'cython>=0.27.3', 'matplotlib>=2.1.0'
+          'setuptools>=18.0', 'cython>=0.27.3, <3.0.0', 'matplotlib>=2.1.0'
       ],
-      version='12.0',
+      version='12.1',
       ext_modules=ext_modules)
```

