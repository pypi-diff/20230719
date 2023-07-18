# Comparing `tmp/fitsviz-0.0.4.tar.gz` & `tmp/fitsviz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsviz-0.0.4.tar", last modified: Tue Jul 18 22:38:37 2023, max compression
+gzip compressed data, was "fitsviz-0.0.5.tar", last modified: Tue Jul 18 22:47:19 2023, max compression
```

## Comparing `fitsviz-0.0.4.tar` & `fitsviz-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.237568 fitsviz-0.0.4/
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 22:38:37.237568 fitsviz-0.0.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1888 2023-07-18 22:38:22.000000 fitsviz-0.0.4/README.md
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.235568 fitsviz-0.0.4/fitsviz/
--rw-r--r--   0 user      (1000) user      (1000)      203 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2829 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/__main__.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.236568 fitsviz-0.0.4/fitsviz/detection/
--rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/detection/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     8040 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/detection/ap_photometry.py
--rw-r--r--   0 user      (1000) user      (1000)     1485 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/detection/core.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.236568 fitsviz-0.0.4/fitsviz/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/tests/test_loading.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/tests/test_viz.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.237568 fitsviz-0.0.4/fitsviz/utils/
--rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/utils/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2392 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/utils/cutils.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.237568 fitsviz-0.0.4/fitsviz/viz/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/viz/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2315 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/viz/plot_bokeh.py
--rw-r--r--   0 user      (1000) user      (1000)     1226 2023-07-18 22:38:22.000000 fitsviz-0.0.4/fitsviz/viz/plot_matplotlib.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:38:37.235568 fitsviz-0.0.4/fitsviz.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 22:38:37.000000 fitsviz-0.0.4/fitsviz.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      522 2023-07-18 22:38:37.000000 fitsviz-0.0.4/fitsviz.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-18 22:38:37.000000 fitsviz-0.0.4/fitsviz.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 22:38:37.000000 fitsviz-0.0.4/fitsviz.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-07-18 22:38:37.000000 fitsviz-0.0.4/fitsviz.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      496 2023-07-18 22:38:22.000000 fitsviz-0.0.4/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-18 22:38:37.237568 fitsviz-0.0.4/setup.cfg
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.416146 fitsviz-0.0.5/
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 22:47:19.416146 fitsviz-0.0.5/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1888 2023-07-18 22:47:06.000000 fitsviz-0.0.5/README.md
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.415146 fitsviz-0.0.5/fitsviz/
+-rw-r--r--   0 user      (1000) user      (1000)      203 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2829 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/__main__.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.416146 fitsviz-0.0.5/fitsviz/detection/
+-rw-r--r--   0 user      (1000) user      (1000)       71 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/detection/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     8040 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/detection/ap_photometry.py
+-rw-r--r--   0 user      (1000) user      (1000)     1485 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/detection/core.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.416146 fitsviz-0.0.5/fitsviz/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/tests/test_loading.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/tests/test_viz.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.416146 fitsviz-0.0.5/fitsviz/utils/
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/utils/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2392 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/utils/cutils.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.416146 fitsviz-0.0.5/fitsviz/viz/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/viz/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2315 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/viz/plot_bokeh.py
+-rw-r--r--   0 user      (1000) user      (1000)     1226 2023-07-18 22:47:06.000000 fitsviz-0.0.5/fitsviz/viz/plot_matplotlib.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2023-07-18 22:47:19.415146 fitsviz-0.0.5/fitsviz.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-07-18 22:47:19.000000 fitsviz-0.0.5/fitsviz.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      522 2023-07-18 22:47:19.000000 fitsviz-0.0.5/fitsviz.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-18 22:47:19.000000 fitsviz-0.0.5/fitsviz.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       89 2023-07-18 22:47:19.000000 fitsviz-0.0.5/fitsviz.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-07-18 22:47:19.000000 fitsviz-0.0.5/fitsviz.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      520 2023-07-18 22:47:06.000000 fitsviz-0.0.5/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-18 22:47:19.417146 fitsviz-0.0.5/setup.cfg
```

### Comparing `fitsviz-0.0.4/PKG-INFO` & `fitsviz-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsviz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Autodetection of sources and visualization of FITS files
 Author-email: Phani Velicheti <phaniv@arizona.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 
 # fitsviz
```

### Comparing `fitsviz-0.0.4/README.md` & `fitsviz-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz/__main__.py` & `fitsviz-0.0.5/fitsviz/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz/detection/ap_photometry.py` & `fitsviz-0.0.5/fitsviz/detection/ap_photometry.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz/detection/core.py` & `fitsviz-0.0.5/fitsviz/detection/core.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz/utils/cutils.py` & `fitsviz-0.0.5/fitsviz/utils/cutils.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz/viz/plot_bokeh.py` & `fitsviz-0.0.5/fitsviz/viz/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz/viz/plot_matplotlib.py` & `fitsviz-0.0.5/fitsviz/viz/plot_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.4/fitsviz.egg-info/PKG-INFO` & `fitsviz-0.0.5/fitsviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsviz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Autodetection of sources and visualization of FITS files
 Author-email: Phani Velicheti <phaniv@arizona.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 
 # fitsviz
```

### Comparing `fitsviz-0.0.4/fitsviz.egg-info/SOURCES.txt` & `fitsviz-0.0.5/fitsviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

