# Comparing `tmp/OnloadTable-0.3.3.tar.gz` & `tmp/OnloadTable-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnloadTable-0.3.3.tar", last modified: Fri May 12 01:52:02 2023, max compression
+gzip compressed data, was "OnloadTable-0.3.4.tar", last modified: Wed Jul 19 07:04:36 2023, max compression
```

## Comparing `OnloadTable-0.3.3.tar` & `OnloadTable-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.829961 OnloadTable-0.3.3/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 OnloadTable-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 OnloadTable-0.3.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.809961 OnloadTable-0.3.3/OnloadTable/
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.819961 OnloadTable-0.3.3/OnloadTable/Function/
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.820962 OnloadTable-0.3.3/OnloadTable/Function/Function/
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.3/OnloadTable/Function/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.825961 OnloadTable-0.3.3/OnloadTable/Function/Ui/
--rw-rw-rw-   0        0        0    46080 2023-04-28 06:34:36.000000 OnloadTable-0.3.3/OnloadTable/Function/Ui/ExcelUi.pyd
--rw-rw-rw-   0        0        0    40448 2023-04-28 06:34:44.000000 OnloadTable-0.3.3/OnloadTable/Function/Ui/MaskWin.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.3/OnloadTable/Function/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.3/OnloadTable/Function/__init__.py
--rw-rw-rw-   0        0        0   290816 2023-05-05 13:21:34.000000 OnloadTable-0.3.3/OnloadTable/Function/mysqlexcel.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:24:22.000000 OnloadTable-0.3.3/OnloadTable/Function/optionDb.pyd
--rw-rw-rw-   0        0        0       36 2023-03-01 03:36:32.000000 OnloadTable-0.3.3/OnloadTable/Function/settings.py
--rw-rw-rw-   0        0        0   249344 2023-05-12 01:47:39.000000 OnloadTable-0.3.3/OnloadTable/OnloadTable.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.828961 OnloadTable-0.3.3/OnloadTable/Ui/
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.3/OnloadTable/Ui/__init__.py
--rw-rw-rw-   0        0        0    90112 2023-04-28 06:24:14.000000 OnloadTable-0.3.3/OnloadTable/Ui/onloadUi.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.3/OnloadTable/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 01:52:02.814961 OnloadTable-0.3.3/OnloadTable.egg-info/
--rw-rw-rw-   0        0        0      394 2023-05-12 01:52:02.000000 OnloadTable-0.3.3/OnloadTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      585 2023-05-12 01:52:02.000000 OnloadTable-0.3.3/OnloadTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 01:52:02.000000 OnloadTable-0.3.3/OnloadTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-12 01:52:02.000000 OnloadTable-0.3.3/OnloadTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      394 2023-05-12 01:52:02.829961 OnloadTable-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 OnloadTable-0.3.3/README.md
--rw-rw-rw-   0        0        0      136 2023-05-12 01:52:02.830961 OnloadTable-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      966 2023-05-12 01:38:42.000000 OnloadTable-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.720596 OnloadTable-0.3.4/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 OnloadTable-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 OnloadTable-0.3.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.685594 OnloadTable-0.3.4/OnloadTable/
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.703594 OnloadTable-0.3.4/OnloadTable/Function/
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.705594 OnloadTable-0.3.4/OnloadTable/Function/Function/
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.4/OnloadTable/Function/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.712594 OnloadTable-0.3.4/OnloadTable/Function/Ui/
+-rw-rw-rw-   0        0        0    46080 2023-04-28 06:34:36.000000 OnloadTable-0.3.4/OnloadTable/Function/Ui/ExcelUi.pyd
+-rw-rw-rw-   0        0        0    40448 2023-04-28 06:34:44.000000 OnloadTable-0.3.4/OnloadTable/Function/Ui/MaskWin.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.4/OnloadTable/Function/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.4/OnloadTable/Function/__init__.py
+-rw-rw-rw-   0        0        0   290816 2023-05-05 13:21:34.000000 OnloadTable-0.3.4/OnloadTable/Function/mysqlexcel.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:24:22.000000 OnloadTable-0.3.4/OnloadTable/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0       36 2023-03-01 03:36:32.000000 OnloadTable-0.3.4/OnloadTable/Function/settings.py
+-rw-rw-rw-   0        0        0   247296 2023-07-19 06:49:42.000000 OnloadTable-0.3.4/OnloadTable/OnloadTable.pyd
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.717596 OnloadTable-0.3.4/OnloadTable/Ui/
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.4/OnloadTable/Ui/__init__.py
+-rw-rw-rw-   0        0        0    90112 2023-04-28 06:24:14.000000 OnloadTable-0.3.4/OnloadTable/Ui/onloadUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.4/OnloadTable/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:04:36.693594 OnloadTable-0.3.4/OnloadTable.egg-info/
+-rw-rw-rw-   0        0        0      394 2023-07-19 07:04:36.000000 OnloadTable-0.3.4/OnloadTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-07-19 07:04:36.000000 OnloadTable-0.3.4/OnloadTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:04:36.000000 OnloadTable-0.3.4/OnloadTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-19 07:04:36.000000 OnloadTable-0.3.4/OnloadTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      394 2023-07-19 07:04:36.721596 OnloadTable-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 OnloadTable-0.3.4/README.md
+-rw-rw-rw-   0        0        0      136 2023-07-19 07:04:36.722597 OnloadTable-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      966 2023-05-18 09:19:33.000000 OnloadTable-0.3.4/setup.py
```

### Comparing `OnloadTable-0.3.3/LICENSE.txt` & `OnloadTable-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnloadTable-0.3.3/OnloadTable.egg-info/SOURCES.txt` & `OnloadTable-0.3.4/OnloadTable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnloadTable-0.3.3/setup.py` & `OnloadTable-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "OnloadTable",
```

