# Comparing `tmp/alibabacloud_bailian20230601-1.0.0.tar.gz` & `tmp/alibabacloud_bailian20230601-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bailian20230601-1.0.0.tar", last modified: Tue Jul  4 12:30:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bailian20230601-1.1.0.tar", last modified: Wed Jul 19 07:07:57 2023, max compression
```

## Comparing `alibabacloud_bailian20230601-1.0.0.tar` & `alibabacloud_bailian20230601-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4039 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601/client.py
--rw-r--r--   0 root         (0) root         (0)     4852 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      439 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 12:30:34.000000 alibabacloud_bailian20230601-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2023-07-04 12:30:33.000000 alibabacloud_bailian20230601-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33175 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601/client.py
+-rw-r--r--   0 root         (0) root         (0)    50155 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-07-19 07:07:57.000000 alibabacloud_bailian20230601-1.1.0/setup.py
```

### Comparing `alibabacloud_bailian20230601-1.0.0/LICENSE` & `alibabacloud_bailian20230601-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bailian20230601-1.0.0/PKG-INFO` & `alibabacloud_bailian20230601-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bailian20230601
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud bailian (20230601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bailian20230601-1.0.0/README-CN.md` & `alibabacloud_bailian20230601-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bailian20230601-1.0.0/README.md` & `alibabacloud_bailian20230601-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bailian20230601-1.0.0/alibabacloud_bailian20230601.egg-info/PKG-INFO` & `alibabacloud_bailian20230601-1.1.0/alibabacloud_bailian20230601.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bailian20230601
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud bailian (20230601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bailian20230601-1.0.0/setup.py` & `alibabacloud_bailian20230601-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bailian20230601.
 
-Created on 04/07/2023
+Created on 19/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bailian20230601"
 NAME = "alibabacloud_bailian20230601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud bailian (20230601) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

