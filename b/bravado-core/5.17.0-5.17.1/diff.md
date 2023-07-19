# Comparing `tmp/bravado-core-5.17.0.tar.gz` & `tmp/bravado-core-5.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bravado-core-5.17.0.tar", last modified: Fri Apr  3 13:21:26 2020, max compression
+gzip compressed data, was "dist/bravado-core-5.17.1.tar", last modified: Fri Sep  2 17:27:10 2022, max compression
```

## Comparing `bravado-core-5.17.0.tar` & `bravado-core-5.17.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 sjaensch (1475161668) AD\Domain Users (1954207199)        0 2020-04-03 13:21:26.369569 bravado-core-5.17.0/
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    28531 2020-04-03 13:20:11.000000 bravado-core-5.17.0/CHANGELOG.rst
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     1587 2020-03-09 08:35:34.000000 bravado-core-5.17.0/LICENSE.txt
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)       61 2020-03-09 08:35:34.000000 bravado-core-5.17.0/MANIFEST.in
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     3993 2020-04-03 13:21:26.369701 bravado-core-5.17.0/PKG-INFO
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     2446 2020-03-09 08:35:34.000000 bravado-core-5.17.0/README.rst
-drwxr-xr-x   0 sjaensch (1475161668) AD\Domain Users (1954207199)        0 2020-04-03 13:21:26.367284 bravado-core-5.17.0/bravado_core/
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)       43 2020-04-03 13:21:15.000000 bravado-core-5.17.0/bravado_core/__init__.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)      676 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/_compat.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)      456 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/_compat_typing.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     3428 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/_decorators.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)       90 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/content_type.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     5289 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/docstring.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     1986 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/exception.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     7541 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/formatter.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    16058 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/marshal.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    35645 2020-04-03 13:11:15.000000 bravado-core-5.17.0/bravado_core/model.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     9718 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/operation.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    14518 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/param.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)        0 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/py.typed
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     2687 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/request.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     6523 2020-04-03 13:11:15.000000 bravado-core-5.17.0/bravado_core/resource.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     8920 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/response.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     8520 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/schema.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     2771 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/security_definition.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     2537 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/security_requirement.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    25804 2020-04-03 13:11:15.000000 bravado-core-5.17.0/bravado_core/spec.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    19039 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/spec_flattening.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    12598 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/swagger20_validator.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    16765 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/unmarshal.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)    10813 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/util.py
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     7466 2020-03-09 08:35:34.000000 bravado-core-5.17.0/bravado_core/validate.py
-drwxr-xr-x   0 sjaensch (1475161668) AD\Domain Users (1954207199)        0 2020-04-03 13:21:26.369347 bravado-core-5.17.0/bravado_core.egg-info/
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)     3993 2020-04-03 13:21:26.000000 bravado-core-5.17.0/bravado_core.egg-info/PKG-INFO
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)      943 2020-04-03 13:21:26.000000 bravado-core-5.17.0/bravado_core.egg-info/SOURCES.txt
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)        1 2020-04-03 13:21:26.000000 bravado-core-5.17.0/bravado_core.egg-info/dependency_links.txt
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)        1 2020-04-03 13:17:55.000000 bravado-core-5.17.0/bravado_core.egg-info/not-zip-safe
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)      223 2020-04-03 13:21:26.000000 bravado-core-5.17.0/bravado_core.egg-info/requires.txt
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)       13 2020-04-03 13:21:26.000000 bravado-core-5.17.0/bravado_core.egg-info/top_level.txt
--rw-r--r--   0 sjaensch (1475161668) AD\Domain Users (1954207199)      106 2020-04-03 13:21:26.370139 bravado-core-5.17.0/setup.cfg
--rwxr-xr-x   0 sjaensch (1475161668) AD\Domain Users (1954207199)     1795 2020-03-09 08:35:34.000000 bravado-core-5.17.0/setup.py
+drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2022-09-02 17:27:10.000000 bravado-core-5.17.1/
+-rw-r--r--   0 bariteau  (3176) users      (100)    28531 2022-09-01 22:21:26.000000 bravado-core-5.17.1/CHANGELOG.rst
+-rw-r--r--   0 bariteau  (3176) users      (100)     1587 2022-09-01 22:21:26.000000 bravado-core-5.17.1/LICENSE.txt
+-rw-r--r--   0 bariteau  (3176) users      (100)       61 2022-09-01 22:21:26.000000 bravado-core-5.17.1/MANIFEST.in
+-rw-r--r--   0 bariteau  (3176) users      (100)     3957 2022-09-02 17:27:10.000000 bravado-core-5.17.1/PKG-INFO
+-rw-r--r--   0 bariteau  (3176) users      (100)     2460 2022-09-01 22:21:26.000000 bravado-core-5.17.1/README.rst
+drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2022-09-02 17:27:10.000000 bravado-core-5.17.1/bravado_core/
+-rw-r--r--   0 bariteau  (3176) users      (100)       43 2022-09-02 17:25:10.000000 bravado-core-5.17.1/bravado_core/__init__.py
+-rw-r--r--   0 bariteau  (3176) users      (100)      676 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/_compat.py
+-rw-r--r--   0 bariteau  (3176) users      (100)      456 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/_compat_typing.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     3428 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/_decorators.py
+-rw-r--r--   0 bariteau  (3176) users      (100)       90 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/content_type.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     5289 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/docstring.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     1986 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/exception.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     7541 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/formatter.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    16058 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/marshal.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    35645 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/model.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     9718 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/operation.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    14518 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/param.py
+-rw-r--r--   0 bariteau  (3176) users      (100)        0 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/py.typed
+-rw-r--r--   0 bariteau  (3176) users      (100)     2687 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/request.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     6523 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/resource.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     8920 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/response.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     8520 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/schema.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     2771 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/security_definition.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     2537 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/security_requirement.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    26681 2022-09-02 17:24:42.000000 bravado-core-5.17.1/bravado_core/spec.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    19039 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/spec_flattening.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    12598 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/swagger20_validator.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    16765 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/unmarshal.py
+-rw-r--r--   0 bariteau  (3176) users      (100)    10813 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/util.py
+-rw-r--r--   0 bariteau  (3176) users      (100)     7466 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/validate.py
+drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2022-09-02 17:27:10.000000 bravado-core-5.17.1/bravado_core.egg-info/
+-rw-r--r--   0 bariteau  (3176) users      (100)     3957 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/PKG-INFO
+-rw-r--r--   0 bariteau  (3176) users      (100)      943 2022-09-02 17:27:10.000000 bravado-core-5.17.1/bravado_core.egg-info/SOURCES.txt
+-rw-r--r--   0 bariteau  (3176) users      (100)        1 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/dependency_links.txt
+-rw-r--r--   0 bariteau  (3176) users      (100)        1 2022-09-01 22:27:29.000000 bravado-core-5.17.1/bravado_core.egg-info/not-zip-safe
+-rw-r--r--   0 bariteau  (3176) users      (100)      232 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/requires.txt
+-rw-r--r--   0 bariteau  (3176) users      (100)       13 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/top_level.txt
+-rw-r--r--   0 bariteau  (3176) users      (100)      106 2022-09-02 17:27:10.000000 bravado-core-5.17.1/setup.cfg
+-rwxr-xr-x   0 bariteau  (3176) users      (100)     1894 2022-09-02 17:24:42.000000 bravado-core-5.17.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bravado-core-5.17.0/CHANGELOG.rst` & `bravado-core-5.17.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/LICENSE.txt` & `bravado-core-5.17.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/PKG-INFO` & `bravado-core-5.17.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: bravado-core
-Version: 5.17.0
+Version: 5.17.1
 Summary: Library for adding Swagger support to clients and servers
 Home-page: https://github.com/Yelp/bravado-core
 Author: Digium, Inc. and Yelp, Inc.
 Author-email: opensource+bravado-core@yelp.com
 License: BSD 3-Clause License
