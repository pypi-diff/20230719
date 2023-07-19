# Comparing `tmp/ros-cdk-pai-1.0.15.tar.gz` & `tmp/ros-cdk-pai-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-pai-1.0.15.tar", last modified: Wed Jun 28 10:20:38 2023, max compression
+gzip compressed data, was "dist/ros-cdk-pai-1.0.16.tar", last modified: Wed Jul 19 02:37:47 2023, max compression
```

## Comparing `ros-cdk-pai-1.0.15.tar` & `ros-cdk-pai-1.0.16.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1875 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai/
--rw-r--r--   0 root         (0) root         (0)   124936 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58354 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai/_jsii/ros-cdk-pai@1.0.15.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 10:20:37.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-28 10:20:38.000000 ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai/
+-rw-r--r--   0 root         (0) root         (0)   124936 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68206 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai/_jsii/ros-cdk-pai@1.0.16.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-19 02:37:47.000000 ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/top_level.txt
```

### Comparing `ros-cdk-pai-1.0.15/LICENSE` & `ros-cdk-pai-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-pai-1.0.15/PKG-INFO` & `ros-cdk-pai-1.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-pai
-Version: 1.0.15
+Version: 1.0.16
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PAI Construct Library
```

### Comparing `ros-cdk-pai-1.0.15/setup.py` & `ros-cdk-pai-1.0.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-pai",
-    "version": "1.0.15",
+    "version": "1.0.16",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "ros_cdk_pai",
         "ros_cdk_pai._jsii"
     ],
     "package_data": {
         "ros_cdk_pai._jsii": [
-            "ros-cdk-pai@1.0.15.jsii.tgz"
+            "ros-cdk-pai@1.0.16.jsii.tgz"
         ],
         "ros_cdk_pai": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `ros-cdk-pai-1.0.15/src/ros_cdk_pai/__init__.py` & `ros-cdk-pai-1.0.16/src/ros_cdk_pai/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-pai-1.0.15/src/ros_cdk_pai.egg-info/PKG-INFO` & `ros-cdk-pai-1.0.16/src/ros_cdk_pai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-pai
-Version: 1.0.15
+Version: 1.0.16
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PAI Construct Library
```

