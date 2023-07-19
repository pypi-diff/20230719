# Comparing `tmp/mmif-python-1.0.2.tar.gz` & `tmp/mmif-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-1.0.2.tar", last modified: Tue Jul 11 01:07:32 2023, max compression
+gzip compressed data, was "mmif-python-1.0.3.tar", last modified: Wed Jul 19 04:48:28 2023, max compression
```

## Comparing `mmif-python-1.0.2.tar` & `mmif-python-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.870120 mmif-python-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-11 01:06:51.000000 mmif-python-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 01:06:51.000000 mmif-python-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-11 01:07:32.870120 mmif-python-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 01:06:51.000000 mmif-python-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 01:06:51.000000 mmif-python-1.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.862120 mmif-python-1.0.2/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.862120 mmif-python-1.0.2/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.862120 mmif-python-1.0.2/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.866120 mmif-python-1.0.2/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.866120 mmif-python-1.0.2/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.870120 mmif-python-1.0.2/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 01:06:51.000000 mmif-python-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:07:32.870120 mmif-python-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-11 01:06:51.000000 mmif-python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 04:47:56.000000 mmif-python-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 04:47:56.000000 mmif-python-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 04:48:28.537462 mmif-python-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 04:47:56.000000 mmif-python-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 04:47:57.000000 mmif-python-1.0.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.533462 mmif-python-1.0.3/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.533462 mmif-python-1.0.3/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-19 04:47:56.000000 mmif-python-1.0.3/mmif/utils/video_document_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:48:28.537462 mmif-python-1.0.3/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 04:48:28.000000 mmif-python-1.0.3/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 04:47:56.000000 mmif-python-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:48:28.537462 mmif-python-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-19 04:47:56.000000 mmif-python-1.0.3/setup.py
```

### Comparing `mmif-python-1.0.2/LICENSE` & `mmif-python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/PKG-INFO` & `mmif-python-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai). 
@@ -13,8 +13,9 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cv
 Provides-Extra: dev
```

### Comparing `mmif-python-1.0.2/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.3/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif/res/mmif.json` & `mmif-python-1.0.3/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif/serialize/annotation.py` & `mmif-python-1.0.3/mmif/serialize/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 In MMIF, annotations are created by apps in a pipeline as a part
 of a view. For documentation on how views are represented, see
 :mod:`mmif.serialize.view`.
 """
 import importlib
 import itertools
+import os
 import pathlib
 import pkgutil
 import re
 import typing
 import warnings
 from typing import Union, Dict, List, Optional, Iterator, MutableMapping, TypeVar
 from urllib.parse import urlparse
@@ -131,14 +132,21 @@
             raise KeyError(f"Property {prop_name} does not exist in this annotation.")
 
     get_property = get
 
     def __getitem__(self, prop_name: str):
         return self.get(prop_name)
     
+    def __contains__(self, item):
+        try:
+            self.get(item)
+            return True
+        except KeyError:
+            return False
+    
     def is_document(self):
         return isinstance(self.at_type, DocumentTypesBase)
 
 
 class Document(Annotation):
     """
     Document object that represents a single document in a MMIF file.
@@ -215,15 +223,23 @@
 
     def get(self, prop_name):
         """
         A special getter for Document properties. This is to allow for reading 
         the three properties in a specific order so that the latest value is 
         returned, in case there are multiple values for the same key.
         """
-        if prop_name in self._props_temporary:
+        if prop_name == 'id':
+            # because all three dicts have `id` key as required field, we need
+            # this special case to return the correct value from the correct dict
+            return self.id
+        elif prop_name == 'location':
+            # because location is internally stored in self.location_,
+            # it doesn't work with regular __getitem__ method
+            return self.location
+        elif prop_name in self._props_temporary:
             return self._props_temporary[prop_name]
         elif prop_name in self._props_existing:
             return self._props_existing[prop_name]
         else:
             return super().get(prop_name)
 
     get_property = get
@@ -374,15 +390,15 @@
         super()._deserialize(input_dict)
 
     def _serialize(self, alt_container: Optional[Dict] = None) -> dict:
         serialized = super()._serialize()
         if "location_" in serialized:
             serialized["location"] = serialized.pop("location_")
         return serialized
-
+    
     @property
     def text_language(self) -> str:
         return self.text.lang
 
     @text_language.setter
     def text_language(self, lang_code: str) -> None:
         self.text.lang = lang_code
@@ -434,33 +450,37 @@
         else:
             return "".join((parsed_location.netloc, parsed_location.path))
 
     def location_path(self) -> Optional[str]:
         warnings.warn('location_path() is deprecated. Use location_path_resolved() instead.', DeprecationWarning)
         return self.location_path_resolved()
     