-Description: .. image:: https://img.shields.io/travis/Yelp/bravado-core/master.svg?label=Linux+Build
-          :target: https://travis-ci.org/Yelp/bravado-core?branch=master
+Description: .. image:: https://github.com/Yelp/bravado-core/workflows/build/badge.svg?branch=master
+          :target: https://github.com/Yelp/bravado-core/actions?query=workflow%3Abuild
         
         .. image:: https://img.shields.io/coveralls/Yelp/bravado-core.svg
           :target: https://coveralls.io/r/Yelp/bravado-core
         
         .. image:: https://img.shields.io/pypi/v/bravado-core.svg
             :target: https://pypi.python.org/pypi/bravado-core/
             :alt: PyPi version
@@ -98,11 +98,10 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: !=3.0,!=3.1,!=3.2,!=3.3,!=3.4,!=3.5.0
```

### Comparing `bravado-core-5.17.0/README.rst` & `bravado-core-5.17.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.. image:: https://img.shields.io/travis/Yelp/bravado-core/master.svg?label=Linux+Build
-  :target: https://travis-ci.org/Yelp/bravado-core?branch=master
+.. image:: https://github.com/Yelp/bravado-core/workflows/build/badge.svg?branch=master
+  :target: https://github.com/Yelp/bravado-core/actions?query=workflow%3Abuild
 
 .. image:: https://img.shields.io/coveralls/Yelp/bravado-core.svg
   :target: https://coveralls.io/r/Yelp/bravado-core
 
 .. image:: https://img.shields.io/pypi/v/bravado-core.svg
     :target: https://pypi.python.org/pypi/bravado-core/
     :alt: PyPi version
