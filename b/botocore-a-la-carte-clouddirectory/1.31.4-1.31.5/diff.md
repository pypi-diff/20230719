# Comparing `tmp/botocore-a-la-carte-clouddirectory-1.31.4.tar.gz` & `tmp/botocore-a-la-carte-clouddirectory-1.31.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-clouddirectory-1.31.4.tar", last modified: Tue Jul 18 01:54:54 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-clouddirectory-1.31.5.tar", last modified: Wed Jul 19 02:43:37 2023, max compression
```

## Comparing `botocore-a-la-carte-clouddirectory-1.31.4.tar` & `botocore-a-la-carte-clouddirectory-1.31.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.956147 botocore-a-la-carte-clouddirectory-1.31.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:54:54.000000 botocore-a-la-carte-clouddirectory-1.31.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-18 01:54:54.956147 botocore-a-la-carte-clouddirectory-1.31.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.952146 botocore-a-la-carte-clouddirectory-1.31.4/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.952146 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.952146 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.952146 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   229185 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.956147 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   236443 2023-07-18 01:54:49.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:54.956147 botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-18 01:54:54.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-18 01:54:54.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:54:54.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:54:54.000000 botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:54:54.956147 botocore-a-la-carte-clouddirectory-1.31.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 01:54:54.000000 botocore-a-la-carte-clouddirectory-1.31.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:43:36.000000 botocore-a-la-carte-clouddirectory-1.31.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.003519 botocore-a-la-carte-clouddirectory-1.31.5/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.003519 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   229185 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   236443 2023-07-19 02:43:32.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 02:43:36.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-19 02:43:36.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:43:36.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:43:36.000000 botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:43:37.007519 botocore-a-la-carte-clouddirectory-1.31.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-19 02:43:36.000000 botocore-a-la-carte-clouddirectory-1.31.5/setup.py
```

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/LICENSE.txt` & `botocore-a-la-carte-clouddirectory-1.31.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/PKG-INFO` & `botocore-a-la-carte-clouddirectory-1.31.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-clouddirectory
-Version: 1.31.4
+Version: 1.31.5
 Summary: clouddirectory data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/paginators-1.json` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2016-05-10/service-2.json` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2016-05-10/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/endpoint-rule-set-1.json` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/paginators-1.json` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore/data/clouddirectory/2017-01-11/service-2.json` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore/data/clouddirectory/2017-01-11/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/PKG-INFO` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-clouddirectory
-Version: 1.31.4
+Version: 1.31.5
 Summary: clouddirectory data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/botocore_a_la_carte_clouddirectory.egg-info/SOURCES.txt` & `botocore-a-la-carte-clouddirectory-1.31.5/botocore_a_la_carte_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-clouddirectory-1.31.4/setup.py` & `botocore-a-la-carte-clouddirectory-1.31.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-clouddirectory',
-    version="1.31.4",
+    version="1.31.5",
     description='clouddirectory data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/clouddirectory/*/*.json'],
```

