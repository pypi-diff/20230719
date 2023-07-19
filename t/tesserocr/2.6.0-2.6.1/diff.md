# Comparing `tmp/tesserocr-2.6.0.tar.gz` & `tmp/tesserocr-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesserocr-2.6.0.tar", last modified: Tue Mar 14 12:54:18 2023, max compression
+gzip compressed data, was "tesserocr-2.6.1.tar", last modified: Wed Jul 19 13:28:32 2023, max compression
```

## Comparing `tesserocr-2.6.0.tar` & `tesserocr-2.6.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 fz        (1000) fz        (1000)        0 2023-03-14 12:54:18.326918 tesserocr-2.6.0/
--rw-r--r--   0 fz        (1000) fz        (1000)     1082 2019-11-08 22:49:38.000000 tesserocr-2.6.0/LICENSE
--rw-r--r--   0 fz        (1000) fz        (1000)      105 2021-06-19 20:02:07.000000 tesserocr-2.6.0/MANIFEST.in
--rw-r--r--   0 fz        (1000) fz        (1000)    12520 2023-03-14 12:54:18.325920 tesserocr-2.6.0/PKG-INFO
--rw-r--r--   0 fz        (1000) fz        (1000)     8884 2021-09-14 12:55:56.000000 tesserocr-2.6.0/README.rst
--rw-r--r--   0 fz        (1000) fz        (1000)       38 2023-03-14 12:54:18.326918 tesserocr-2.6.0/setup.cfg
--rw-r--r--   0 fz        (1000) fz        (1000)    11241 2023-03-13 15:14:00.000000 tesserocr-2.6.0/setup.py
--rw-r--r--   0 fz        (1000) fz        (1000)    20672 2021-09-14 16:48:53.000000 tesserocr-2.6.0/tesseract.pxd
--rw-r--r--   0 fz        (1000) fz        (1000)    14365 2023-03-13 15:13:32.000000 tesserocr-2.6.0/tesseract5.pxd
-drwxr-xr-x   0 fz        (1000) fz        (1000)        0 2023-03-14 12:54:18.320934 tesserocr-2.6.0/tesserocr.egg-info/
--rw-r--r--   0 fz        (1000) fz        (1000)    12520 2023-03-14 12:54:17.000000 tesserocr-2.6.0/tesserocr.egg-info/PKG-INFO
--rw-r--r--   0 fz        (1000) fz        (1000)      294 2023-03-14 12:54:18.000000 tesserocr-2.6.0/tesserocr.egg-info/SOURCES.txt
--rw-r--r--   0 fz        (1000) fz        (1000)        1 2023-03-14 12:54:17.000000 tesserocr-2.6.0/tesserocr.egg-info/dependency_links.txt
--rw-r--r--   0 fz        (1000) fz        (1000)       10 2023-03-14 12:54:17.000000 tesserocr-2.6.0/tesserocr.egg-info/top_level.txt
--rw-r--r--   0 fz        (1000) fz        (1000)    97593 2023-03-14 12:52:05.000000 tesserocr-2.6.0/tesserocr.pyx
--rw-r--r--   0 fz        (1000) fz        (1000)     5614 2019-11-08 22:49:38.000000 tesserocr-2.6.0/tesserocr_experiment.pyx
-drwxr-xr-x   0 fz        (1000) fz        (1000)        0 2023-03-14 12:54:18.323926 tesserocr-2.6.0/tests/
--rw-r--r--   0 fz        (1000) fz        (1000)        0 2019-11-08 22:49:38.000000 tesserocr-2.6.0/tests/__init__.py
--rw-r--r--   0 fz        (1000) fz        (1000)    14756 2021-06-19 20:02:07.000000 tesserocr-2.6.0/tests/eurotext.png
--rw-r--r--   0 fz        (1000) fz        (1000)    13971 2021-06-19 20:02:07.000000 tesserocr-2.6.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:28:32.548594 tesserocr-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-19 13:28:26.000000 tesserocr-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 13:28:26.000000 tesserocr-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-19 13:28:32.548594 tesserocr-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-19 13:28:26.000000 tesserocr-2.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-19 13:28:26.000000 tesserocr-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:28:32.548594 tesserocr-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-07-19 13:28:26.000000 tesserocr-2.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tesseract.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tesseract5.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:28:32.548594 tesserocr-2.6.1/tesserocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-19 13:28:30.000000 tesserocr-2.6.1/tesserocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-19 13:28:32.000000 tesserocr-2.6.1/tesserocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:28:30.000000 tesserocr-2.6.1/tesserocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 13:28:30.000000 tesserocr-2.6.1/tesserocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    97593 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tesserocr.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tesserocr_experiment.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:28:32.548594 tesserocr-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tests/eurotext.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13971 2023-07-19 13:28:26.000000 tesserocr-2.6.1/tests/test_api.py
```

### Comparing `tesserocr-2.6.0/LICENSE` & `tesserocr-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tesserocr-2.6.0/PKG-INFO` & `tesserocr-2.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tesserocr
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple, Pillow-friendly, Python wrapper around tesseract-ocr API using Cython
 Home-page: https://github.com/sirfz/tesserocr
 Author: Fayez Zouheiry
 Author-email: iamfayez@gmail.com
 License: MIT
 Description: =========
         tesserocr
         =========
         
         A simple, |Pillow|_-friendly,
         wrapper around the ``tesseract-ocr`` API for Optical Character Recognition
         (OCR).
         