```

### Comparing `bravado-core-5.17.0/bravado_core/_compat.py` & `bravado-core-5.17.1/bravado_core/_compat.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/_decorators.py` & `bravado-core-5.17.1/bravado_core/_decorators.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/docstring.py` & `bravado-core-5.17.1/bravado_core/docstring.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/exception.py` & `bravado-core-5.17.1/bravado_core/exception.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/formatter.py` & `bravado-core-5.17.1/bravado_core/formatter.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/marshal.py` & `bravado-core-5.17.1/bravado_core/marshal.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/model.py` & `bravado-core-5.17.1/bravado_core/model.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/operation.py` & `bravado-core-5.17.1/bravado_core/operation.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/param.py` & `bravado-core-5.17.1/bravado_core/param.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/request.py` & `bravado-core-5.17.1/bravado_core/request.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/resource.py` & `bravado-core-5.17.1/bravado_core/resource.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/response.py` & `bravado-core-5.17.1/bravado_core/response.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/schema.py` & `bravado-core-5.17.1/bravado_core/schema.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/security_definition.py` & `bravado-core-5.17.1/bravado_core/security_definition.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/security_requirement.py` & `bravado-core-5.17.1/bravado_core/security_requirement.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/spec.py` & `bravado-core-5.17.1/bravado_core/spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 import json
 import logging
 import os.path
 import warnings
 from copy import deepcopy
 from itertools import chain
 
+import requests
 import typing
 import yaml
 from jsonref import JsonRef
 from jsonschema import FormatChecker
 from jsonschema.validators import RefResolver
 from six import iteritems
 from six import iterkeys
 from six.moves import range
 from six.moves.urllib.parse import urlparse
 from six.moves.urllib.parse import urlunparse
 from six.moves.urllib.request import url2pathname
 from swagger_spec_validator import validator20
 from swagger_spec_validator.ref_validators import in_scope
 
+try:
+    from yaml import CSafeLoader as SafeLoader
+except ImportError:
+    from yaml import SafeLoader  # type: ignore
+
 from bravado_core import formatter
 from bravado_core import version as _version
 from bravado_core.exception import SwaggerSchemaError
 from bravado_core.exception import SwaggerValidationError
 from bravado_core.formatter import return_true_wrapper
 from bravado_core.model import _from_pickleable_representation
 from bravado_core.model import _to_pickleable_representation
@@ -116,15 +122,15 @@
 
     def __init__(
         self, spec_dict, origin_url=None, http_client=None,
         config=None,
     ):
         self.spec_dict = spec_dict
         self.origin_url = origin_url
-        self.http_client = http_client
+        self.http_client = http_client or BasicHTTPClient()
         self.api_url = None
         self.config = dict(CONFIG_DEFAULTS, **(config or {}))
 
         # (key, value) = (simple format def name, Model type)
         # (key, value) = (#/ format def ref, Model type)
         self.definitions = {}
 
