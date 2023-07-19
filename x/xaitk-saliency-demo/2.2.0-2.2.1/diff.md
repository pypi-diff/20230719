# Comparing `tmp/xaitk-saliency-demo-2.2.0.tar.gz` & `tmp/xaitk-saliency-demo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaitk-saliency-demo-2.2.0.tar", last modified: Wed Jul 12 15:21:24 2023, max compression
+gzip compressed data, was "xaitk-saliency-demo-2.2.1.tar", last modified: Wed Jul 19 00:21:10 2023, max compression
```

## Comparing `xaitk-saliency-demo-2.2.0.tar` & `xaitk-saliency-demo-2.2.1.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1504 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/LICENSE
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       44 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/MANIFEST.in
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1953 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/PKG-INFO
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1171 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/README.rst
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1282 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/setup.cfg
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       38 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/setup.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       49 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/__init__.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       50 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/__init__.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      197 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/__init__.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      498 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/__init__.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/__pycache__/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      707 2023-07-06 21:36:39.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)    10472 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1974 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/main.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     9702 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_models.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     5561 2023-07-07 00:51:07.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_xai.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     2443 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/options.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     5323 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_exec.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     4031 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_state.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1085 2023-07-07 00:51:07.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/jupyter.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      689 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/main.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       62 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/__init__.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     4178 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/main.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1092 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/options.py
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)    16390 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/ui_helper.py
-drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1953 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/PKG-INFO
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1079 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        1 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       65 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/entry_points.txt
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      330 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/requires.txt
--rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       20 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.256391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.256391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/
+-rw-r--r--   0 root         (0) root         (0)      498 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10472 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/main.py
+-rw-r--r--   0 root         (0) root         (0)     9702 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_models.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_xai.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/options.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_exec.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_state.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/main.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/options.py
+-rw-r--r--   0 root         (0) root         (0)    16375 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/ui_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.256391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/top_level.txt
```

### Comparing `xaitk-saliency-demo-2.2.0/LICENSE` & `xaitk-saliency-demo-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/setup.cfg` & `xaitk-saliency-demo-2.2.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xaitk-saliency-demo
-version = 2.2.0
+version = 2.2.1
 description = Web application demonstrating XAITK Saliency functionality
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -48,11 +48,14 @@
 	scikit-learn==1.3.0
 	scikit-image==0.21.0
 
 [options.entry_points]
 console_scripts = 
 	xaitk-saliency-demo = xaitk_saliency_demo:main
 
+[semantic_release]
+version_pattern = setup.cfg:version = (\d+\.\d+\.\d+)
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/main.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/main.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_models.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_models.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_xai.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_xai.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import numpy as np
 from scipy.special import softmax
 
 # pytorch
 import torch
 
 # xaitk-saliency
-from xaitk_saliency.impls.perturb_image.rise import RISEGrid
-from xaitk_saliency.impls.gen_detector_prop_sal.drise_scoring import DRISEScoring
+# from xaitk_saliency.impls.perturb_image.rise import RISEGrid
+# from xaitk_saliency.impls.gen_detector_prop_sal.drise_scoring import DRISEScoring
 
 from xaitk_saliency.impls.gen_image_similarity_blackbox_sal.sbsm import SBSMStack
 from xaitk_saliency.impls.gen_image_classifier_blackbox_sal.rise import RISEStack
 from xaitk_saliency.impls.gen_image_classifier_blackbox_sal.slidingwindow import (
     SlidingWindowStack,
 )
 from xaitk_saliency.impls.gen_object_detector_blackbox_sal.drise import DRISEStack
```

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/options.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/options.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_exec.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_exec.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_state.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_state.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/jupyter.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/jupyter.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     # Disable logging
     import logging
 
     engine_logger = logging.getLogger("xaitks_saliency_demo")
     engine_logger.setLevel(logging.ERROR)
 
-    # Initilize app
+    # Initialize app
     if new_server:
         # Try to use GPU by default
         update_ml_device(False)
 
         engine.initialize(server)
         ui.initialize(server)
```

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/main.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/main.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/main.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     @state.change("xai_viz_color_min", "xai_viz_color_max")
     def xai_viz_color_range_change(xai_viz_color_min, xai_viz_color_max, **kwargs):
         try:
             state.xai_viz_heatmap_color_range = [
                 float(xai_viz_color_min),
                 float(xai_viz_color_max),
             ]
-        except:
+        except Exception:
             pass
 
     # -----------------------------------------------------------------------------
     # UI
     # -----------------------------------------------------------------------------
 
     with SinglePageLayout(server) as layout:
```

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/options.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/options.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/ui_helper.py` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/ui_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
 def create_section_input():
     _card, _header, _content = create_card_container(
         classes="ma-4",
         style=("{ width: `${2 * 216 + 8}px`}",),
     )
     _content.style = "min-height: 224px;"
-    _file = ""
 
     with _header:
         _header.add_child("Data Selection")
         vuetify.VSpacer()
         create_btn_icon(
             "mdi-image-plus",
             small=True,
```

### Comparing `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/SOURCES.txt` & `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,12 +18,11 @@
 xaitk_saliency_demo/app/engine/ml_models.py
 xaitk_saliency_demo/app/engine/ml_xai.py
 xaitk_saliency_demo/app/engine/options.py
 xaitk_saliency_demo/app/engine/trame_exec.py
 xaitk_saliency_demo/app/engine/trame_state.py
 xaitk_saliency_demo/app/engine/assets/__init__.py
 xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
-xaitk_saliency_demo/app/engine/assets/__pycache__/__init__.cpython-39.pyc
 xaitk_saliency_demo/app/ui/__init__.py
 xaitk_saliency_demo/app/ui/main.py
 xaitk_saliency_demo/app/ui/options.py
 xaitk_saliency_demo/app/ui/ui_helper.py
```

