# Comparing `tmp/mmif-python-1.0.5.tar.gz` & `tmp/mmif-python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-1.0.5.tar", last modified: Wed Jul 19 07:30:46 2023, max compression
+gzip compressed data, was "mmif-python-1.0.6.tar", last modified: Wed Jul 19 14:48:57 2023, max compression
```

## Comparing `mmif-python-1.0.5.tar` & `mmif-python-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 07:30:12.000000 mmif-python-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-19 07:30:12.000000 mmif-python-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 07:30:46.556393 mmif-python-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 07:30:12.000000 mmif-python-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 07:30:12.000000 mmif-python-1.0.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:45.000000 mmif-python-1.0.5/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 07:30:45.000000 mmif-python-1.0.5/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-19 07:30:45.000000 mmif-python-1.0.5/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-19 07:30:12.000000 mmif-python-1.0.5/mmif/utils/video_document_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 07:30:45.000000 mmif-python-1.0.5/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 07:30:45.000000 mmif-python-1.0.5/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:46.556393 mmif-python-1.0.5/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 07:30:46.000000 mmif-python-1.0.5/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 07:30:12.000000 mmif-python-1.0.5/requirements.cv
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 07:30:12.000000 mmif-python-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:30:46.556393 mmif-python-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-19 07:30:12.000000 mmif-python-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.176333 mmif-python-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 14:48:21.000000 mmif-python-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-19 14:48:21.000000 mmif-python-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 14:48:57.176333 mmif-python-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 14:48:21.000000 mmif-python-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 14:48:22.000000 mmif-python-1.0.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.172332 mmif-python-1.0.6/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.172332 mmif-python-1.0.6/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:56.000000 mmif-python-1.0.6/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 14:48:56.000000 mmif-python-1.0.6/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.172332 mmif-python-1.0.6/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.172332 mmif-python-1.0.6/mmif/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-19 14:48:22.000000 mmif-python-1.0.6/mmif/utils/video_document_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.172332 mmif-python-1.0.6/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 14:48:56.000000 mmif-python-1.0.6/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 14:48:56.000000 mmif-python-1.0.6/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.176333 mmif-python-1.0.6/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:48:57.176333 mmif-python-1.0.6/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 14:48:57.000000 mmif-python-1.0.6/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 14:48:22.000000 mmif-python-1.0.6/requirements.cv
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 14:48:22.000000 mmif-python-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:48:57.176333 mmif-python-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-19 14:48:22.000000 mmif-python-1.0.6/setup.py
```

### Comparing `mmif-python-1.0.5/LICENSE` & `mmif-python-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/PKG-INFO` & `mmif-python-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.5/mmif/__init__.py` & `mmif-python-1.0.6/mmif/__init__.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.6/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/res/mmif.json` & `mmif-python-1.0.6/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/serialize/annotation.py` & `mmif-python-1.0.6/mmif/serialize/annotation.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/serialize/mmif.py` & `mmif-python-1.0.6/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/serialize/model.py` & `mmif-python-1.0.6/mmif/serialize/model.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/serialize/view.py` & `mmif-python-1.0.6/mmif/serialize/view.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/utils/video_document_helper.py` & `mmif-python-1.0.6/mmif/utils/video_document_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import importlib
+import warnings
 from typing import List, Union, Tuple
 
-import numpy as np
-from PIL import Image
-
+import mmif
 from mmif import Annotation, Document, Mmif
 from mmif.vocabulary import DocumentTypes
 
-try:
-    import cv2
-    import ffmpeg
-    import PIL
-except ImportError as e:
-    raise ImportError(
-        f"Optional package {e.name} not found. You might want to install Computer-Vision dependencies by running `pip install mmif-python[cv]`")
+for cv_dep in ('cv2', 'ffmpeg', 'PIL'):
+    try:
+        importlib.__import__(cv_dep)
+    except ImportError as e:
+        warnings.warn(f"Optional package \"{e.name}\" is not found. "
+                      f"You might want to install Computer-Vision dependencies "
+                      f"by running `pip install mmif-python[cv]=={mmif.__version__}`")
+
 
 FPS_DOCPROP_KEY = 'fps'
 UNIT_NORMALIZATION = {
     'm': 'millisecond',
     'ms': 'millisecond',
     'msec': 'millisecond',
     'millisecond': 'millisecond',
@@ -29,15 +30,16 @@
     'f': 'frame',
     'fr': 'frame',
     'frame': 'frame',
     'frames': 'frame',
 }
 
 
-def capture(vd: Document) -> cv2.VideoCapture:
+def capture(vd: Document):
+    import cv2  # pytype: disable=import-error
     if vd is None or vd.at_type != DocumentTypes.VideoDocument:
         raise ValueError(f'The document does not exist.')
 
     v = cv2.VideoCapture(vd.location_path())
     vd.add_property(FPS_DOCPROP_KEY, v.get(cv2.CAP_PROP_FPS))
     return v
 
@@ -51,37 +53,40 @@
         if k in vd:
             fps = vd.get_property(k)
             return fps
     capture(vd)
     return vd.get_property(FPS_DOCPROP_KEY)
 
 
-def extract_frames_as_images(vd: Document, framenums: List[int], as_PIL: bool = False) -> List[Union[np.ndarray, PIL.Image.Image]]:
+def extract_frames_as_images(vd: Document, framenums: List[int], as_PIL: bool = False):
     """
     Extracts frames from a video document as a list of numpy arrays.
     Use `sample_frames` function in this module to get the list of frame numbers first. 
     
     :param vd: VideoDocument object that holds the video file location
     :param framenums: integers representing the frame numbers to extract
     :param as_PIL: use PIL.Image instead of numpy.ndarray
     :return: frames as a list of numpy arrays or PIL.Image objects
     """
+    import cv2  # pytype: disable=import-error
+    if as_PIL:
+        from PIL import Image
     frames = []
     video = capture(vd)
     for framenum in framenums:
         video.set(cv2.CAP_PROP_POS_FRAMES, framenum)
         ret, frame = video.read()
         if ret:
             frames.append(Image.fromarray(frame[:, :, ::-1]) if as_PIL else frame)
         else:
             break
     return frames
 
 
-def extract_mid_frame(mmif: Mmif, tf: Annotation, as_PIL: bool = False) -> Union[np.ndarray, PIL.Image.Image]:
+def extract_mid_frame(mmif: Mmif, tf: Annotation, as_PIL: bool = False):
     """
     Extracts the middle frame from a video document
     """
     timeunit = get_annotation_property(mmif, tf, 'timeUnit')
     vd = mmif[get_annotation_property(mmif, tf, 'document')]
     fps = get_framerate(vd)
     midframe = sum(convert(float(tf.get_property(timepoint_propkey)), timeunit, 'frame', fps) for timepoint_propkey in ('start', 'end')) // 2
```

### Comparing `mmif-python-1.0.5/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.6/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/vocabulary/base_types.py` & `mmif-python-1.0.6/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif/vocabulary/document_types.py` & `mmif-python-1.0.6/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.6/mmif_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.5/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.6/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.5/setup.py` & `mmif-python-1.0.6/setup.py`

 * *Files identical despite different names*

