# Comparing `tmp/portion-2.4.0.tar.gz` & `tmp/portion-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portion-2.4.0.tar", last modified: Mon Mar 13 16:11:59 2023, max compression
+gzip compressed data, was "portion-2.4.1.tar", last modified: Wed Jul 19 07:30:19 2023, max compression
```

## Comparing `portion-2.4.0.tar` & `portion-2.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:11:59.395044 portion-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-03-13 16:11:45.000000 portion-2.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-03-13 16:11:59.395044 portion-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32367 2023-03-13 16:11:45.000000 portion-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:11:59.395044 portion-2.4.0/portion/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-13 16:11:45.000000 portion-2.4.0/portion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-13 16:11:45.000000 portion-2.4.0/portion/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-13 16:11:45.000000 portion-2.4.0/portion/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-03-13 16:11:45.000000 portion-2.4.0/portion/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-03-13 16:11:45.000000 portion-2.4.0/portion/func.py
--rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-03-13 16:11:45.000000 portion-2.4.0/portion/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-03-13 16:11:45.000000 portion-2.4.0/portion/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:11:59.395044 portion-2.4.0/portion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-03-13 16:11:59.000000 portion-2.4.0/portion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-13 16:11:59.000000 portion-2.4.0/portion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 16:11:59.000000 portion-2.4.0/portion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-13 16:11:59.000000 portion-2.4.0/portion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 16:11:59.000000 portion-2.4.0/portion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 16:11:59.000000 portion-2.4.0/portion.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-13 16:11:45.000000 portion-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 16:11:59.395044 portion-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-13 16:11:45.000000 portion-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:11:59.395044 portion-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    31018 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-03-13 16:11:45.000000 portion-2.4.0/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:19.318216 portion-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-19 07:30:02.000000 portion-2.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-07-19 07:30:19.318216 portion-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32367 2023-07-19 07:30:02.000000 portion-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:19.314216 portion-2.4.1/portion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-19 07:30:02.000000 portion-2.4.1/portion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-19 07:30:02.000000 portion-2.4.1/portion/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-19 07:30:02.000000 portion-2.4.1/portion/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-19 07:30:02.000000 portion-2.4.1/portion/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-19 07:30:02.000000 portion-2.4.1/portion/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-07-19 07:30:02.000000 portion-2.4.1/portion/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-19 07:30:02.000000 portion-2.4.1/portion/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:19.318216 portion-2.4.1/portion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-07-19 07:30:19.000000 portion-2.4.1/portion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-19 07:30:19.000000 portion-2.4.1/portion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:30:19.000000 portion-2.4.1/portion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-19 07:30:19.000000 portion-2.4.1/portion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 07:30:19.000000 portion-2.4.1/portion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:30:19.000000 portion-2.4.1/portion.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-19 07:30:02.000000 portion-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:30:19.318216 portion-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-19 07:30:02.000000 portion-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:30:19.318216 portion-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31393 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-19 07:30:02.000000 portion-2.4.1/tests/test_io.py
```

### Comparing `portion-2.4.0/LICENSE.txt` & `portion-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/PKG-INFO` & `portion-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portion
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python data structure and operations for intervals
 Home-page: https://github.com/AlexandreDecan/portion
 Author: Alexandre Decan
 License: LGPLv3
 Keywords: interval operation range math
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portion-2.4.0/README.md` & `portion-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion/__init__.py` & `portion-2.4.1/portion/__init__.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion/api.py` & `portion-2.4.1/portion/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import importlib
+import importlib.util
 
 from .const import Bound, inf
 from .func import iterate, open, closed, openclosed, closedopen, empty, singleton
 from .io import from_string, to_string, from_data, to_data
 from .dict import IntervalDict
```

### Comparing `portion-2.4.0/portion/const.py` & `portion-2.4.1/portion/const.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion/dict.py` & `portion-2.4.1/portion/dict.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion/func.py` & `portion-2.4.1/portion/func.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion/interval.py` & `portion-2.4.1/portion/interval.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion/io.py` & `portion-2.4.1/portion/io.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/portion.egg-info/PKG-INFO` & `portion-2.4.1/portion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portion
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python data structure and operations for intervals
 Home-page: https://github.com/AlexandreDecan/portion
 Author: Alexandre Decan
 License: LGPLv3
 Keywords: interval operation range math
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portion-2.4.0/setup.py` & `portion-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="portion",
-    version="2.4.0",
+    version="2.4.1",
     license="LGPLv3",
     author="Alexandre Decan",
     url="https://github.com/AlexandreDecan/portion",
     description="Python data structure and operations for intervals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `portion-2.4.0/tests/test_const.py` & `portion-2.4.1/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/tests/test_dict.py` & `portion-2.4.1/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/tests/test_discrete.py` & `portion-2.4.1/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/tests/test_doc.py` & `portion-2.4.1/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/tests/test_func.py` & `portion-2.4.1/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `portion-2.4.0/tests/test_interval.py` & `portion-2.4.1/tests/test_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,18 @@
         assert not (P.empty() >= P.closedopen(0, P.inf))
 
         assert not (P.closedopen(0, P.inf) < P.empty())
         assert not (P.closedopen(0, P.inf) > P.empty())
         assert not (P.closedopen(0, P.inf) <= P.empty())
         assert not (P.closedopen(0, P.inf) >= P.empty())
 
+    def test_edge_cases(self):
+        assert not (P.closed(0, 2) >= P.open(0, 1))
+        assert not (P.closed(0, 2) >= P.openclosed(0, 1))
+
     def test_with_values(self):
         with pytest.deprecated_call():
             assert 0 < P.closed(1, 2)
 
         with pytest.deprecated_call():
             assert not (0 < P.closed(-1, 1))
 
@@ -504,17 +508,20 @@
         assert P.open(1, 2) in P.closed(1, 2)
         assert P.closed(1, 2) not in P.open(1, 2)
         assert P.closed(0, 1) not in P.closed(1, 2)
         assert P.closed(0, 2) not in P.closed(1, 3)
         assert P.closed(-P.inf, P.inf) in P.closed(-P.inf, P.inf)
         assert P.closed(0, 1) in P.closed(-P.inf, P.inf)
         assert P.closed(-P.inf, P.inf) not in P.closed(0, 1)
+        assert P.singleton(0) | P.singleton(5) in P.closed(0, 5)
+        assert P.singleton(0) | P.singleton(5) in P.closed(0, 1) | P.closed(4, 5)
 
         # https://github.com/AlexandreDecan/portion/issues/28
         assert P.closed(5, 6) not in P.closed(1, 2) | P.closed(3, 4)
+        assert P.singleton(0) | P.singleton(6) not in P.closed(0, 1) | P.closed(4, 5)
 
     def test_with_unions(self):
         assert P.closed(0, 1) | P.closed(2, 3) in P.closed(0, 4)
         assert P.closed(0, 1) | P.closed(2, 3) in P.closed(0, 1) | P.closed(2, 3)
         assert P.closed(0, 1) | P.closed(2, 3) in P.closed(0, 0) | P.closed(0, 1) | P.closed(2, 3)
 
         assert P.closed(0, 1) | P.closed(2, 3) not in P.closed(0, 2)
```

### Comparing `portion-2.4.0/tests/test_io.py` & `portion-2.4.1/tests/test_io.py`

 * *Files identical despite different names*

