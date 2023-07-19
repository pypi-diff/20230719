# Comparing `tmp/numan-1.0.9.tar.gz` & `tmp/numan-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numan-1.0.9.tar", last modified: Thu Jul  6 19:22:24 2023, max compression
+gzip compressed data, was "numan-1.1.0.tar", last modified: Wed Jul 19 06:07:50 2023, max compression
```

## Comparing `numan-1.0.9.tar` & `numan-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.247105 numan-1.0.9/
--rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.9/LICENSE.md
--rw-rw-rw-   0        0        0     2181 2023-07-06 19:22:24.247105 numan-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.9/README.md
--rw-rw-rw-   0        0        0     1314 2023-07-06 19:21:25.000000 numan-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 19:22:24.248091 numan-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.136089 numan-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.212089 numan-1.0.9/src/numan/
--rw-rw-rw-   0        0        0      224 2023-07-06 19:21:33.000000 numan-1.0.9/src/numan/__init__.py
--rw-rw-rw-   0        0        0    45479 2023-07-05 18:23:16.000000 numan-1.0.9/src/numan/analysis.py
--rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.9/src/numan/notifications.py
--rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.9/src/numan/plots.py
--rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.9/src/numan/project.py
--rw-rw-rw-   0        0        0    27665 2023-07-06 19:14:10.000000 numan-1.0.9/src/numan/report.py
--rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.9/src/numan/runner.py
--rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.0.9/src/numan/utils.py
--rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.9/src/numan/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.236091 numan-1.0.9/src/numan.egg-info/
--rw-rw-rw-   0        0        0     2181 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.245126 numan-1.0.9/tests/
--rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.9/tests/test_plots.py
--rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.0.9/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:07:50.280646 numan-1.1.0/
+-rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     2181 2023-07-19 06:07:50.279645 numan-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1314 2023-07-19 06:06:26.000000 numan-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 06:07:50.280646 numan-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:07:50.219644 numan-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 06:07:50.245645 numan-1.1.0/src/numan/
+-rw-rw-rw-   0        0        0      224 2023-07-19 06:04:49.000000 numan-1.1.0/src/numan/__init__.py
+-rw-rw-rw-   0        0        0    50772 2023-07-19 04:49:30.000000 numan-1.1.0/src/numan/analysis.py
+-rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.1.0/src/numan/notifications.py
+-rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.1.0/src/numan/plots.py
+-rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.1.0/src/numan/project.py
+-rw-rw-rw-   0        0        0    27658 2023-07-18 03:23:08.000000 numan-1.1.0/src/numan/report.py
+-rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.1.0/src/numan/runner.py
+-rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.1.0/src/numan/utils.py
+-rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.1.0/src/numan/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:07:50.274646 numan-1.1.0/src/numan.egg-info/
+-rw-rw-rw-   0        0        0     2181 2023-07-19 06:07:50.000000 numan-1.1.0/src/numan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-07-19 06:07:50.000000 numan-1.1.0/src/numan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 06:07:50.000000 numan-1.1.0/src/numan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-19 06:07:50.000000 numan-1.1.0/src/numan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 06:07:50.000000 numan-1.1.0/src/numan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 06:07:50.277646 numan-1.1.0/tests/
+-rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.1.0/tests/test_plots.py
+-rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.1.0/tests/test_utils.py
```

### Comparing `numan-1.0.9/LICENSE.md` & `numan-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/PKG-INFO` & `numan-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.9
+Version: 1.1.0
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.9/README.md` & `numan-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/pyproject.toml` & `numan-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numan"
-version = "1.0.9"
+version = "1.1.0"
 description='numerosity analysis package'
 readme = "README.md"
 authors = [{ name = "Anna Nadtochiy", email = "nadtochi@usc.edu" }]
 license = { file = "LICENSE" }
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
@@ -34,15 +34,15 @@
 [project.optional-dependencies]
 dev = ["bumpver"]
 
 [project.urls] # Read The Docs will also go in here
 Homepage = "https://github.com/LemonJust/numan"
 
 [tool.bumpver]