-        .. image:: https://travis-ci.com/sirfz/tesserocr.svg?branch=master
-            :target: https://travis-ci.com/sirfz/tesserocr
-            :alt: TravisCI build status
+        .. image:: https://github.com/sirfz/tesserocr/actions/workflows/build.yml/badge.svg
+            :target: https://github.com/sirfz/tesserocr/actions/workflows/build.yml
+            :alt: Github Actions build status
         
         .. image:: https://img.shields.io/pypi/v/tesserocr.svg?maxAge=2592000
             :target: https://pypi.python.org/pypi/tesserocr
             :alt: Latest version on PyPi
         
         .. image:: https://img.shields.io/pypi/pyversions/tesserocr.svg?maxAge=2592000
             :alt: Supported python versions
```

### Comparing `tesserocr-2.6.0/README.rst` & `tesserocr-2.6.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 tesserocr
 =========
 
 A simple, |Pillow|_-friendly,
 wrapper around the ``tesseract-ocr`` API for Optical Character Recognition
 (OCR).
 
-.. image:: https://travis-ci.com/sirfz/tesserocr.svg?branch=master
-    :target: https://travis-ci.com/sirfz/tesserocr
-    :alt: TravisCI build status
+.. image:: https://github.com/sirfz/tesserocr/actions/workflows/build.yml/badge.svg
+    :target: https://github.com/sirfz/tesserocr/actions/workflows/build.yml
+    :alt: Github Actions build status
 
 .. image:: https://img.shields.io/pypi/v/tesserocr.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/tesserocr
     :alt: Latest version on PyPi
 
 .. image:: https://img.shields.io/pypi/pyversions/tesserocr.svg?maxAge=2592000
     :alt: Supported python versions
```

### Comparing `tesserocr-2.6.0/setup.py` & `tesserocr-2.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,9 +324,9 @@
         'Programming Language :: Cython',
     ],
     keywords='Tesseract,tesseract-ocr,OCR,optical character recognition,'
     'PIL,Pillow,Cython',
     cmdclass={'build_ext': my_build_ext},
     ext_modules=[make_extension()],
     test_suite='tests',
-    setup_requires=['Cython>=0.23'],
+    setup_requires=['Cython>=0.23,<3.0.0'],
 )
```

### Comparing `tesserocr-2.6.0/tesseract.pxd` & `tesserocr-2.6.1/tesseract.pxd`

 * *Files identical despite different names*

### Comparing `tesserocr-2.6.0/tesseract5.pxd` & `tesserocr-2.6.1/tesseract5.pxd`

 * *Files identical despite different names*

### Comparing `tesserocr-2.6.0/tesserocr.egg-info/PKG-INFO` & `tesserocr-2.6.1/tesserocr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tesserocr
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple, Pillow-friendly, Python wrapper around tesseract-ocr API using Cython
 Home-page: https://github.com/sirfz/tesserocr
 Author: Fayez Zouheiry
 Author-email: iamfayez@gmail.com
 License: MIT
 Description: =========
         tesserocr
         =========
         
         A simple, |Pillow|_-friendly,
         wrapper around the ``tesseract-ocr`` API for Optical Character Recognition
         (OCR).
         
-        .. image:: https://travis-ci.com/sirfz/tesserocr.svg?branch=master
-            :target: https://travis-ci.com/sirfz/tesserocr
-            :alt: TravisCI build status
+        .. image:: https://github.com/sirfz/tesserocr/actions/workflows/build.yml/badge.svg
+            :target: https://github.com/sirfz/tesserocr/actions/workflows/build.yml
+            :alt: Github Actions build status
         
         .. image:: https://img.shields.io/pypi/v/tesserocr.svg?maxAge=2592000
             :target: https://pypi.python.org/pypi/tesserocr
             :alt: Latest version on PyPi
         
         .. image:: https://img.shields.io/pypi/pyversions/tesserocr.svg?maxAge=2592000
             :alt: Supported python versions
```

### Comparing `tesserocr-2.6.0/tesserocr.pyx` & `tesserocr-2.6.1/tesserocr.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     leptonica-1.72
     libjpeg 8d (libjpeg-turbo 1.3.0) : libpng 1.2.51 : libtiff 4.0.3 : zlib 1.2.8
 >>> get_languages()
 ('/usr/share/tesseract-ocr/tessdata/',
  ['eng', 'osd', 'equ'])
 """
 
-__version__ = '2.6.0'
+__version__ = '2.6.1'
 
 import os
 from io import BytesIO
 from os.path import abspath, join
 try:
     from PIL import Image
 except ImportError:
```

### Comparing `tesserocr-2.6.0/tesserocr_experiment.pyx` & `tesserocr-2.6.1/tesserocr_experiment.pyx`

 * *Files identical despite different names*

### Comparing `tesserocr-2.6.0/tests/eurotext.png` & `tesserocr-2.6.1/tests/eurotext.png`

 * *Files identical despite different names*

### Comparing `tesserocr-2.6.0/tests/test_api.py` & `tesserocr-2.6.1/tests/test_api.py`

 * *Files identical despite different names*