-    def location_path_resolved(self) -> Optional[str]:
+    def location_path_resolved(self, nonexist_ok=True) -> Optional[str]:
         """
         Retrieves only path name of the document location (hostname is ignored), 
         and then try to resolve the path name in the local file system.
         This method should be used when the document scheme is ``file`` or empty.
         For other schemes, users should install ``mmif-locdoc-<scheme>`` plugin.
         
         Returns None when no location is set.
         Raise ValueError when no code found to resolve the given location scheme.
         """
         if self.location is None:
             return None
         scheme = self.location_scheme()
         if scheme in ('', 'file'):
-            return urlparse(self.location).path
+            p = urlparse(self.location).path
         elif scheme in discovered_docloc_plugins:
-            return discovered_docloc_plugins[scheme].resolve(self.location)
+            p = discovered_docloc_plugins[scheme].resolve(self.location)
         else:
             raise ValueError(f'Cannot resolve location of scheme "{scheme}". Interested in developing mmif-locdoc-{scheme} plugin? See https://clams.ai/mmif-python/plugins')
+        if not nonexist_ok and not os.path.exists(p):
+            raise FileNotFoundError(f'Cannot find file "{p}"')
+        else:
+            return p
 
     def location_path_literal(self) -> Optional[str]:
         """
         Retrieves only path name of the document location (hostname is ignored). 
         Returns None when no location is set.
         """
         if self.location is None:
```

### Comparing `mmif-python-1.0.2/mmif/serialize/mmif.py` & `mmif-python-1.0.3/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif/serialize/model.py` & `mmif-python-1.0.3/mmif/serialize/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 
 These objects are generally instantiated from JSON, either as a string
 or as an already-loaded Python dictionary. This base class provides the
 core functionality for deserializing MMIF JSON data into live objects
 and serializing live objects into MMIF JSON data. Specialized behavior
 for the different components of MMIF is added in the subclasses.
 """
+
 import json
 from datetime import datetime
-from types import MethodType
 from typing import Union, Any, Dict, Optional, TypeVar, Generic, Generator, Iterator, Type, Set
 
 from deepdiff import DeepDiff
 
-import mmif
-
 T = TypeVar('T')
 S = TypeVar('S')
 JSON_PRMTV_TYPES: Type = Union[str, int, float, bool, None]
 
 __all__ = [
     'MmifObject',
     'MmifObjectEncoder',
@@ -101,16 +99,14 @@
             self._required_attributes = []
         if not hasattr(self, '_exclude_from_diff'):
             self._exclude_from_diff = set()
         if not hasattr(self, '_unnamed_attributes'):
             self._unnamed_attributes = {}
         if mmif_obj is not None:
             self.deserialize(mmif_obj)
-        for method in mmif.patches[self.__class__]:
-            setattr(self, method.__name__, MethodType(method, self))
 
     def disallow_additional_properties(self) -> None:
         """
         Call this method in :func:`__init__` to prevent the insertion
         of unnamed attributes after initialization.
         """
         self._unnamed_attributes = None
```

### Comparing `mmif-python-1.0.2/mmif/serialize/view.py` & `mmif-python-1.0.3/mmif/serialize/view.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.3/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif/vocabulary/base_types.py` & `mmif-python-1.0.3/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif/vocabulary/document_types.py` & `mmif-python-1.0.3/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.2/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.3/mmif_python.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai). 
@@ -13,8 +13,9 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cv
 Provides-Extra: dev
```

### Comparing `mmif-python-1.0.2/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.3/mmif_python.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 mmif/res/do-not-edit.txt
 mmif/res/mmif.json
 mmif/serialize/__init__.py
 mmif/serialize/annotation.py
 mmif/serialize/mmif.py
 mmif/serialize/model.py
 mmif/serialize/view.py
+mmif/utils/__init__.py
+mmif/utils/video_document_helper.py
 mmif/ver/__init__.py
 mmif/ver/do-not-edit.txt
 mmif/vocabulary/__init__.py
 mmif/vocabulary/annotation_types.py
 mmif/vocabulary/base_types.py
 mmif/vocabulary/do-not-edit.txt
 mmif/vocabulary/document_types.py
```

### Comparing `mmif-python-1.0.2/setup.py` & `mmif-python-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,17 @@
 
 with open('README.md') as readme:
     long_desc = readme.read()
 
 with open('requirements.txt') as requirements:
     requires = requirements.readlines()
 
+with open('requirements.cv') as requirements:
+    cv_requires = requirements.readlines()
+
 setuptools.setup(
     name=name,
     version=version,
     author="Brandeis Lab for Linguistics and Computation",
     author_email="admin@clams.ai",
     description="Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)",
     long_description=long_desc,
@@ -283,14 +286,15 @@
     # this is for *building*, building (build, bdist_*) doesn't get along with MANIFEST.in
     # so using this param explicitly is much safer implementation
     package_data={
         'mmif': [f'{mmif_res_pkg}/*', f'{mmif_ver_pkg}/*', f'{mmif_vocabulary_pkg}/*'],
     },
     install_requires=requires,
     extras_require={
+        'cv': cv_requires,
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov',
             'pytype',
             'sphinx'
         ]
```