-current_version = "1.0.9"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `numan-1.0.9/src/numan/analysis.py` & `numan-1.1.0/src/numan/analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,121 @@
 
 import matplotlib.pyplot as plt
 import warnings
 from tqdm import tqdm
 import pandas as pd
 import PyPDF2
 
+from scipy.spatial import cKDTree
+import copy
+
 # try:
 import ants
 # except ImportError:
 #     print("ants not installed, some registration will not work")
 
 from .utils import *
 
+def nearest_neighbour_assignmnet(centroids1, centroids2, depth=None, radius = None):
+    """
+    Find nearest k-dimensional point pairs between centroids1 and centroids1 and returns the matching and the distance.
+    depth is the cutoff distance for the nearest neighbor search.
+
+    Args:
+        centroids1: array with first pointcloud with shape (n, k)
+        centroids2: array with second pointcloud with shape (m, k)
+        depth: maximum number of nearest neighbors to search for
+        radius: maximum euclidean distance between points in a pair
+
+    Returns:
+        distances: the distances between the nearest neighbors in centroids1 and centroids2. shape (len(centroids2), depth)
+        indices_1: the indices of the nearest neighbors in centroids1 for each point in centroids2. shape (len(centroids2), depth)
+        indices_2: the indices of the points in centroids2. shape (len(centroids2),)
+    """
+
+    if depth is None:
+        # set depth to be the minimum of the number of points or 100 ( arbitrary)
+        depth = min(max(len(centroids1), len(centroids2)), 100)
+
+    indices_2 = np.arange(len(centroids2))
+    distances, indices_1 = cKDTree(centroids1).query(centroids2, k = depth, distance_upper_bound=radius)
+
+    return distances, indices_1, indices_2
+
+def unique_nearest_neighbour_assignment(centroids1, centroids2, depth=None, radius = None, return_bothways = False):
+    """
+    Find nearest k-dimensional point pairs between centroids1 and centroids1 and returns the matching and the distance.
+    Returns the assignmnets and distances in both directions if return_bothways is True.
+
+    Args:
+        centroids1: array with first pointcloud with shape (n, k)
+        centroids2: array with second pointcloud with shape (m, k)
+        depth: maximum number of nearest neighbors to search for
+        radius: maximum euclidean distance between points in a pair
+        return_bothways: if True, returns the assignments and distances in both directions
+
+    Returns:
+        distances_2_to_1: the distances between the nearest neighbors in centroids1 and centroids2. 
+            shape (len(centroids2),)
+        assignment_2_to_1: the indices of the nearest neighbors in centroids1 for each point in centroids2. 
+            shape (len(centroids2),)
+        indices_2: the indices of the points in centroids2. 
+            shape (len(centroids2),)
+     
+        distances_1_to_2: the distances between the nearest neighbors in centroids2 and centroids1. 
+            shape (len(centroids1),)
+        assignment_1_to_2: the indices of the nearest neighbors in centroids2 for each point in centroids1. 
+            shape (len(centroids1),)
+        indices_1: the indices of the points in centroids1. 
+            shape (len(centroids1),)
+    """
+    if depth is None:
+        # set depth to be the minimum of the number of points or 100 ( arbitrary)
+        depth = min(max(len(centroids1), len(centroids2)), 100)
+    
+    assert depth > 1, "depth must be larger than 1, otherwise there are no duplicates"
+
+    distances, indices_1, indices_2 = nearest_neighbour_assignmnet(centroids1, centroids2, 
+                                                                   depth = depth, radius = radius)
+
+    # resolve non-unique assignments
+    # assert that indices_2 are simply the indices of the points in centroids2 (0, 1, 2, 3, ...)
+    # since this is importnat for the next step
+    assert (indices_2 == np.arange(len(centroids2))).all()
+
+    assignment_2_to_1 = np.zeros(len(centroids2), dtype=int) - 1 # for each point in centroids2, the index of the point in centroids1 
+    assignment_1_to_2 = np.zeros(len(centroids1), dtype=int) - 1 # for each point in centroids1, the index of the point in centroids2
+    distances_2_to_1 = np.full(len(centroids2), np.inf)
+    if return_bothways:
+        distances_1_to_2 = np.full(len(centroids1), np.inf)
+
+
+    # for each order of the nearest neighbor search, find the duplicates
+    for d in range(depth):
+        # sort the distances and corresponding order of indices in centroids2
+        sorted_indices_2 = np.argsort(distances[:, d])
+        for idx2 in sorted_indices_2:
+            if distances[idx2, d] < radius:
+                # the index of the point in centroids1 that is closest to the point in centroids2 with index idx2 for the d-th order of the nearest neighbor search
+                pair_idx1 = indices_1[idx2, d]
+                # if both points are not yet assigned, assign them to each other
+                if assignment_1_to_2[pair_idx1] == -1 and assignment_2_to_1[idx2] == -1:
+
+                    assignment_2_to_1[idx2] = pair_idx1
+                    assignment_1_to_2[pair_idx1] = idx2
+
+                    distances_2_to_1[idx2] = distances[idx2, d]
+                    if return_bothways:
+                        distances_1_to_2[pair_idx1] = distances[idx2, d]
+
+    if return_bothways:
+        indices_1 = np.arange(len(centroids1))
+        return distances_2_to_1, assignment_2_to_1, indices_2, distances_1_to_2, assignment_1_to_2, indices_1
+    else:
+        return distances_2_to_1, assignment_2_to_1, indices_2
 
 class Spot:
     """
     This is a class for a n individual segmented spot.
     """
 
     def __init__(self, center, diameter, resolution=None, units='pix'):
@@ -548,15 +648,15 @@
         self.signals = Signals.from_spots(self.spots, volumes=volumes, experiment=experiment,
                                           batch_size=batch_size, movie=movie, traces_type=traces_type)
 
     def get_group_mask(self, group, mask_shape, diameter=None, units='pix'):
         """
         Create a 3D volume that only shows the spots that belong to the particular group
         group : list[bool], the length of spots
-        mask_shape : the shape of the 3D volume of the mask
+        mask_shape : the shape of the 3D volume of the mask (the whole image shape)
         diameter : list or numpy array or int, diameter in zyx order. If int, then it is a sphere.
                     If not None, diameter will be used to create a mask.
                     If None, then spots diameter will be used and units will be ignored.
         units: what units is the diameter in : 'pix' or 'phs'
         """
         mask = np.zeros(mask_shape)
         for ispot in tqdm(np.where(group)[0]):
```

