# Comparing `tmp/dobot_utils-1.0.0.tar.gz` & `tmp/dobot_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dobot_utils-1.0.0.tar", last modified: Wed Jul 19 02:16:49 2023, max compression
+gzip compressed data, was "dobot_utils-1.0.1.tar", last modified: Wed Jul 19 02:20:32 2023, max compression
```

## Comparing `dobot_utils-1.0.0.tar` & `dobot_utils-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:16:49.799291 dobot_utils-1.0.0/
--rw-rw-r--   0 neo       (1000) neo       (1000)    35149 2023-07-11 06:33:31.000000 dobot_utils-1.0.0/LICENSE
--rw-rw-r--   0 neo       (1000) neo       (1000)      746 2023-07-19 02:16:49.799291 dobot_utils-1.0.0/PKG-INFO
--rw-rw-r--   0 neo       (1000) neo       (1000)      175 2023-07-19 02:13:40.000000 dobot_utils-1.0.0/README.md
--rw-r--r--   0 neo       (1000) neo       (1000)      679 2023-07-19 02:13:33.000000 dobot_utils-1.0.0/pyproject.toml
--rw-rw-r--   0 neo       (1000) neo       (1000)       38 2023-07-19 02:16:49.799291 dobot_utils-1.0.0/setup.cfg
--rw-r--r--   0 neo       (1000) neo       (1000)       68 2023-07-19 02:13:35.000000 dobot_utils-1.0.0/setup.py
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:16:49.799291 dobot_utils-1.0.0/src/
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:16:49.799291 dobot_utils-1.0.0/src/dobot_utils/
--rw-r--r--   0 neo       (1000) neo       (1000)        0 2023-07-06 15:15:38.000000 dobot_utils-1.0.0/src/dobot_utils/__init__.py
--rw-rw-r--   0 neo       (1000) neo       (1000)     9435 2023-07-19 02:13:31.000000 dobot_utils-1.0.0/src/dobot_utils/dobot_api.py
--rw-rw-r--   0 neo       (1000) neo       (1000)     4768 2023-07-11 22:32:05.000000 dobot_utils-1.0.0/src/dobot_utils/types.py
--rw-rw-r--   0 neo       (1000) neo       (1000)     1808 2023-07-19 02:13:44.000000 dobot_utils-1.0.0/src/dobot_utils/util.py
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:16:49.799291 dobot_utils-1.0.0/src/dobot_utils.egg-info/
--rw-rw-r--   0 neo       (1000) neo       (1000)      746 2023-07-19 02:16:49.000000 dobot_utils-1.0.0/src/dobot_utils.egg-info/PKG-INFO
--rw-rw-r--   0 neo       (1000) neo       (1000)      341 2023-07-19 02:16:49.000000 dobot_utils-1.0.0/src/dobot_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 neo       (1000) neo       (1000)        1 2023-07-19 02:16:49.000000 dobot_utils-1.0.0/src/dobot_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 neo       (1000) neo       (1000)       14 2023-07-19 02:16:49.000000 dobot_utils-1.0.0/src/dobot_utils.egg-info/requires.txt
--rw-rw-r--   0 neo       (1000) neo       (1000)       12 2023-07-19 02:16:49.000000 dobot_utils-1.0.0/src/dobot_utils.egg-info/top_level.txt
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/
+-rw-rw-r--   0 neo       (1000) neo       (1000)    35149 2023-07-11 06:33:31.000000 dobot_utils-1.0.1/LICENSE
+-rw-rw-r--   0 neo       (1000) neo       (1000)      770 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/PKG-INFO
+-rw-rw-r--   0 neo       (1000) neo       (1000)      175 2023-07-19 02:13:40.000000 dobot_utils-1.0.1/README.md
+-rw-r--r--   0 neo       (1000) neo       (1000)      703 2023-07-19 02:20:08.000000 dobot_utils-1.0.1/pyproject.toml
+-rw-rw-r--   0 neo       (1000) neo       (1000)       38 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)       68 2023-07-19 02:13:35.000000 dobot_utils-1.0.1/setup.py
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/src/
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/src/dobot_utils/
+-rw-r--r--   0 neo       (1000) neo       (1000)        0 2023-07-06 15:15:38.000000 dobot_utils-1.0.1/src/dobot_utils/__init__.py
+-rw-rw-r--   0 neo       (1000) neo       (1000)     9435 2023-07-19 02:13:31.000000 dobot_utils-1.0.1/src/dobot_utils/dobot_api.py
+-rw-rw-r--   0 neo       (1000) neo       (1000)     4768 2023-07-11 22:32:05.000000 dobot_utils-1.0.1/src/dobot_utils/types.py
+-rw-rw-r--   0 neo       (1000) neo       (1000)     1808 2023-07-19 02:13:44.000000 dobot_utils-1.0.1/src/dobot_utils/util.py
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/src/dobot_utils.egg-info/
+-rw-rw-r--   0 neo       (1000) neo       (1000)      770 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 neo       (1000) neo       (1000)      341 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 neo       (1000) neo       (1000)        1 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 neo       (1000) neo       (1000)       14 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/requires.txt
+-rw-rw-r--   0 neo       (1000) neo       (1000)       12 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/top_level.txt
```

### Comparing `dobot_utils-1.0.0/LICENSE` & `dobot_utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dobot_utils-1.0.0/PKG-INFO` & `dobot_utils-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dobot_utils
-Version: 1.0.0
-Summary: A better implementation of the Dobot API in Python
+Version: 1.0.1
+Summary: An ergonomic and type-hinted Python API for Dobot Products TCP-IP Protocol
 Author-email: Calastrophe <vmxoperation@proton.me>
 Project-URL: Homepage, https://github.com/Calastrophe/dobot_utils
 Project-URL: Bug Tracker, https://github.com/Calastrophe/dobot_utils/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `dobot_utils-1.0.0/pyproject.toml` & `dobot_utils-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dobot_utils"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Calastrophe", email = "vmxoperation@proton.me" }]
-description = "A better implementation of the Dobot API in Python"
+description = "An ergonomic and type-hinted Python API for Dobot Products TCP-IP Protocol"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ['numpy', 'StrEnum']
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `dobot_utils-1.0.0/src/dobot_utils/dobot_api.py` & `dobot_utils-1.0.1/src/dobot_utils/dobot_api.py`

 * *Files identical despite different names*

### Comparing `dobot_utils-1.0.0/src/dobot_utils/types.py` & `dobot_utils-1.0.1/src/dobot_utils/types.py`

 * *Files identical despite different names*

### Comparing `dobot_utils-1.0.0/src/dobot_utils/util.py` & `dobot_utils-1.0.1/src/dobot_utils/util.py`

 * *Files identical despite different names*

### Comparing `dobot_utils-1.0.0/src/dobot_utils.egg-info/PKG-INFO` & `dobot_utils-1.0.1/src/dobot_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dobot-utils
-Version: 1.0.0
-Summary: A better implementation of the Dobot API in Python
+Version: 1.0.1
+Summary: An ergonomic and type-hinted Python API for Dobot Products TCP-IP Protocol
 Author-email: Calastrophe <vmxoperation@proton.me>
 Project-URL: Homepage, https://github.com/Calastrophe/dobot_utils
 Project-URL: Bug Tracker, https://github.com/Calastrophe/dobot_utils/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

