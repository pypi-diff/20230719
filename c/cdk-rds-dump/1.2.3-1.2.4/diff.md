# Comparing `tmp/cdk-rds-dump-1.2.3.tar.gz` & `tmp/cdk-rds-dump-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-1.2.3.tar", last modified: Tue Jul 18 14:20:15 2023, max compression
+gzip compressed data, was "cdk-rds-dump-1.2.4.tar", last modified: Tue Jul 18 15:20:55 2023, max compression
```

## Comparing `cdk-rds-dump-1.2.3.tar` & `cdk-rds-dump-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.084325 cdk-rds-dump-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-18 14:20:15.084325 cdk-rds-dump-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:20:15.084325 cdk-rds-dump-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2576417 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:20:55.720733 cdk-rds-dump-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-18 15:20:55.720733 cdk-rds-dump-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:20:55.720733 cdk-rds-dump-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:20:55.716733 cdk-rds-dump-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:20:55.716733 cdk-rds-dump-1.2.4/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:20:55.720733 cdk-rds-dump-1.2.4/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2576428 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:20:40.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:20:55.716733 cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-18 15:20:55.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 15:20:55.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:20:55.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:20:55.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:20:55.000000 cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-1.2.3/LICENSE` & `cdk-rds-dump-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.3/PKG-INFO` & `cdk-rds-dump-1.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.3
+Version: 1.2.4
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,19 +24,20 @@
 
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-rds-dump)](https://constructs.dev/packages/cdk-rds-dump)
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
 
 Install from npm:
 
 ```sh
```

### Comparing `cdk-rds-dump-1.2.3/README.md` & `cdk-rds-dump-1.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-rds-dump)](https://constructs.dev/packages/cdk-rds-dump)
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
 
 Install from npm:
 
 ```sh
```

### Comparing `cdk-rds-dump-1.2.3/setup.py` & `cdk-rds-dump-1.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "1.2.3",
+    "version": "1.2.4",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@1.2.3.jsii.tgz"
+            "cdk-rds-dump@1.2.4.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-rds-dump-1.2.3/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-1.2.4/src/cdk_rds_dump/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 '''
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-rds-dump)](https://constructs.dev/packages/cdk-rds-dump)
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
 
 Install from npm:
 
 ```sh
```

### Comparing `cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-1.2.4/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.3
+Version: 1.2.4
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,19 +24,20 @@
 
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-rds-dump)](https://constructs.dev/packages/cdk-rds-dump)
 [![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
 
 Install from npm:
 
 ```sh
```