### Comparing `numan-1.0.9/src/numan/notifications.py` & `numan-1.1.0/src/numan/notifications.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/src/numan/plots.py` & `numan-1.1.0/src/numan/plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/src/numan/project.py` & `numan-1.1.0/src/numan/project.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/src/numan/report.py` & `numan-1.1.0/src/numan/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import matplotlib.pyplot as plt
 import warnings
 from tqdm import tqdm
 import pandas as pd
 
 import PyPDF2
-from PyPDF2 import PdfFileReader
+from PyPDF2 import PdfReader
 from reportlab.pdfgen import canvas
 from reportlab.lib.pagesizes import letter
 from reportlab.lib.colors import white, black
 
 from pathlib import Path
 
 from .plots import *
@@ -495,16 +495,16 @@
         return group_filenames, new_groups, spot_tags
 
     @staticmethod
     def get_checked_boxes(filename):
         """get checked boxes from pdf"""
 
         f = open(filename, "rb")
-        group_pdf = PyPDF2.PdfFileReader(f)
-        fields = group_pdf.getFields()
+        group_pdf = PyPDF2.PdfReader(f)
+        fields = group_pdf.get_fields()
         spots_in_group = np.array([spot for spot in fields if
                                    fields[spot]['/V'] == '/Yes']).astype(int)
         f.close()
         return spots_in_group
 
     def add_groups_from_pdf(self, rewrite=False):
         spots = Spots.from_json(f"spots/signals/spots_{self.spot_tags[0]}.json")
```

### Comparing `numan-1.0.9/src/numan/runner.py` & `numan-1.1.0/src/numan/runner.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/src/numan/utils.py` & `numan-1.1.0/src/numan/utils.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/src/numan/visualization.py` & `numan-1.1.0/src/numan/visualization.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/src/numan.egg-info/PKG-INFO` & `numan-1.1.0/src/numan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.9
+Version: 1.1.0
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.9/tests/test_plots.py` & `numan-1.1.0/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.9/tests/test_utils.py` & `numan-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

