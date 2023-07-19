# Comparing `tmp/cdk8s-plus-24-2.8.96.tar.gz` & `tmp/cdk8s-plus-24-2.8.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-24-2.8.96.tar", last modified: Tue Jul 18 00:29:35 2023, max compression
+gzip compressed data, was "cdk8s-plus-24-2.8.97.tar", last modified: Tue Jul 18 02:41:26 2023, max compression
```

## Comparing `cdk8s-plus-24-2.8.96.tar` & `cdk8s-plus-24-2.8.97.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:29:35.136450 cdk8s-plus-24-2.8.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-18 00:29:35.136450 cdk8s-plus-24-2.8.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 00:29:35.136450 cdk8s-plus-24-2.8.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:29:35.124450 cdk8s-plus-24-2.8.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:29:35.128450 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/
--rw-r--r--   0 runner    (1001) docker     (123)  1161790 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:29:35.128450 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1279961 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/_jsii/cdk8s-plus-24@2.8.96.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:29:35.132450 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2878966 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:29:18.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:29:35.128450 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-18 00:29:35.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 00:29:35.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:29:35.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 00:29:35.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 00:29:35.000000 cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:41:26.025774 cdk8s-plus-24-2.8.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-18 02:41:26.025774 cdk8s-plus-24-2.8.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:41:26.025774 cdk8s-plus-24-2.8.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:41:26.017773 cdk8s-plus-24-2.8.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:41:26.021774 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/
+-rw-r--r--   0 runner    (1001) docker     (123)  1161790 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:41:26.021774 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1279964 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/_jsii/cdk8s-plus-24@2.8.97.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:41:26.021774 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2878966 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:41:14.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:41:26.021774 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-18 02:41:25.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 02:41:25.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:41:25.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 02:41:25.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 02:41:25.000000 cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-24-2.8.96/LICENSE` & `cdk8s-plus-24-2.8.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.96/PKG-INFO` & `cdk8s-plus-24-2.8.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-24
-Version: 2.8.96
+Version: 2.8.97
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-24-2.8.96/README.md` & `cdk8s-plus-24-2.8.97/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.96/setup.py` & `cdk8s-plus-24-2.8.97/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-24",
-    "version": "2.8.96",
+    "version": "2.8.97",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,25 +23,25 @@
     "packages": [
         "cdk8s_plus_24",
         "cdk8s_plus_24._jsii",
         "cdk8s_plus_24.k8s"
     ],
     "package_data": {
         "cdk8s_plus_24._jsii": [
-            "cdk8s-plus-24@2.8.96.jsii.tgz"
+            "cdk8s-plus-24@2.8.97.jsii.tgz"
         ],
         "cdk8s_plus_24": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdk8s>=2.7.112, <3.0.0",
+        "cdk8s>=2.7.114, <3.0.0",
         "constructs>=10.2.69, <11.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/__init__.py` & `cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.96/src/cdk8s_plus_24/k8s/__init__.py` & `cdk8s-plus-24-2.8.97/src/cdk8s_plus_24/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.96/src/cdk8s_plus_24.egg-info/PKG-INFO` & `cdk8s-plus-24-2.8.97/src/cdk8s_plus_24.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-24
-Version: 2.8.96
+Version: 2.8.97
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

