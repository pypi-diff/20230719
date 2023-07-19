# Comparing `tmp/cdk-datadog-integration-2.1.3.tar.gz` & `tmp/cdk-datadog-integration-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-datadog-integration-2.1.3.tar", last modified: Mon Jun 19 00:23:26 2023, max compression
+gzip compressed data, was "cdk-datadog-integration-2.1.4.tar", last modified: Wed Jul 19 09:22:55 2023, max compression
```

## Comparing `cdk-datadog-integration-2.1.3.tar` & `cdk-datadog-integration-2.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.468894 cdk-datadog-integration-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    61591 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35298 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/_jsii/cdk-datadog-integration@2.1.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    62073 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35769 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/_jsii/cdk-datadog-integration@2.1.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:22:43.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:22:55.878189 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-19 09:22:55.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-19 09:22:55.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:22:55.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 09:22:55.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 09:22:55.000000 cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/top_level.txt
```

### Comparing `cdk-datadog-integration-2.1.3/LICENSE` & `cdk-datadog-integration-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-datadog-integration-2.1.3/PKG-INFO` & `cdk-datadog-integration-2.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-datadog-integration
-Version: 2.1.3
+Version: 2.1.4
 Summary: cdk-datadog-integration
 Home-page: https://github.com/blimmer/cdk-datadog-integration.git
 Author: Ben Limmer
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-datadog-integration.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,24 @@
 # AWS Cloud Development Kit (CDK) Datadog Integration
 
 This construct makes it easy to integrate your AWS account with Datadog. It
 creates nested stacks based on the official
 [Datadog Cloudformation templates](https://github.com/DataDog/cloudformation-template/blob/master/aws/main.yaml)
 using [Amazon Cloud Development Kit (CDK)](https://aws.amazon.com/cdk/).
 
+## Warning
+
+:warning: This construct does not use the newest Datadog CloudFormation template because sensitive
+parameters must be hard-coded. See https://github.com/DataDog/cloudformation-template/issues/68 for an upstream
+feature request. :warning:
+
+This construct will still work, but it cannot be updated to the latest integration template until the upstream
+issue is fixed. Please add a +1 to https://github.com/DataDog/cloudformation-template/issues/68 to help
+prioritize it.
+
 ## Basic Usage
 
 1. Install the package
 
    ```console
    npm i --save cdk-datadog-integration
    ```
```

### Comparing `cdk-datadog-integration-2.1.3/README.md` & `cdk-datadog-integration-2.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # AWS Cloud Development Kit (CDK) Datadog Integration
 
 This construct makes it easy to integrate your AWS account with Datadog. It
 creates nested stacks based on the official
 [Datadog Cloudformation templates](https://github.com/DataDog/cloudformation-template/blob/master/aws/main.yaml)
 using [Amazon Cloud Development Kit (CDK)](https://aws.amazon.com/cdk/).
 
+## Warning
+
+:warning: This construct does not use the newest Datadog CloudFormation template because sensitive
+parameters must be hard-coded. See https://github.com/DataDog/cloudformation-template/issues/68 for an upstream
+feature request. :warning:
+
+This construct will still work, but it cannot be updated to the latest integration template until the upstream
+issue is fixed. Please add a +1 to https://github.com/DataDog/cloudformation-template/issues/68 to help
+prioritize it.
+
 ## Basic Usage
 
 1. Install the package
 
    ```console
    npm i --save cdk-datadog-integration
    ```
```

### Comparing `cdk-datadog-integration-2.1.3/setup.py` & `cdk-datadog-integration-2.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-datadog-integration",
-    "version": "2.1.3",
+    "version": "2.1.4",
     "description": "cdk-datadog-integration",
     "license": "Apache-2.0",
     "url": "https://github.com/blimmer/cdk-datadog-integration.git",
     "long_description_content_type": "text/markdown",
     "author": "Ben Limmer",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_datadog_integration",
         "cdk_datadog_integration._jsii"
     ],
     "package_data": {
         "cdk_datadog_integration._jsii": [
-            "cdk-datadog-integration@2.1.3.jsii.tgz"
+            "cdk-datadog-integration@2.1.4.jsii.tgz"
         ],
         "cdk_datadog_integration": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/__init__.py` & `cdk-datadog-integration-2.1.4/src/cdk_datadog_integration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 # AWS Cloud Development Kit (CDK) Datadog Integration
 
 This construct makes it easy to integrate your AWS account with Datadog. It
 creates nested stacks based on the official
 [Datadog Cloudformation templates](https://github.com/DataDog/cloudformation-template/blob/master/aws/main.yaml)
 using [Amazon Cloud Development Kit (CDK)](https://aws.amazon.com/cdk/).
 
+## Warning
+
+:warning: This construct does not use the newest Datadog CloudFormation template because sensitive
+parameters must be hard-coded. See https://github.com/DataDog/cloudformation-template/issues/68 for an upstream
+feature request. :warning:
+
+This construct will still work, but it cannot be updated to the latest integration template until the upstream
+issue is fixed. Please add a +1 to https://github.com/DataDog/cloudformation-template/issues/68 to help
+prioritize it.
+
 ## Basic Usage
 
 1. Install the package
 
    ```console
    npm i --save cdk-datadog-integration
    ```
```

### Comparing `cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/PKG-INFO` & `cdk-datadog-integration-2.1.4/src/cdk_datadog_integration.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-datadog-integration
-Version: 2.1.3
+Version: 2.1.4
 Summary: cdk-datadog-integration
 Home-page: https://github.com/blimmer/cdk-datadog-integration.git
 Author: Ben Limmer
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-datadog-integration.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,24 @@
 # AWS Cloud Development Kit (CDK) Datadog Integration
 
 This construct makes it easy to integrate your AWS account with Datadog. It
 creates nested stacks based on the official
 [Datadog Cloudformation templates](https://github.com/DataDog/cloudformation-template/blob/master/aws/main.yaml)
 using [Amazon Cloud Development Kit (CDK)](https://aws.amazon.com/cdk/).
 
+## Warning
+
+:warning: This construct does not use the newest Datadog CloudFormation template because sensitive
+parameters must be hard-coded. See https://github.com/DataDog/cloudformation-template/issues/68 for an upstream
+feature request. :warning:
+
+This construct will still work, but it cannot be updated to the latest integration template until the upstream
+issue is fixed. Please add a +1 to https://github.com/DataDog/cloudformation-template/issues/68 to help
+prioritize it.
+
 ## Basic Usage
 
 1. Install the package
 
    ```console
    npm i --save cdk-datadog-integration
    ```
```

