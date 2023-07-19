# Comparing `tmp/botocore-a-la-carte-compute-optimizer-1.31.4.tar.gz` & `tmp/botocore-a-la-carte-compute-optimizer-1.31.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-compute-optimizer-1.31.4.tar", last modified: Tue Jul 18 01:55:02 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-compute-optimizer-1.31.5.tar", last modified: Wed Jul 19 02:43:44 2023, max compression
```

## Comparing `botocore-a-la-carte-compute-optimizer-1.31.4.tar` & `botocore-a-la-carte-compute-optimizer-1.31.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:55:02.000000 botocore-a-la-carte-compute-optimizer-1.31.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-18 01:54:50.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-18 01:54:50.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   225149 2023-07-18 01:54:50.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/botocore_a_la_carte_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 01:55:02.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-18 01:55:02.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore_a_la_carte_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:55:02.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore_a_la_carte_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:55:02.000000 botocore-a-la-carte-compute-optimizer-1.31.4/botocore_a_la_carte_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:55:02.544189 botocore-a-la-carte-compute-optimizer-1.31.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-18 01:55:02.000000 botocore-a-la-carte-compute-optimizer-1.31.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:44.291512 botocore-a-la-carte-compute-optimizer-1.31.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:43:44.000000 botocore-a-la-carte-compute-optimizer-1.31.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-19 02:43:44.291512 botocore-a-la-carte-compute-optimizer-1.31.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:44.287512 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:44.287512 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:44.287512 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:44.291512 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-19 02:43:32.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 02:43:32.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-19 02:43:32.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   225149 2023-07-19 02:43:32.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:43:44.291512 botocore-a-la-carte-compute-optimizer-1.31.5/botocore_a_la_carte_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-19 02:43:44.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-19 02:43:44.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore_a_la_carte_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:43:44.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore_a_la_carte_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:43:44.000000 botocore-a-la-carte-compute-optimizer-1.31.5/botocore_a_la_carte_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:43:44.291512 botocore-a-la-carte-compute-optimizer-1.31.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-19 02:43:44.000000 botocore-a-la-carte-compute-optimizer-1.31.5/setup.py
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/LICENSE.txt` & `botocore-a-la-carte-compute-optimizer-1.31.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/PKG-INFO` & `botocore-a-la-carte-compute-optimizer-1.31.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-compute-optimizer
-Version: 1.31.4
+Version: 1.31.5
 Summary: compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/paginators-1.json` & `botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/botocore/data/compute-optimizer/2019-11-01/service-2.json` & `botocore-a-la-carte-compute-optimizer-1.31.5/botocore/data/compute-optimizer/2019-11-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO` & `botocore-a-la-carte-compute-optimizer-1.31.5/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-compute-optimizer
-Version: 1.31.4
+Version: 1.31.5
 Summary: compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.31.4/setup.py` & `botocore-a-la-carte-compute-optimizer-1.31.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-compute-optimizer',
-    version="1.31.4",
+    version="1.31.5",
     description='compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/compute-optimizer/*/*.json'],
```

