# Comparing `tmp/qcio-0.3.3.tar.gz` & `tmp/qcio-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.3.3.tar", max compression
+gzip compressed data, was "qcio-0.3.4.tar", max compression
```

## Comparing `qcio-0.3.3.tar` & `qcio-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1079 2023-07-18 02:24:27.790026 qcio-0.3.3/LICENSE
--rw-r--r--   0        0        0      898 2023-07-18 02:24:27.790026 qcio-0.3.3/README.md
--rw-r--r--   0        0        0     1246 2023-07-18 02:24:27.790026 qcio-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      573 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/constants.py
--rw-r--r--   0        0        0      483 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/helper_types.py
--rw-r--r--   0        0        0      272 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/models/__init__.py
--rw-r--r--   0        0        0     9738 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/models/base_models.py
--rw-r--r--   0        0        0     3082 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/models/inputs.py
--rw-r--r--   0        0        0     2236 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     8354 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/molecule.py
--rw-r--r--   0        0        0     3585 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/outputs.py
--rw-r--r--   0        0        0     1935 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/outputs_base.py
--rw-r--r--   0        0        0     4794 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/results.py
--rw-r--r--   0        0        0     4569 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/qcel.py
--rw-r--r--   0        0        0      838 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/utils.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-19 00:17:48.815614 qcio-0.3.4/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-19 00:17:48.815614 qcio-0.3.4/README.md
+-rw-r--r--   0        0        0     1246 2023-07-19 00:17:48.815614 qcio-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/constants.py
+-rw-r--r--   0        0        0      483 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/helper_types.py
+-rw-r--r--   0        0        0      235 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/__init__.py
+-rw-r--r--   0        0        0     9738 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3082 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2236 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     8354 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/molecule.py
+-rw-r--r--   0        0        0     8102 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1935 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0     4569 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/qcel.py
+-rw-r--r--   0        0        0      838 2023-07-19 00:17:48.815614 qcio-0.3.4/qcio/utils.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.4/PKG-INFO
```

### Comparing `qcio-0.3.3/LICENSE` & `qcio-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/README.md` & `qcio-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/pyproject.toml` & `qcio-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.3.3"
+version = "0.3.4"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.3.3/qcio/__init__.py` & `qcio-0.3.4/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/models/base_models.py` & `qcio-0.3.4/qcio/models/base_models.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/models/inputs.py` & `qcio-0.3.4/qcio/models/inputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/models/inputs_base.py` & `qcio-0.3.4/qcio/models/inputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/models/molecule.py` & `qcio-0.3.4/qcio/models/molecule.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/models/outputs_base.py` & `qcio-0.3.4/qcio/models/outputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/qcel.py` & `qcio-0.3.4/qcio/qcel.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/qcio/utils.py` & `qcio-0.3.4/qcio/utils.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.3/PKG-INFO` & `qcio-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.3.3
+Version: 0.3.4
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

