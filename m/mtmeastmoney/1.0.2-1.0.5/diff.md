# Comparing `tmp/mtmeastmoney-1.0.2.tar.gz` & `tmp/mtmeastmoney-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmeastmoney-1.0.2.tar", last modified: Thu Apr 20 05:33:27 2023, max compression
+gzip compressed data, was "mtmeastmoney-1.0.5.tar", last modified: Wed Jul 19 13:14:39 2023, max compression
```

## Comparing `mtmeastmoney-1.0.2.tar` & `mtmeastmoney-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 05:33:27.534497 mtmeastmoney-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-04-20 05:33:27.534497 mtmeastmoney-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 05:33:27.534497 mtmeastmoney-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 05:33:27.534497 mtmeastmoney-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 05:33:27.534497 mtmeastmoney-1.0.2/src/mtmeastmoney/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/src/mtmeastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/src/mtmeastmoney/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/src/mtmeastmoney/dbaccount.py
--rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/src/mtmeastmoney/eastmoney.py
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-20 05:33:19.000000 mtmeastmoney-1.0.2/src/mtmeastmoney/ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 05:33:27.534497 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-04-20 05:33:27.000000 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-20 05:33:27.000000 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 05:33:27.000000 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 05:33:27.000000 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 05:33:27.000000 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-20 05:33:27.000000 mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.857837 mtmeastmoney-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/src/mtmeastmoney/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/dbaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8454 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/eastmoney.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3279 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/jointquant.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/tiantianfund.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/top_level.txt
```

### Comparing `mtmeastmoney-1.0.2/LICENSE` & `mtmeastmoney-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.2/PKG-INFO` & `mtmeastmoney-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmeastmoney
-Version: 1.0.2
+Version: 1.0.5
 Summary: A Personal Eastmoney Library
 Home-page: https://github.com/imutum/imutum_eastmoney_library
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmeastmoney-1.0.2/setup.py` & `mtmeastmoney-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = 'imutum_eastmoney_library'
 abbreviation_name = "mtmeastmoney"
 description = "A Personal Eastmoney Library"
-version = "1.0.2"
+version = "1.0.5"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmeastmoney-1.0.2/src/mtmeastmoney/common.py` & `mtmeastmoney-1.0.5/src/mtmeastmoney/common.py`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.2/src/mtmeastmoney/dbaccount.py` & `mtmeastmoney-1.0.5/src/mtmeastmoney/dbaccount.py`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.2/src/mtmeastmoney.egg-info/PKG-INFO` & `mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmeastmoney
-Version: 1.0.2
+Version: 1.0.5
 Summary: A Personal Eastmoney Library
 Home-page: https://github.com/imutum/imutum_eastmoney_library
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

