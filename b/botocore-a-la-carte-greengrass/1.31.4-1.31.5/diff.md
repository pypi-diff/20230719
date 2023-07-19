# Comparing `tmp/botocore-a-la-carte-greengrass-1.31.4.tar.gz` & `tmp/botocore-a-la-carte-greengrass-1.31.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-greengrass-1.31.4.tar", last modified: Tue Jul 18 01:55:07 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-greengrass-1.31.5.tar", last modified: Wed Jul 19 02:43:49 2023, max compression
```

## Comparing `botocore-a-la-carte-greengrass-1.31.4.tar` & `botocore-a-la-carte-greengrass-1.31.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:07.688215 botocore-a-la-carte-greengrass-1.31.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:55:07.000000 botocore-a-la-carte-greengrass-1.31.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 01:55:07.688215 botocore-a-la-carte-greengrass-1.31.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:07.684215 botocore-a-la-carte-greengrass-1.31.4/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:07.684215 botocore-a-la-carte-greengrass-1.31.4/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:07.684215 botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:07.684215 botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-07-18 01:54:50.000000 botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-18 01:54:50.000000 botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   216808 2023-07-18 01:54:50.000000 botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:07.688215 botocore-a-la-carte-greengrass-1.31.4/botocore_a_la_carte_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 01:55:07.000000 botocore-a-la-carte-greengrass-1.31.4/botocore_a_la_carte_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-18 01:55:07.000000 botocore-a-la-carte-greengrass-1.31.4/botocore_a_la_carte_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:55:07.000000 botocore-a-la-carte-greengrass-1.31.4/botocore_a_la_carte_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:55:07.000000 botocore-a-la-carte-greengrass-1.31.4/botocore_a_la_carte_greengrass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:55:07.688215 botocore-a-la-carte-greengrass-1.31.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-18 01:55:07.000000 botocore-a-la-carte-greengrass-1.31.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:49.191522 botocore-a-la-carte-greengrass-1.31.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:43:49.000000 botocore-a-la-carte-greengrass-1.31.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-19 02:43:49.191522 botocore-a-la-carte-greengrass-1.31.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:49.187522 botocore-a-la-carte-greengrass-1.31.5/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:49.187522 botocore-a-la-carte-greengrass-1.31.5/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:49.187522 botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:49.191522 botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/
+-rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-07-19 02:43:32.000000 botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-19 02:43:32.000000 botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   216808 2023-07-19 02:43:32.000000 botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:49.191522 botocore-a-la-carte-greengrass-1.31.5/botocore_a_la_carte_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-19 02:43:49.000000 botocore-a-la-carte-greengrass-1.31.5/botocore_a_la_carte_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-19 02:43:49.000000 botocore-a-la-carte-greengrass-1.31.5/botocore_a_la_carte_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:43:49.000000 botocore-a-la-carte-greengrass-1.31.5/botocore_a_la_carte_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:43:49.000000 botocore-a-la-carte-greengrass-1.31.5/botocore_a_la_carte_greengrass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:43:49.191522 botocore-a-la-carte-greengrass-1.31.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-19 02:43:49.000000 botocore-a-la-carte-greengrass-1.31.5/setup.py
```

### Comparing `botocore-a-la-carte-greengrass-1.31.4/LICENSE.txt` & `botocore-a-la-carte-greengrass-1.31.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-greengrass-1.31.4/PKG-INFO` & `botocore-a-la-carte-greengrass-1.31.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-greengrass
-Version: 1.31.4
+Version: 1.31.5
 Summary: greengrass data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/endpoint-rule-set-1.json` & `botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/paginators-1.json` & `botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-greengrass-1.31.4/botocore/data/greengrass/2017-06-07/service-2.json` & `botocore-a-la-carte-greengrass-1.31.5/botocore/data/greengrass/2017-06-07/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-greengrass-1.31.4/botocore_a_la_carte_greengrass.egg-info/PKG-INFO` & `botocore-a-la-carte-greengrass-1.31.5/botocore_a_la_carte_greengrass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-greengrass
-Version: 1.31.4
+Version: 1.31.5
 Summary: greengrass data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-greengrass-1.31.4/setup.py` & `botocore-a-la-carte-greengrass-1.31.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-greengrass',
-    version="1.31.4",
+    version="1.31.5",
     description='greengrass data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/greengrass/*/*.json'],
```

