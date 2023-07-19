# Comparing `tmp/periodicity_detection-0.1.0rc1.tar.gz` & `tmp/periodicity_detection-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/periodicity_detection-0.1.0rc1.tar", last modified: Wed Jul 19 11:22:26 2023, max compression
+gzip compressed data, was "dist/periodicity_detection-0.1.0rc2.tar", last modified: Wed Jul 19 11:49:34 2023, max compression
```

## Comparing `periodicity_detection-0.1.0rc1.tar` & `periodicity_detection-0.1.0rc2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/autoperiod.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/find_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/findfrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/number_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/periodicity_detection/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:22:26.000000 periodicity_detection-0.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-19 11:21:21.000000 periodicity_detection-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/autoperiod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/find_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/findfrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/number_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/periodicity_detection/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:49:34.000000 periodicity_detection-0.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-19 11:49:05.000000 periodicity_detection-0.1.0rc2/setup.py
```

### Comparing `periodicity_detection-0.1.0rc1/LICENSE` & `periodicity_detection-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/PKG-INFO` & `periodicity_detection-0.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodicity_detection
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Detect the dominant period in univariate, equidistant time series data.
 Home-page: https://github.com/CodeLionX/periodicity_detection
 Author: Sebastian Schmidl
 Author-email: sebastian.schmidl@hpi.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `periodicity_detection-0.1.0rc1/README.md` & `periodicity_detection-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection/__init__.py` & `periodicity_detection-0.1.0rc2/periodicity_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection/__main__.py` & `periodicity_detection-0.1.0rc2/periodicity_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection/autoperiod.py` & `periodicity_detection-0.1.0rc2/periodicity_detection/autoperiod.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection/find_length.py` & `periodicity_detection-0.1.0rc2/periodicity_detection/find_length.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection/findfrequency.py` & `periodicity_detection-0.1.0rc2/periodicity_detection/findfrequency.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection/number_peaks.py` & `periodicity_detection-0.1.0rc2/periodicity_detection/number_peaks.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/PKG-INFO` & `periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodicity-detection
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Detect the dominant period in univariate, equidistant time series data.
 Home-page: https://github.com/CodeLionX/periodicity_detection
 Author: Sebastian Schmidl
 Author-email: sebastian.schmidl@hpi.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `periodicity_detection-0.1.0rc1/periodicity_detection.egg-info/SOURCES.txt` & `periodicity_detection-0.1.0rc2/periodicity_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/pyproject.toml` & `periodicity_detection-0.1.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.0rc1/setup.py` & `periodicity_detection-0.1.0rc2/setup.py`

 * *Files identical despite different names*

