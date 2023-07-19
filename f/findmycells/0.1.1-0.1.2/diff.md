# Comparing `tmp/findmycells-0.1.1.tar.gz` & `tmp/findmycells-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmycells-0.1.1.tar", last modified: Tue Feb 21 15:15:57 2023, max compression
+gzip compressed data, was "findmycells-0.1.2.tar", last modified: Tue Feb 21 16:33:02 2023, max compression
```

## Comparing `findmycells-0.1.1.tar` & `findmycells-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.199355 findmycells-0.1.1/
--rw-r--r--   0 ds        (1000) ds        (1000)    35149 2022-10-27 16:21:08.000000 findmycells-0.1.1/LICENSE
--rw-rw-r--   0 ds        (1000) ds        (1000)      111 2022-09-05 16:31:43.000000 findmycells-0.1.1/MANIFEST.in
--rw-r--r--   0 ds        (1000) ds        (1000)     3089 2023-02-21 15:15:57.199355 findmycells-0.1.1/PKG-INFO
--rw-r--r--   0 ds        (1000) ds        (1000)     2225 2023-02-21 15:12:35.000000 findmycells-0.1.1/README.md
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.189355 findmycells-0.1.1/findmycells/
--rw-r--r--   0 ds        (1000) ds        (1000)      244 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)   178751 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/_modidx.py
--rw-r--r--   0 ds        (1000) ds        (1000)    25349 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/configs.py
--rw-r--r--   0 ds        (1000) ds        (1000)    17831 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/core.py
--rw-r--r--   0 ds        (1000) ds        (1000)    26899 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/database.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.189355 findmycells-0.1.1/findmycells/inspection/
--rw-r--r--   0 ds        (1000) ds        (1000)       21 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/inspection/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)    26361 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/inspection/methods.py
--rw-r--r--   0 ds        (1000) ds        (1000)    93566 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/interfaces.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.189355 findmycells-0.1.1/findmycells/postprocessing/
--rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/postprocessing/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)     4446 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/postprocessing/specs.py
--rw-r--r--   0 ds        (1000) ds        (1000)    42640 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/postprocessing/strategies.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.189355 findmycells-0.1.1/findmycells/preprocessing/
--rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/preprocessing/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)     8625 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/preprocessing/specs.py
--rw-r--r--   0 ds        (1000) ds        (1000)    25613 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/preprocessing/strategies.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.199355 findmycells-0.1.1/findmycells/quantification/
--rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/quantification/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)     4120 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/quantification/specs.py
--rw-r--r--   0 ds        (1000) ds        (1000)     1847 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/quantification/strategies.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.199355 findmycells-0.1.1/findmycells/readers/
--rw-r--r--   0 ds        (1000) ds        (1000)       70 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/readers/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)     9514 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/readers/microscopy_images.py
--rw-r--r--   0 ds        (1000) ds        (1000)     3689 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/readers/rois.py
--rw-r--r--   0 ds        (1000) ds        (1000)    10942 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/readers/specs.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.199355 findmycells-0.1.1/findmycells/segmentation/
--rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/segmentation/__init__.py
--rw-r--r--   0 ds        (1000) ds        (1000)     4050 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/segmentation/specs.py
--rw-r--r--   0 ds        (1000) ds        (1000)    23151 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/segmentation/strategies.py
--rw-r--r--   0 ds        (1000) ds        (1000)     4316 2023-02-21 15:15:27.000000 findmycells-0.1.1/findmycells/utils.py
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.189355 findmycells-0.1.1/findmycells.egg-info/
-drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 15:15:57.189355 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 ds        (1000) ds        (1000)     1056 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 ds        (1000) ds        (1000)     1112 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 ds        (1000) ds        (1000)        1 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
--rw-r--r--   0 ds        (1000) ds        (1000)      156 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 ds        (1000) ds        (1000)       12 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 ds        (1000) ds        (1000)     3089 2023-02-21 15:15:57.000000 findmycells-0.1.1/findmycells.egg-info/PKG-INFO
--rw-r--r--   0 ds        (1000) ds        (1000)     1504 2023-02-21 15:15:57.000000 findmycells-0.1.1/findmycells.egg-info/SOURCES.txt
--rw-r--r--   0 ds        (1000) ds        (1000)        1 2023-02-21 15:15:57.000000 findmycells-0.1.1/findmycells.egg-info/dependency_links.txt
--rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 15:15:57.000000 findmycells-0.1.1/findmycells.egg-info/entry_points.txt
--rw-r--r--   0 ds        (1000) ds        (1000)        1 2023-02-20 11:52:43.000000 findmycells-0.1.1/findmycells.egg-info/not-zip-safe
--rw-r--r--   0 ds        (1000) ds        (1000)      140 2023-02-21 15:15:57.000000 findmycells-0.1.1/findmycells.egg-info/requires.txt
--rw-r--r--   0 ds        (1000) ds        (1000)       12 2023-02-21 15:15:57.000000 findmycells-0.1.1/findmycells.egg-info/top_level.txt
--rw-r--r--   0 ds        (1000) ds        (1000)     1083 2023-02-21 15:15:06.000000 findmycells-0.1.1/settings.ini
--rw-r--r--   0 ds        (1000) ds        (1000)       38 2023-02-21 15:15:57.199355 findmycells-0.1.1/setup.cfg
--rw-rw-r--   0 ds        (1000) ds        (1000)     2541 2022-09-05 16:31:43.000000 findmycells-0.1.1/setup.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.959362 findmycells-0.1.2/
+-rw-r--r--   0 ds        (1000) ds        (1000)    35149 2022-10-27 16:21:08.000000 findmycells-0.1.2/LICENSE
+-rw-rw-r--   0 ds        (1000) ds        (1000)      111 2022-09-05 16:31:43.000000 findmycells-0.1.2/MANIFEST.in
+-rw-r--r--   0 ds        (1000) ds        (1000)     3089 2023-02-21 16:33:02.959362 findmycells-0.1.2/PKG-INFO
+-rw-r--r--   0 ds        (1000) ds        (1000)     2225 2023-02-21 16:32:08.000000 findmycells-0.1.2/README.md
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.949362 findmycells-0.1.2/findmycells/
+-rw-r--r--   0 ds        (1000) ds        (1000)      244 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)   178751 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/_modidx.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    25349 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/configs.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    17831 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/core.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    26899 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/database.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.949362 findmycells-0.1.2/findmycells/inspection/
+-rw-r--r--   0 ds        (1000) ds        (1000)       21 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/inspection/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    26361 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/inspection/methods.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    93566 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/interfaces.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.949362 findmycells-0.1.2/findmycells/postprocessing/
+-rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/postprocessing/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     4446 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/postprocessing/specs.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    42640 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/postprocessing/strategies.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.959362 findmycells-0.1.2/findmycells/preprocessing/
+-rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/preprocessing/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     8625 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/preprocessing/specs.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    25613 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/preprocessing/strategies.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.959362 findmycells-0.1.2/findmycells/quantification/
+-rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/quantification/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     4120 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/quantification/specs.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     1847 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/quantification/strategies.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.959362 findmycells-0.1.2/findmycells/readers/
+-rw-r--r--   0 ds        (1000) ds        (1000)       70 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/readers/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     9514 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/readers/microscopy_images.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     3689 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/readers/rois.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    10942 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/readers/specs.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.959362 findmycells-0.1.2/findmycells/segmentation/
+-rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/segmentation/__init__.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     4050 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/segmentation/specs.py
+-rw-r--r--   0 ds        (1000) ds        (1000)    23151 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/segmentation/strategies.py
+-rw-r--r--   0 ds        (1000) ds        (1000)     4316 2023-02-21 16:31:55.000000 findmycells-0.1.2/findmycells/utils.py
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.949362 findmycells-0.1.2/findmycells.egg-info/
+drwxr-xr-x   0 ds        (1000) ds        (1000)        0 2023-02-21 16:33:02.949362 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 ds        (1000) ds        (1000)     1056 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 ds        (1000) ds        (1000)     1112 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)        1 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)      156 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)       12 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)     3089 2023-02-21 16:33:02.000000 findmycells-0.1.2/findmycells.egg-info/PKG-INFO
+-rw-r--r--   0 ds        (1000) ds        (1000)     1504 2023-02-21 16:33:02.000000 findmycells-0.1.2/findmycells.egg-info/SOURCES.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)        1 2023-02-21 16:33:02.000000 findmycells-0.1.2/findmycells.egg-info/dependency_links.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)       44 2023-02-21 16:33:02.000000 findmycells-0.1.2/findmycells.egg-info/entry_points.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)        1 2023-02-20 11:52:43.000000 findmycells-0.1.2/findmycells.egg-info/not-zip-safe
+-rw-r--r--   0 ds        (1000) ds        (1000)      177 2023-02-21 16:33:02.000000 findmycells-0.1.2/findmycells.egg-info/requires.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)       12 2023-02-21 16:33:02.000000 findmycells-0.1.2/findmycells.egg-info/top_level.txt
+-rw-r--r--   0 ds        (1000) ds        (1000)     1120 2023-02-21 16:31:22.000000 findmycells-0.1.2/settings.ini
+-rw-r--r--   0 ds        (1000) ds        (1000)       38 2023-02-21 16:33:02.959362 findmycells-0.1.2/setup.cfg
+-rw-rw-r--   0 ds        (1000) ds        (1000)     2541 2022-09-05 16:31:43.000000 findmycells-0.1.2/setup.py
```

### Comparing `findmycells-0.1.1/LICENSE` & `findmycells-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/PKG-INFO` & `findmycells-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmycells
-Version: 0.1.1
+Version: 0.1.2
 Summary: An end-to-end bioimage analysis pipeline with state-of-the-art tools for non-coding experts
 Home-page: https://github.com/Defense-Circuits-Lab/findmycells
 Author: DSegebarth
 Author-email: d.segebarth@gmail.com
 License: GNU General Public License v3
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmycells Version: 0.1.1 Summary: An end-to-end
+Metadata-Version: 2.1 Name: findmycells Version: 0.1.2 Summary: An end-to-end
 bioimage analysis pipeline with state-of-the-art tools for non-coding experts
 Home-page: https://github.com/Defense-Circuits-Lab/findmycells Author:
 DSegebarth Author-email: d.segebarth@gmail.com License: GNU General Public
 License v3 Keywords: nbdev jupyter notebook python Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `findmycells-0.1.1/README.md` & `findmycells-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/_modidx.py` & `findmycells-0.1.2/findmycells/_modidx.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/configs.py` & `findmycells-0.1.2/findmycells/configs.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/core.py` & `findmycells-0.1.2/findmycells/core.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/database.py` & `findmycells-0.1.2/findmycells/database.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/inspection/methods.py` & `findmycells-0.1.2/findmycells/inspection/methods.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/interfaces.py` & `findmycells-0.1.2/findmycells/interfaces.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/postprocessing/specs.py` & `findmycells-0.1.2/findmycells/postprocessing/specs.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/postprocessing/strategies.py` & `findmycells-0.1.2/findmycells/postprocessing/strategies.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/preprocessing/specs.py` & `findmycells-0.1.2/findmycells/preprocessing/specs.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/preprocessing/strategies.py` & `findmycells-0.1.2/findmycells/preprocessing/strategies.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/quantification/specs.py` & `findmycells-0.1.2/findmycells/quantification/specs.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/quantification/strategies.py` & `findmycells-0.1.2/findmycells/quantification/strategies.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/readers/microscopy_images.py` & `findmycells-0.1.2/findmycells/readers/microscopy_images.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/readers/rois.py` & `findmycells-0.1.2/findmycells/readers/rois.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/readers/specs.py` & `findmycells-0.1.2/findmycells/readers/specs.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/segmentation/specs.py` & `findmycells-0.1.2/findmycells/segmentation/specs.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/segmentation/strategies.py` & `findmycells-0.1.2/findmycells/segmentation/strategies.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells/utils.py` & `findmycells-0.1.2/findmycells/utils.py`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `findmycells-0.1.2/findmycells.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/findmycells.egg-info/PKG-INFO` & `findmycells-0.1.2/findmycells.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmycells
-Version: 0.1.1
+Version: 0.1.2
 Summary: An end-to-end bioimage analysis pipeline with state-of-the-art tools for non-coding experts
 Home-page: https://github.com/Defense-Circuits-Lab/findmycells
 Author: DSegebarth
 Author-email: d.segebarth@gmail.com
 License: GNU General Public License v3
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmycells Version: 0.1.1 Summary: An end-to-end
+Metadata-Version: 2.1 Name: findmycells Version: 0.1.2 Summary: An end-to-end
 bioimage analysis pipeline with state-of-the-art tools for non-coding experts
 Home-page: https://github.com/Defense-Circuits-Lab/findmycells Author:
 DSegebarth Author-email: d.segebarth@gmail.com License: GNU General Public
 License v3 Keywords: nbdev jupyter notebook python Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `findmycells-0.1.1/findmycells.egg-info/SOURCES.txt` & `findmycells-0.1.2/findmycells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findmycells-0.1.1/settings.ini` & `findmycells-0.1.2/settings.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = findmycells
 lib_name = findmycells
-version = 0.1.1
+version = 0.1.2
 min_python = 3.7
 license = gpl3
 doc_path = _docs
 lib_path = findmycells
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,16 +21,16 @@
 author_email = d.segebarth@gmail.com
 copyright = 2022 onwards, DSegebarth
 description = An end-to-end bioimage analysis pipeline with state-of-the-art tools for non-coding experts
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Defense-Circuits-Lab
-requirements = shapely>=1.8.0 ipywidgets==7.6.5
-pip_requirements = deepflash2==0.1.7 cellpose>=2.0.5 czifile roifile connected-components-3d ipyfilechooser wget
+requirements = shapely>=1.8.0 ipywidgets==7.6.5 jupyterlab
+pip_requirements = deepflash2==0.1.7 cellpose>=2.0.5 czifile roifile connected-components-3d ipyfilechooser wget jupyterlab-widgets==1.0.2
 dev_requirements = nbdev
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
```

### Comparing `findmycells-0.1.1/setup.py` & `findmycells-0.1.2/setup.py`

 * *Files identical despite different names*

