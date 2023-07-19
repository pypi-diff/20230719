# Comparing `tmp/event-processor-3.2.0.tar.gz` & `tmp/event-processor-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event-processor-3.2.0.tar", last modified: Tue Dec 13 18:29:38 2022, max compression
+gzip compressed data, was "event-processor-3.2.1.tar", last modified: Wed Jul 19 03:34:32 2023, max compression
```

## Comparing `event-processor-3.2.0.tar` & `event-processor-3.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:38.265596 event-processor-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-13 18:29:19.000000 event-processor-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-13 18:29:19.000000 event-processor-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2022-12-13 18:29:38.265596 event-processor-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2022-12-13 18:29:19.000000 event-processor-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-13 18:29:37.000000 event-processor-3.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 18:29:38.265596 event-processor-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2022-12-13 18:29:19.000000 event-processor-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:38.261596 event-processor-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:38.265596 event-processor-3.2.0/src/event_processor/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/error_handling_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/invocation_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/event_processor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:38.265596 event-processor-3.2.0/src/event_processor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2022-12-13 18:29:38.000000 event-processor-3.2.0/src/event_processor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-13 18:29:38.000000 event-processor-3.2.0/src/event_processor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 18:29:38.000000 event-processor-3.2.0/src/event_processor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-13 18:29:38.000000 event-processor-3.2.0/src/event_processor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 18:29:38.000000 event-processor-3.2.0/src/event_processor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 18:29:38.000000 event-processor-3.2.0/src/event_processor.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:38.265596 event-processor-3.2.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:38.265596 event-processor-3.2.0/src/tests/package_for_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/package_for_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/package_for_tests/a_module.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/package_for_tests/b_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_error_handling_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_event_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_invocation_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-13 18:29:19.000000 event-processor-3.2.0/src/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:32.101265 event-processor-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 03:34:07.000000 event-processor-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 03:34:07.000000 event-processor-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-19 03:34:32.101265 event-processor-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-19 03:34:07.000000 event-processor-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 03:34:30.000000 event-processor-3.2.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 03:34:32.101265 event-processor-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-19 03:34:07.000000 event-processor-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:32.097265 event-processor-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:32.101265 event-processor-3.2.1/src/event_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/error_handling_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/invocation_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/event_processor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:32.101265 event-processor-3.2.1/src/event_processor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-19 03:34:32.000000 event-processor-3.2.1/src/event_processor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-19 03:34:32.000000 event-processor-3.2.1/src/event_processor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:34:32.000000 event-processor-3.2.1/src/event_processor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 03:34:32.000000 event-processor-3.2.1/src/event_processor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 03:34:32.000000 event-processor-3.2.1/src/event_processor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:34:32.000000 event-processor-3.2.1/src/event_processor.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:32.101265 event-processor-3.2.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:32.101265 event-processor-3.2.1/src/tests/package_for_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/package_for_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/package_for_tests/a_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/package_for_tests/b_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_error_handling_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_invocation_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-19 03:34:07.000000 event-processor-3.2.1/src/tests/test_util.py
```

### Comparing `event-processor-3.2.0/LICENSE` & `event-processor-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/PKG-INFO` & `event-processor-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-processor
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pythonic event-processing library based on decorators
 Home-page: https://github.com/marier-nico/event-processor
 Author: Nicolas Marier
 Author-email: software@nmarier.com
 License: UNKNOWN
 Project-URL: Documentation, https://event-processor.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/marier-nico/event-processor
```

### Comparing `event-processor-3.2.0/README.md` & `event-processor-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/setup.py` & `event-processor-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,14 @@
     ],
     keywords="event decorators development",
 
     # Packages and depencies
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     install_requires=[],
-    extras_require={"pydantic": ["pydantic >= 1.8.2,< 2.0"]},
+    extras_require={"pydantic": ["pydantic >= 1.8.2,< 3.0"]},
     package_data={"": ["VERSION"], "event_processor": ["py.typed"]},
 
     # Other configurations
     zip_safe=True,
     platforms="any",
 )
```

### Comparing `event-processor-3.2.0/src/event_processor/dependencies.py` & `event-processor-3.2.1/src/event_processor/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     _has_pydantic = True
 except ImportError:  # pragma: no cover
     _has_pydantic = False
 
 try:
     from typing import get_args, get_origin  # type: ignore
 except ImportError:  # pragma: no cover
-    from src.event_processor.util import py37_get_origin as get_origin
+    from src.event_processor.util import py37_get_origin as get_origin  # type: ignore
     from src.event_processor.util import py37_get_args as get_args
 
 
 DependsReturn = typing.TypeVar("DependsReturn")
 
 
 class Event(dict):
```

### Comparing `event-processor-3.2.0/src/event_processor/error_handling_strategies.py` & `event-processor-3.2.1/src/event_processor/error_handling_strategies.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor/event_processor.py` & `event-processor-3.2.1/src/event_processor/event_processor.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor/exceptions.py` & `event-processor-3.2.1/src/event_processor/exceptions.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor/filters.py` & `event-processor-3.2.1/src/event_processor/filters.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor/invocation_strategies.py` & `event-processor-3.2.1/src/event_processor/invocation_strategies.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor/result.py` & `event-processor-3.2.1/src/event_processor/result.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor/util.py` & `event-processor-3.2.1/src/event_processor/util.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/event_processor.egg-info/PKG-INFO` & `event-processor-3.2.1/src/event_processor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-processor
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pythonic event-processing library based on decorators
 Home-page: https://github.com/marier-nico/event-processor
 Author: Nicolas Marier
 Author-email: software@nmarier.com
 License: UNKNOWN
 Project-URL: Documentation, https://event-processor.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/marier-nico/event-processor
```

### Comparing `event-processor-3.2.0/src/event_processor.egg-info/SOURCES.txt` & `event-processor-3.2.1/src/event_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_dependencies.py` & `event-processor-3.2.1/src/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_end_to_end.py` & `event-processor-3.2.1/src/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_error_handling_strategies.py` & `event-processor-3.2.1/src/tests/test_error_handling_strategies.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_event_processor.py` & `event-processor-3.2.1/src/tests/test_event_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         pass
 
     assert len(event_processor.processors) == 1
     assert len(event_processor.processors[Accept(), 0]) == 2
 
 
 def test_processor_raises_exception_when_the_processor_takes_invalid_params(event_processor):
-
     with pytest.raises(FilterError):
 
         @event_processor.processor(Accept())
         def fn(*_args):
             pass
 
 
@@ -148,15 +147,14 @@
     event_processor.invoke({"a": 0, "b": 0})
     event_processor.invoke({"a": 0, "b": 0})
     assert a_calls == 2
     assert b_calls == 2
 
 
 def test_invoke_raises_for_no_matching_processors(event_processor):
-
     with pytest.raises(InvocationError):
         event_processor.invoke({"a": 0})
 
 
 def test_invoke_returns_the_processor_return_value(event_processor):
     result_mock = Mock()
     event_processor.processors[Accept(), 0] = [lambda: result_mock]
```

### Comparing `event-processor-3.2.0/src/tests/test_filters.py` & `event-processor-3.2.1/src/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_invocation_strategies.py` & `event-processor-3.2.1/src/tests/test_invocation_strategies.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_result.py` & `event-processor-3.2.1/src/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `event-processor-3.2.0/src/tests/test_util.py` & `event-processor-3.2.1/src/tests/test_util.py`

 * *Files identical despite different names*

