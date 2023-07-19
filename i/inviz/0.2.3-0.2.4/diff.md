# Comparing `tmp/inviz-0.2.3.tar.gz` & `tmp/inviz-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.3.tar", last modified: Thu Jul 13 22:24:17 2023, max compression
+gzip compressed data, was "inviz-0.2.4.tar", last modified: Wed Jul 19 02:04:55 2023, max compression
```

## Comparing `inviz-0.2.3.tar` & `inviz-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-13 22:24:17.169098 inviz-0.2.3/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.3/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.3/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-13 22:24:17.169098 inviz-0.2.3/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.3/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-13 22:24:17.159098 inviz-0.2.3/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-13 22:24:17.169098 inviz-0.2.3/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      103 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10766 2023-07-13 22:19:19.000000 inviz-0.2.3/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-13 22:24:17.169098 inviz-0.2.3/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1139 2023-07-13 22:23:34.000000 inviz-0.2.3/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-19 02:04:55.539195 inviz-0.2.4/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.4/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.4/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-19 02:04:55.539195 inviz-0.2.4/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.4/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-19 02:04:55.539195 inviz-0.2.4/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-19 02:04:55.539195 inviz-0.2.4/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      103 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10791 2023-07-19 02:02:33.000000 inviz-0.2.4/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-19 02:04:55.539195 inviz-0.2.4/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1139 2023-07-19 02:02:33.000000 inviz-0.2.4/setup.py
```

### Comparing `inviz-0.2.3/LICENSE` & `inviz-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.3/PKG-INFO` & `inviz-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.3
+Version: 0.2.4
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.3/README.md` & `inviz-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.2.3/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.4/inviz/inviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.3
+Version: 0.2.4
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.3/inviz/inviz.py` & `inviz-0.2.4/inviz/inviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import holoviews as hv
 from holoviews import dim, opts, streams
 import pandas as pd
 import numpy as np
 import panel as pn
 import spatialpandas
 from bokeh.models import HoverTool
-from typing import Callable
+from typing import List, Callable, Union
 
 hv.extension('bokeh')
 pn.extension()
 
 
 class Observable:
     """
@@ -41,20 +41,20 @@
 
     plot_opts: holoviews Options object
         customization options for the observable plot. see Holoviews documentation
     """
     
     def __init__(
         self, 
-        name: str | list[str] = None, 
-        parameters: dict | list[dict] = None, 
+        name: Union[str, List[str]] = None, 
+        parameters: Union[dict, List[dict]] = None, 
         myfunc: Callable = None,
         myfunc_args: tuple = None, 
-        plot_type: str | list[str] = None,
-        plot_opts: type[opts] | list[type[opts]] = None,
+        plot_type: Union[str, List[str]] = None,
+        plot_opts: Union[opts, List[opts]] = None,
         latex_labels: dict = None
     ):
         if isinstance(name, str):
             self.name = [name]
         else:
             self.name = name
         if isinstance(parameters, dict):
```

### Comparing `inviz-0.2.3/setup.py` & `inviz-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.3",
+    version = "0.2.4",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
```

