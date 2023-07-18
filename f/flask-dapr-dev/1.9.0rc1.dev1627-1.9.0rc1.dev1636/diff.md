# Comparing `tmp/flask-dapr-dev-1.9.0rc1.dev1627.tar.gz` & `tmp/flask-dapr-dev-1.9.0rc1.dev1636.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-dapr-dev-1.9.0rc1.dev1627.tar", last modified: Fri Jul 14 18:52:14 2023, max compression
+gzip compressed data, was "dist/flask-dapr-dev-1.9.0rc1.dev1636.tar", last modified: Tue Jul 18 22:44:58 2023, max compression
```

## Comparing `flask-dapr-dev-1.9.0rc1.dev1627.tar` & `flask-dapr-dev-1.9.0rc1.dev1636.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-14 18:52:14.000000 flask-dapr-dev-1.9.0rc1.dev1627/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-14 18:51:50.000000 flask-dapr-dev-1.9.0rc1.dev1627/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 22:44:58.000000 flask-dapr-dev-1.9.0rc1.dev1636/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-18 22:44:37.000000 flask-dapr-dev-1.9.0rc1.dev1636/setup.py
```

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/LICENSE` & `flask-dapr-dev-1.9.0rc1.dev1636/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/PKG-INFO` & `flask-dapr-dev-1.9.0rc1.dev1636/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-dapr-dev
-Version: 1.9.0rc1.dev1627
+Version: 1.9.0rc1.dev1636
 Summary: The developmental release for Dapr Python SDK Flask.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/README.rst` & `flask-dapr-dev-1.9.0rc1.dev1636/README.rst`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/__init__.py` & `flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/actor.py` & `flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/actor.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/app.py` & `flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/app.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr/version.py` & `flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr/version.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/flask_dapr_dev.egg-info/PKG-INFO` & `flask-dapr-dev-1.9.0rc1.dev1636/flask_dapr_dev.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-dapr-dev
-Version: 1.9.0rc1.dev1627
+Version: 1.9.0rc1.dev1636
 Summary: The developmental release for Dapr Python SDK Flask.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/setup.cfg` & `flask-dapr-dev-1.9.0rc1.dev1636/setup.cfg`

 * *Files identical despite different names*

### Comparing `flask-dapr-dev-1.9.0rc1.dev1627/setup.py` & `flask-dapr-dev-1.9.0rc1.dev1636/setup.py`

 * *Files identical despite different names*

