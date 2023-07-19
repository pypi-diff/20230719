# Comparing `tmp/jref-0.3.0.tar.gz` & `tmp/jref-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jref-0.3.0.tar", last modified: Wed Sep 22 12:51:30 2021, max compression
+gzip compressed data, was "jref-0.4.1.tar", last modified: Wed Jul 19 10:30:34 2023, max compression
```

## Comparing `jref-0.3.0.tar` & `jref-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:30.366670 jref-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-22 12:51:21.000000 jref-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2021-09-22 12:51:30.366670 jref-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2021-09-22 12:51:21.000000 jref-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:30.362670 jref-0.3.0/jref/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:21.000000 jref-0.3.0/jref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2021-09-22 12:51:21.000000 jref-0.3.0/jref/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7160 2021-09-22 12:51:21.000000 jref-0.3.0/jref/context.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-22 12:51:21.000000 jref-0.3.0/jref/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2021-09-22 12:51:21.000000 jref-0.3.0/jref/pointer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-09-22 12:51:21.000000 jref-0.3.0/jref/reference.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-09-22 12:51:21.000000 jref-0.3.0/jref/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:30.362670 jref-0.3.0/jref/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/test_document_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7332 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/test_pointer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5155 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-09-22 12:51:21.000000 jref-0.3.0/jref/test/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-22 12:51:21.000000 jref-0.3.0/jref/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:30.366670 jref-0.3.0/jref/util/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-09-22 12:51:21.000000 jref-0.3.0/jref/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-09-22 12:51:21.000000 jref-0.3.0/jref/util/document_cache_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-09-22 12:51:21.000000 jref-0.3.0/jref/util/equality_comparable_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2021-09-22 12:51:21.000000 jref-0.3.0/jref/util/streaming_request.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-22 12:51:21.000000 jref-0.3.0/jref/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-09-22 12:51:21.000000 jref-0.3.0/jref/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 12:51:30.362670 jref-0.3.0/jref.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2021-09-22 12:51:30.000000 jref-0.3.0/jref.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      683 2021-09-22 12:51:30.000000 jref-0.3.0/jref.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-22 12:51:30.000000 jref-0.3.0/jref.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-09-22 12:51:30.000000 jref-0.3.0/jref.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-22 12:51:30.000000 jref-0.3.0/jref.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-09-22 12:51:30.000000 jref-0.3.0/jref.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-22 12:51:21.000000 jref-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-09-22 12:51:30.366670 jref-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-09-22 12:51:21.000000 jref-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:34.847010 jref-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 10:30:09.000000 jref-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-19 10:30:34.847010 jref-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-19 10:30:09.000000 jref-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:34.847010 jref-0.4.1/jref/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:09.000000 jref-0.4.1/jref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-19 10:30:09.000000 jref-0.4.1/jref/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-19 10:30:09.000000 jref-0.4.1/jref/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 10:30:09.000000 jref-0.4.1/jref/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-19 10:30:09.000000 jref-0.4.1/jref/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-19 10:30:09.000000 jref-0.4.1/jref/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-19 10:30:09.000000 jref-0.4.1/jref/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:34.847010 jref-0.4.1/jref/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/test_document_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/test_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-19 10:30:09.000000 jref-0.4.1/jref/test/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 10:30:09.000000 jref-0.4.1/jref/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:34.847010 jref-0.4.1/jref/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-19 10:30:09.000000 jref-0.4.1/jref/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-19 10:30:09.000000 jref-0.4.1/jref/util/document_cache_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-19 10:30:09.000000 jref-0.4.1/jref/util/equality_comparable_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-19 10:30:09.000000 jref-0.4.1/jref/util/streaming_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 10:30:09.000000 jref-0.4.1/jref/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-19 10:30:09.000000 jref-0.4.1/jref/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:30:34.847010 jref-0.4.1/jref.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-19 10:30:34.000000 jref-0.4.1/jref.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-19 10:30:34.000000 jref-0.4.1/jref.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:30:34.000000 jref-0.4.1/jref.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 10:30:34.000000 jref-0.4.1/jref.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-19 10:30:34.000000 jref-0.4.1/jref.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 10:30:34.000000 jref-0.4.1/jref.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-19 10:30:09.000000 jref-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 10:30:34.851010 jref-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-19 10:30:09.000000 jref-0.4.1/setup.py
```

### Comparing `jref-0.3.0/LICENSE` & `jref-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/PKG-INFO` & `jref-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: jref
-Version: 0.3.0
+Version: 0.4.1
 Summary: JSON Reference and JSON Pointer implementations
 Home-page: https://github.com/biochimia/python-jref
 Author: João Abecasis
 Author-email: joao@abecasis.name
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -100,9 +98,7 @@
 ```
 
 ## References
 
 * JSON Reference, Internet Draft,
   https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03
 * JSON Pointer, RFC 6901, https://tools.ietf.org/html/rfc6901
-
-
```

### Comparing `jref-0.3.0/README.md` & `jref-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/__main__.py` & `jref-0.4.1/jref/__main__.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/context.py` & `jref-0.4.1/jref/context.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/pointer.py` & `jref-0.4.1/jref/pointer.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/reference.py` & `jref-0.4.1/jref/reference.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/scalar.py` & `jref-0.4.1/jref/scalar.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/test/test_data.py` & `jref-0.4.1/jref/test/test_data.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/test/test_document_cache.py` & `jref-0.4.1/jref/test/test_document_cache.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/test/test_pointer.py` & `jref-0.4.1/jref/test/test_pointer.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/test/test_reference.py` & `jref-0.4.1/jref/test/test_reference.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/test/test_scalar.py` & `jref-0.4.1/jref/test/test_scalar.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/test/test_yaml.py` & `jref-0.4.1/jref/test/test_yaml.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/util/document_cache_mixin.py` & `jref-0.4.1/jref/util/document_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/util/streaming_request.py` & `jref-0.4.1/jref/util/streaming_request.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref/yaml.py` & `jref-0.4.1/jref/yaml.py`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/jref.egg-info/PKG-INFO` & `jref-0.4.1/jref.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: jref
-Version: 0.3.0
+Version: 0.4.1
 Summary: JSON Reference and JSON Pointer implementations
 Home-page: https://github.com/biochimia/python-jref
 Author: João Abecasis
 Author-email: joao@abecasis.name
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -100,9 +98,7 @@
 ```
 
 ## References
 
 * JSON Reference, Internet Draft,
   https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03
 * JSON Pointer, RFC 6901, https://tools.ietf.org/html/rfc6901
-
-
```

### Comparing `jref-0.3.0/jref.egg-info/SOURCES.txt` & `jref-0.4.1/jref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jref-0.3.0/setup.py` & `jref-0.4.1/setup.py`

 * *Files identical despite different names*