@@ -181,14 +187,15 @@
         # all the attributes.
         for attr_name in set(chain(iterkeys(self.__dict__), iterkeys(other.__dict__))):
             # Some attributes do not define equality methods.
             # As those attributes are defined internally only we do not expect that users of the library are modifying them.
             if attr_name in {
                 'format_checker',   # jsonschema.FormatChecker does not define an equality method
                 'resolver',         # jsonschema.validators.RefResolver does not define an equality method
+                'http_client',      # this attribute may be different for the same values
             }:
                 continue
 
             # In case of fully dereferenced specs _deref_flattened_spec (and consequently _internal_spec_dict) will contain
             # recursive reference to objects. Python is not capable of comparing them (weird).
             # As _internal_spec_dict and _deref_flattened_spec are private so we don't expect users modifying them.
             if self.config['internally_dereference_refs'] and attr_name in {
@@ -543,14 +550,31 @@
     _, ext = os.path.splitext(url)
     if ext.lower() in yaml_file_extensions:
         return True
 
     return False
 
 
+# this has the minimal interface required for build_http_handlers, but should be
+# more or less compatible with bravado.http_future.HttpFuture
+class BasicHTTPFuture(object):
+    def __init__(self, request_params):
+        self.request_params = request_params
+
+    def result(self):
+        return requests.request(**self.request_params)
+
+
+# this has the minimal interface required for build_http_handlers, but should be
+# more or less compatible with bravado.http_client.HttpClient
+class BasicHTTPClient(object):
+    def request(self, request_params):
+        return BasicHTTPFuture(request_params)
+
+
 def build_http_handlers(http_client):
     """Create a mapping of uri schemes to callables that take a uri. The
     callable is used by jsonschema's RefResolver to download remote $refs.
 
     :param http_client: http_client with a request() method
 
     :returns: dict like {'http': callable, 'https': callable}
@@ -560,22 +584,22 @@
         request_params = {
             'method': 'GET',
             'url': uri,
         }
         response = http_client.request(request_params).result()
         content_type = response.headers.get('content-type', '').lower()
         if is_yaml(uri, content_type):
-            return yaml.safe_load(response.content)
+            return yaml.load(response.content, Loader=SafeLoader)
         else:
             return response.json()
 
     def read_file(uri):
         with open(url2pathname(urlparse(uri).path), mode='rb') as fp:
             if is_yaml(uri):
-                return yaml.safe_load(fp)
+                return yaml.load(fp, Loader=SafeLoader)
             else:
                 return json.loads(fp.read().decode("utf-8"))
 
     return {
         'http': download,
         'https': download,
         # jsonschema ordinarily handles file:// requests, but it assumes that
```

### Comparing `bravado-core-5.17.0/bravado_core/spec_flattening.py` & `bravado-core-5.17.1/bravado_core/spec_flattening.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/swagger20_validator.py` & `bravado-core-5.17.1/bravado_core/swagger20_validator.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/unmarshal.py` & `bravado-core-5.17.1/bravado_core/unmarshal.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/util.py` & `bravado-core-5.17.1/bravado_core/util.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core/validate.py` & `bravado-core-5.17.1/bravado_core/validate.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/bravado_core.egg-info/PKG-INFO` & `bravado-core-5.17.1/bravado_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: bravado-core
-Version: 5.17.0
+Version: 5.17.1
 Summary: Library for adding Swagger support to clients and servers
 Home-page: https://github.com/Yelp/bravado-core
 Author: Digium, Inc. and Yelp, Inc.
 Author-email: opensource+bravado-core@yelp.com
 License: BSD 3-Clause License
-Description: .. image:: https://img.shields.io/travis/Yelp/bravado-core/master.svg?label=Linux+Build
-          :target: https://travis-ci.org/Yelp/bravado-core?branch=master
+Description: .. image:: https://github.com/Yelp/bravado-core/workflows/build/badge.svg?branch=master
+          :target: https://github.com/Yelp/bravado-core/actions?query=workflow%3Abuild
         
         .. image:: https://img.shields.io/coveralls/Yelp/bravado-core.svg
           :target: https://coveralls.io/r/Yelp/bravado-core
         
         .. image:: https://img.shields.io/pypi/v/bravado-core.svg
             :target: https://pypi.python.org/pypi/bravado-core/
             :alt: PyPi version
@@ -98,11 +98,10 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: !=3.0,!=3.1,!=3.2,!=3.3,!=3.4,!=3.5.0
```

### Comparing `bravado-core-5.17.0/bravado_core.egg-info/SOURCES.txt` & `bravado-core-5.17.1/bravado_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.0/setup.py` & `bravado-core-5.17.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013, Digium, Inc.
 # Copyright (c) 2014-2015, Yelp, Inc.
 import os
+import sys
 
 from setuptools import setup
 
 import bravado_core
 
+install_requires = [
+    "jsonref",
+    "jsonschema[format]>=2.5.1",
+    "python-dateutil",
+    "pyyaml",
+    'requests',
+    "simplejson",
+    "six",
+    "swagger-spec-validator>=2.0.1",
+    "pytz",
+    "msgpack>=0.5.2",
+]
+
+# pyrsistent dropped python2 support in 0.17.0
+if sys.version_info < (3, 5):
+    install_requires.append('pyrsistent<0.17')
 
 setup(
     name="bravado-core",
     version=bravado_core.version,
     license="BSD 3-Clause License",
     description="Library for adding Swagger support to clients and servers",
     long_description=open(
@@ -27,29 +44,18 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
-    install_requires=[
-        "jsonref",
-        "jsonschema[format]>=2.5.1",
-        "python-dateutil",
-        "pyyaml",
-        "simplejson",
-        "six",
-        "swagger-spec-validator>=2.0.1",
-        "pytz",
-        "msgpack>=0.5.2",
-    ],
+    install_requires=install_requires,
     package_data={
         'bravado_core': ['py.typed'],
     },
     # https://mypy.readthedocs.io/en/latest/installed_packages.html
     zip_safe=False,
     extras_require={
         ':python_version<"3.5"': ['typing'],
```

