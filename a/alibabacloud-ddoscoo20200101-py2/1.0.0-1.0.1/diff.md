# Comparing `tmp/alibabacloud_ddoscoo20200101_py2-1.0.0.tar.gz` & `tmp/alibabacloud_ddoscoo20200101_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ddoscoo20200101_py2-1.0.0.tar", last modified: Thu Jun 30 07:39:36 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ddoscoo20200101_py2-1.0.1.tar", last modified: Wed Jul 19 02:36:51 2023, max compression
```

## Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0.tar` & `alibabacloud_ddoscoo20200101_py2-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)       49 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200920 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101/client.py
--rw-r--r--   0 root         (0) root         (0)   734385 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2923 2022-06-30 07:39:36.000000 alibabacloud_ddoscoo20200101_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   263246 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)   968767 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 02:36:51.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-07-19 02:36:50.000000 alibabacloud_ddoscoo20200101_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0/LICENSE` & `alibabacloud_ddoscoo20200101_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0/PKG-INFO` & `alibabacloud_ddoscoo20200101_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ddoscoo20200101_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ddoscoo (20200101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0/README-CN.md` & `alibabacloud_ddoscoo20200101_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0/README.md` & `alibabacloud_ddoscoo20200101_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0/alibabacloud_ddoscoo20200101_py2.egg-info/PKG-INFO` & `alibabacloud_ddoscoo20200101_py2-1.0.1/alibabacloud_ddoscoo20200101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ddoscoo20200101-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ddoscoo (20200101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ddoscoo20200101_py2-1.0.0/setup.py` & `alibabacloud_ddoscoo20200101_py2-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ddoscoo20200101_py2.
 
-Created on 30/06/2022
+Created on 19/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ddoscoo20200101"
 NAME = "alibabacloud_ddoscoo20200101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ddoscoo (20200101) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

