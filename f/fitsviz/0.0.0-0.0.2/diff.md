# Comparing `tmp/fitsviz-0.0.0.tar.gz` & `tmp/fitsviz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsviz-0.0.0.tar", last modified: Tue Jul 18 20:36:53 2023, max compression
+gzip compressed data, was "fitsviz-0.0.2.tar", last modified: Tue Jul 18 21:55:15 2023, max compression
```

## Comparing `fitsviz-0.0.0.tar` & `fitsviz-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.444676 fitsviz-0.0.0/
--rw-r--r--   0 user      (1000) user      (1000)       51 2023-07-18 20:36:53.444676 fitsviz-0.0.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1888 2023-07-18 20:36:37.000000 fitsviz-0.0.0/README.md
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.443676 fitsviz-0.0.0/fitsviz/
--rw-r--r--   0 user      (1000) user      (1000)      203 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2829 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/__main__.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.443676 fitsviz-0.0.0/fitsviz/detection/
--rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/detection/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     8062 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/detection/ap_photometry.py
--rw-r--r--   0 user      (1000) user      (1000)     1485 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/detection/core.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.443676 fitsviz-0.0.0/fitsviz/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/tests/test_loading.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/tests/test_viz.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.444676 fitsviz-0.0.0/fitsviz/utils/
--rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/utils/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2392 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/utils/cutils.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.444676 fitsviz-0.0.0/fitsviz/viz/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/viz/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2315 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/viz/plot_bokeh.py
--rw-r--r--   0 user      (1000) user      (1000)     1226 2023-07-18 20:36:37.000000 fitsviz-0.0.0/fitsviz/viz/plot_matplotlib.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 20:36:53.443676 fitsviz-0.0.0/fitsviz.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)       51 2023-07-18 20:36:53.000000 fitsviz-0.0.0/fitsviz.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      492 2023-07-18 20:36:53.000000 fitsviz-0.0.0/fitsviz.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-18 20:36:53.000000 fitsviz-0.0.0/fitsviz.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-07-18 20:36:53.000000 fitsviz-0.0.0/fitsviz.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      484 2023-07-18 20:36:37.000000 fitsviz-0.0.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-18 20:36:53.444676 fitsviz-0.0.0/setup.cfg
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.998581 fitsviz-0.0.2/
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 21:55:15.998581 fitsviz-0.0.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1888 2023-07-18 21:54:05.000000 fitsviz-0.0.2/README.md
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.996581 fitsviz-0.0.2/fitsviz/
+-rw-r--r--   0 user      (1000) user      (1000)      203 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2829 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/__main__.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.997581 fitsviz-0.0.2/fitsviz/detection/
+-rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/detection/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     8062 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/detection/ap_photometry.py
+-rw-r--r--   0 user      (1000) user      (1000)     1485 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/detection/core.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.997581 fitsviz-0.0.2/fitsviz/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/tests/test_loading.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/tests/test_viz.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.998581 fitsviz-0.0.2/fitsviz/utils/
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/utils/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2392 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/utils/cutils.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.998581 fitsviz-0.0.2/fitsviz/viz/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/viz/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2315 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/viz/plot_bokeh.py
+-rw-r--r--   0 user      (1000) user      (1000)     1226 2023-07-18 21:54:05.000000 fitsviz-0.0.2/fitsviz/viz/plot_matplotlib.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 21:55:15.997581 fitsviz-0.0.2/fitsviz.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      522 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      153 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-07-18 21:55:15.000000 fitsviz-0.0.2/fitsviz.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      585 2023-07-18 21:54:05.000000 fitsviz-0.0.2/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-18 21:55:15.998581 fitsviz-0.0.2/setup.cfg
```

### Comparing `fitsviz-0.0.0/README.md` & `fitsviz-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.0/fitsviz/__main__.py` & `fitsviz-0.0.2/fitsviz/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.0/fitsviz/detection/ap_photometry.py` & `fitsviz-0.0.2/fitsviz/detection/ap_photometry.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.0/fitsviz/detection/core.py` & `fitsviz-0.0.2/fitsviz/detection/core.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.0/fitsviz/utils/cutils.py` & `fitsviz-0.0.2/fitsviz/utils/cutils.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.0/fitsviz/viz/plot_bokeh.py` & `fitsviz-0.0.2/fitsviz/viz/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.0/fitsviz/viz/plot_matplotlib.py` & `fitsviz-0.0.2/fitsviz/viz/plot_matplotlib.py`

 * *Files identical despite different names*

