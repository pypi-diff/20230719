# Comparing `tmp/iimcsim-0.1.1.tar.gz` & `tmp/iimcsim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.1.1.tar", last modified: Tue Jul 18 20:09:29 2023, max compression
+gzip compressed data, was "iimcsim-0.1.2.tar", last modified: Wed Jul 19 08:52:48 2023, max compression
```

## Comparing `iimcsim-0.1.1.tar` & `iimcsim-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.478040 iimcsim-0.1.1/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5197 2023-07-18 20:09:29.479037 iimcsim-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4527 2023-07-18 20:09:11.000000 iimcsim-0.1.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      747 2023-07-18 20:09:29.481032 iimcsim-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.412217 iimcsim-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.449118 iimcsim-0.1.1/src/iimcsim/
--rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.1.1/src/iimcsim/MC.py
--rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.1.1/src/iimcsim/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.1.1/src/iimcsim/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.1.1/src/iimcsim/data_gen.py
--rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.1.1/src/iimcsim/data_gen_run.py
--rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.1.1/src/iimcsim/eda.py
--rw-rw-rw-   0        0        0     2698 2023-07-18 17:05:44.000000 iimcsim-0.1.1/src/iimcsim/shape_ext.py
--rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.1.1/src/iimcsim/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.470062 iimcsim-0.1.1/src/iimcsim.egg-info/
--rw-rw-rw-   0        0        0     5197 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.475048 iimcsim-0.1.1/tests/
--rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.1.1/tests/test_mc.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:52:48.662585 iimcsim-0.1.2/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5197 2023-07-19 08:52:48.662585 iimcsim-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4527 2023-07-18 20:09:11.000000 iimcsim-0.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      747 2023-07-19 08:52:48.664579 iimcsim-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 08:52:48.604394 iimcsim-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 08:52:48.630737 iimcsim-0.1.2/src/iimcsim/
+-rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.1.2/src/iimcsim/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.1.2/src/iimcsim/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.1.2/src/iimcsim/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.1.2/src/iimcsim/data_gen.py
+-rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.1.2/src/iimcsim/data_gen_run.py
+-rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.1.2/src/iimcsim/eda.py
+-rw-rw-rw-   0        0        0     2698 2023-07-18 17:05:44.000000 iimcsim-0.1.2/src/iimcsim/shape_ext.py
+-rw-rw-rw-   0        0        0    17014 2023-07-19 08:50:17.000000 iimcsim-0.1.2/src/iimcsim/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:52:48.657638 iimcsim-0.1.2/src/iimcsim.egg-info/
+-rw-rw-rw-   0        0        0     5197 2023-07-19 08:52:48.000000 iimcsim-0.1.2/src/iimcsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-07-19 08:52:48.000000 iimcsim-0.1.2/src/iimcsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:52:48.000000 iimcsim-0.1.2/src/iimcsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 08:52:48.000000 iimcsim-0.1.2/src/iimcsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 08:52:48.660630 iimcsim-0.1.2/tests/
+-rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.1.2/tests/test_mc.py
```

### Comparing `iimcsim-0.1.1/PKG-INFO` & `iimcsim-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.1.1 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.1.2 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.1.1/README.md` & `iimcsim-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/setup.cfg` & `iimcsim-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 0d0a 7665 7273   = iimcsim..vers
-00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
+00000020: 696f 6e20 3d20 302e 312e 320d 0a61 7574  ion = 0.1.2..aut
 00000030: 686f 7220 3d20 4a69 6761 7220 4268 616e  hor = Jigar Bhan
 00000040: 6465 7269 0d0a 6175 7468 6f72 5f65 6d61  deri..author_ema
 00000050: 696c 203d 206a 6967 6172 6268 616e 6465  il = jigarbhande
 00000060: 7269 4067 6d61 696c 2e63 6f6d 0d0a 6465  ri@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 4d6f 6e74 652d  ckage for Monte-
 00000090: 4361 726c 6f20 7369 6d75 6c61 7469 6f6e  Carlo simulation
```

### Comparing `iimcsim-0.1.1/src/iimcsim/MC.py` & `iimcsim-0.1.2/src/iimcsim/MC.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/src/iimcsim/MonteCarlo.py` & `iimcsim-0.1.2/src/iimcsim/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/src/iimcsim/data_gen.py` & `iimcsim-0.1.2/src/iimcsim/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/src/iimcsim/data_gen_run.py` & `iimcsim-0.1.2/src/iimcsim/data_gen_run.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/src/iimcsim/eda.py` & `iimcsim-0.1.2/src/iimcsim/eda.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/src/iimcsim/shape_ext.py` & `iimcsim-0.1.2/src/iimcsim/shape_ext.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.1/src/iimcsim/tools.py` & `iimcsim-0.1.2/src/iimcsim/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,21 +417,16 @@
         cm = np.around(cm, decimals=2)
         cm_display = metrics.ConfusionMatrixDisplay(confusion_matrix = cm)
         #cm_display.plot()
         fig, ax = plt.subplots(figsize=(13,10))
         cm_display.plot(ax=ax)
         #plt.savefig('recall_confusion_matrix.png')
         plt.show()
-import numpy as np
 
-def remove_nonzero_neighbors(arr):
-    # Find the indices of the smallest elements in the array
-    smallest_indices = np.where(arr == np.min(arr))[0]
 
-    # Remove the indices of smallest elements whose neighbors are non-zero
-    modified_indices = []
-    for i in smallest_indices:
-        if i > 0 and i < len(arr) - 1:
-            if arr[i-1] == 0 and arr[i+1] == 0:
-                modified_indices.append(i)
-
-    return modified_indices
+def find_baseline_spikes(arr, A):
+    indices = []
+    n = len(arr)
+    for i in range(1, n - 1):
+        if arr[i] == A and arr[i - 1] == 0 and arr[i + 1] == 0:
+            indices.append(i)
+    return indices
```

### Comparing `iimcsim-0.1.1/src/iimcsim.egg-info/PKG-INFO` & `iimcsim-0.1.2/src/iimcsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.1.1 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.1.2 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.1.1/tests/test_mc.py` & `iimcsim-0.1.2/tests/test_mc.py`

 * *Files identical despite different names*

