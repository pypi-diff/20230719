# Comparing `tmp/mcemtools-0.7.0.tar.gz` & `tmp/mcemtools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.7.0.tar", last modified: Sat Jul 15 12:00:28 2023, max compression
+gzip compressed data, was "mcemtools-0.8.0.tar", last modified: Wed Jul 19 12:55:35 2023, max compression
```

## Comparing `mcemtools-0.7.0.tar` & `mcemtools-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-15 12:00:16.000000 mcemtools-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-15 12:00:16.000000 mcemtools-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-15 12:00:16.000000 mcemtools-0.7.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-15 12:00:16.000000 mcemtools-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-15 12:00:16.000000 mcemtools-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-15 12:00:28.195562 mcemtools-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-15 12:00:16.000000 mcemtools-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.191562 mcemtools-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 12:00:16.000000 mcemtools-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-15 12:00:28.195562 mcemtools-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-15 12:00:16.000000 mcemtools-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-19 12:55:24.000000 mcemtools-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-19 12:55:24.000000 mcemtools-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-19 12:55:24.000000 mcemtools-0.8.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-19 12:55:24.000000 mcemtools-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-19 12:55:24.000000 mcemtools-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-19 12:55:35.405779 mcemtools-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-19 12:55:24.000000 mcemtools-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 12:55:24.000000 mcemtools-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-19 12:55:35.405779 mcemtools-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-19 12:55:24.000000 mcemtools-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_transforms.py
```

### Comparing `mcemtools-0.7.0/CONTRIBUTING.rst` & `mcemtools-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/HISTORY.rst` & `mcemtools-0.8.0/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -31,8 +31,14 @@
 0.6.0 (2023-07-14)
 ------------------
 * More tests are added
 * Names are consistant accross the package.
 
 0.7.0 (2023-07-15)
 ------------------
-* markimage bug is fixed
+* markimage bug is fixed
+
+0.8.0 (2023-07-19)
+------------------
+* markimage bug is fixed really as US version of centre is center.
+* napari based GUI is added to mcemtools.
+* bianary files can be read too.
```

### Comparing `mcemtools-0.7.0/LICENSE` & `mcemtools-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/PKG-INFO` & `mcemtools-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.7.0
+Version: 0.8.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -98,7 +98,13 @@
 ------------------
 * More tests are added
 * Names are consistant accross the package.
 
 0.7.0 (2023-07-15)
 ------------------
 * markimage bug is fixed
+
+0.8.0 (2023-07-19)
+------------------
+* markimage bug is fixed really as US version of centre is center.
+* napari based GUI is added to mcemtools.
+* bianary files can be read too.
```

### Comparing `mcemtools-0.7.0/README.rst` & `mcemtools-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/docs/Makefile` & `mcemtools-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/docs/conf.py` & `mcemtools-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/docs/installation.rst` & `mcemtools-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/docs/make.bat` & `mcemtools-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/mcemtools/__init__.py` & `mcemtools-0.8.0/mcemtools/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
 
 from .transforms import get_polar_coords, polar2image, image2polar, bin_4D
 from .transforms import normalize_4D
 
-from .mcemtools import pltfig_to_numpy, locate_atoms, numbers_as_images
+from .mcemtools import pltfig_to_numpy, locate_atoms, numbers_as_images
+from .mcemtools import open_muSTEM_binary, viewer_4D
```

### Comparing `mcemtools-0.7.0/mcemtools/analysis.py` & `mcemtools-0.8.0/mcemtools/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
     return CoMx, CoMy
 
 def cross_correlation_4D(data4D_a, data4D_b, mask4D = None):
     
     assert data4D_a.shape == data4D_b.shape, \
         'data4D_a should have same shape as data4D_b'
     if mask4D is not None:
-        assert mask4D.shape == data4D.shape,\
-            'mask4D should have the same shape as data4D'
+        assert mask4D.shape == data4D_a.shape,\
+            'mask4D should have the same shape as data4D_a'
 
     data4D_a = normalize_4D(data4D_a.copy(), mask4D)
     data4D_b = normalize_4D(data4D_b.copy(), mask4D)
     corr_mat  = (data4D_a * data4D_b).sum(3).sum(2)
     
     if mask4D is not None:
         mask_STEM = mask4D.sum(3).sum(2)
```

### Comparing `mcemtools-0.7.0/mcemtools/masking.py` & `mcemtools-0.8.0/mcemtools/masking.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         mask *= in_radius <= dist_from_centre
 
     return mask.astype('uint8') 
 
 class image_by_windows:
     def __init__(self, 
                  img_shape: tuple[int, int], 
-                 win_shape: tuple[int, int] = (2, 2),
+                 win_shape: tuple[int, int],
                  skip: tuple[int, int] = (1, 1)):
         """image by windows
         
             I am using OOP here because the user pretty much always wants to
             transform results back to the original shape. It is different
             from typical transforms, where the processing ends at the other
             space.
@@ -250,15 +250,15 @@
         self.fig.canvas.draw_idle()
 
     def update2(self, val):
         if(self.mark_shape == 'circle'):
             r = self.slider_r.val
             cx = self.slider_cx.val
             cy  = self.slider_cy.val
-            self.markshape.set_centre((cy, cx))
+            self.markshape.set_center((cy, cx))
             self.markshape.set_radius(r)
             
         if(self.mark_shape == 'rectangle'):
             self.slider_top_left_r.val
             self.slider_top_left_c.val
             self.slider_bot_right_r.val
             self.slider_s_bot_right_c.val
```

### Comparing `mcemtools-0.7.0/mcemtools/tensor_svd.py` & `mcemtools-0.8.0/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/mcemtools/transforms.py` & `mcemtools-0.8.0/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.8.0/mcemtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.7.0
+Version: 0.8.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -98,7 +98,13 @@
 ------------------
 * More tests are added
 * Names are consistant accross the package.
 
 0.7.0 (2023-07-15)
 ------------------
 * markimage bug is fixed
+
+0.8.0 (2023-07-19)
+------------------
+* markimage bug is fixed really as US version of centre is center.
+* napari based GUI is added to mcemtools.
+* bianary files can be read too.
```

### Comparing `mcemtools-0.7.0/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.8.0/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/setup.py` & `mcemtools-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.7.0/tests/test_analysis.py` & `mcemtools-0.8.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/tests/test_masking.py` & `mcemtools-0.8.0/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/tests/test_mcemtools.py` & `mcemtools-0.8.0/tests/test_mcemtools.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,11 +32,16 @@
     
 def test_pltfig_to_numpy():
     fig, ax = plt.subplots(111)
     ax[0].imshow(np.random.rand(100, 100))
     np_data = mcemtools.pltfig_to_numpy(fig)
     print(np_data.shape)
 
+def test_viewer_4D():
+    data4D = np.random.rand(32, 16, 24, 16)
+    mcemtools.viewer_4D(data4D)
+
 if __name__ == '__main__':
     test_numbers_as_images()
     test_locate_atoms()
-    test_pltfig_to_numpy()
+    test_pltfig_to_numpy()
+    test_viewer_4D()
```

### Comparing `mcemtools-0.7.0/tests/test_tensor_svd.py` & `mcemtools-0.8.0/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.7.0/tests/test_transforms.py` & `mcemtools-0.8.0/tests/test_transforms.py`

 * *Files identical despite different names*

