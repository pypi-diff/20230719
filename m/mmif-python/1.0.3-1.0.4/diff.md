# Comparing `tmp/mmif-python-1.0.3.tar.gz` & `tmp/mmif-python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-1.0.3.tar", last modified: Wed Jul 19 04:48:28 2023, max compression
+gzip compressed data, was "mmif-python-1.0.4.tar", last modified: Wed Jul 19 05:18:22 2023, max compression
```

## Comparing `mmif-python-1.0.3.tar` & `mmif-python-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 04:47:56.000000 mmif-python-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 04:47:56.000000 mmif-python-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 04:48:28.537462 mmif-python-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 04:47:56.000000 mmif-python-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 04:47:57.000000 mmif-python-1.0.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.533462 mmif-python-1.0.3/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.533462 mmif-python-1.0.3/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/utils/video_document_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 04:47:56.000000 mmif-python-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:48:28.537462 mmif-python-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-19 04:47:56.000000 mmif-python-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.851055 mmif-python-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 05:17:51.000000 mmif-python-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-19 05:17:51.000000 mmif-python-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 05:18:22.851055 mmif-python-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 05:17:51.000000 mmif-python-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 05:17:51.000000 mmif-python-1.0.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.847055 mmif-python-1.0.4/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.847055 mmif-python-1.0.4/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.851055 mmif-python-1.0.4/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.851055 mmif-python-1.0.4/mmif/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-19 05:17:51.000000 mmif-python-1.0.4/mmif/utils/video_document_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.851055 mmif-python-1.0.4/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.851055 mmif-python-1.0.4/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:18:22.851055 mmif-python-1.0.4/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 05:18:22.000000 mmif-python-1.0.4/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 05:17:51.000000 mmif-python-1.0.4/requirements.cv
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 05:17:51.000000 mmif-python-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:18:22.851055 mmif-python-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-19 05:17:51.000000 mmif-python-1.0.4/setup.py
```

### Comparing `mmif-python-1.0.3/LICENSE` & `mmif-python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/PKG-INFO` & `mmif-python-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.3/mmif/__init__.py` & `mmif-python-1.0.4/mmif/__init__.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.4/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/res/mmif.json` & `mmif-python-1.0.4/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/serialize/annotation.py` & `mmif-python-1.0.4/mmif/serialize/annotation.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/serialize/mmif.py` & `mmif-python-1.0.4/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/serialize/model.py` & `mmif-python-1.0.4/mmif/serialize/model.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/serialize/view.py` & `mmif-python-1.0.4/mmif/serialize/view.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/utils/video_document_helper.py` & `mmif-python-1.0.4/mmif/utils/video_document_helper.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.4/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/vocabulary/base_types.py` & `mmif-python-1.0.4/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif/vocabulary/document_types.py` & `mmif-python-1.0.4/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.3/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.4/mmif_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.3/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.4/mmif_python.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./VERSION
+./requirements.cv
 ./requirements.txt
 mmif/__init__.py
 mmif/res/__init__.py
 mmif/res/clams.vocabulary.yaml
 mmif/res/do-not-edit.txt
 mmif/res/mmif.json
 mmif/serialize/__init__.py
```

### Comparing `mmif-python-1.0.3/setup.py` & `mmif-python-1.0.4/setup.py`

 * *Files identical despite different names*

