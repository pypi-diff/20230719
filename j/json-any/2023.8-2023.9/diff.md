# Comparing `tmp/json-any-2023.8.tar.gz` & `tmp/json-any-2023.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.8.tar", last modified: Tue Jul 18 10:02:17 2023, max compression
+gzip compressed data, was "json-any-2023.9.tar", last modified: Wed Jul 19 10:28:55 2023, max compression
```

## Comparing `json-any-2023.8.tar` & `json-any-2023.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.8/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4780 2023-07-18 10:02:17.239552 json-any-2023.8/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.8/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     4018 2023-07-17 12:03:11.000000 json-any-2023.8/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.236219 json-any-2023.8/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.8/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.8/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.8/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     5042 2023-07-17 12:17:06.000000 json-any-2023.8/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.8/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/extension/
--rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.8/json_any/extension/module.py
--rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.8/json_any/extension/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)     3306 2023-07-18 09:13:52.000000 json-any-2023.8/json_any/extension/type.py
--rw-r--r--   0 eric      (1000) users      (984)    11694 2023-07-18 09:14:44.000000 json-any-2023.8/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)    12906 2023-07-18 09:15:09.000000 json-any-2023.8/json_any/object_to_json.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/task/
--rw-r--r--   0 eric      (1000) users      (984)     3348 2023-07-17 07:04:05.000000 json-any-2023.8/json_any/task/compression.py
--rw-r--r--   0 eric      (1000) users      (984)     8258 2023-07-17 09:48:29.000000 json-any-2023.8/json_any/task/storage.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-17 12:24:04.000000 json-any-2023.8/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4780 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.8/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-18 10:02:17.239552 json-any-2023.8/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.8/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.364717 json-any-2023.9/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.9/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4780 2023-07-19 10:28:55.364717 json-any-2023.9/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.9/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     4018 2023-07-17 12:03:11.000000 json-any-2023.9/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.361383 json-any-2023.9/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.361383 json-any-2023.9/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.9/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.364717 json-any-2023.9/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.9/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.364717 json-any-2023.9/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.9/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     5167 2023-07-19 10:18:42.000000 json-any-2023.9/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.9/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.364717 json-any-2023.9/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.9/json_any/extension/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.9/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     3306 2023-07-18 09:13:52.000000 json-any-2023.9/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)    11933 2023-07-19 10:20:33.000000 json-any-2023.9/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    13243 2023-07-19 10:19:52.000000 json-any-2023.9/json_any/object_to_json.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.364717 json-any-2023.9/json_any/task/
+-rw-r--r--   0 eric      (1000) users      (984)     3348 2023-07-17 07:04:05.000000 json-any-2023.9/json_any/task/compression.py
+-rw-r--r--   0 eric      (1000) users      (984)     8258 2023-07-17 09:48:29.000000 json-any-2023.9/json_any/task/storage.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-19 10:26:23.000000 json-any-2023.9/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-19 10:28:55.364717 json-any-2023.9/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4780 2023-07-19 10:28:55.000000 json-any-2023.9/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-19 10:28:55.000000 json-any-2023.9/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-19 10:28:55.000000 json-any-2023.9/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-19 10:28:55.000000 json-any-2023.9/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.9/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-19 10:28:55.364717 json-any-2023.9/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.9/setup.py
```

### Comparing `json-any-2023.8/PKG-INFO` & `json-any-2023.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.8
+Version: 2023.9
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.8/README-LICENCE-utf8.txt` & `json-any-2023.9/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/README.rst` & `json-any-2023.9/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/documentation/wiki/description.asciidoc` & `json-any-2023.9/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/__init__.py` & `json-any-2023.9/json_any/__init__.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/catalog/module.py` & `json-any-2023.9/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/catalog/type.py` & `json-any-2023.9/json_any/catalog/type.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 
 from array import array as py_array_t
 from datetime import date as date_t
 from datetime import datetime as date_time_t
 from datetime import time as time_t
 from datetime import timedelta as time_delta_t
 from datetime import timezone as time_zone_t
+from decimal import Decimal as decimal_t
 from enum import Enum as enum_t
+from fractions import Fraction as fraction_t
 from io import BytesIO as io_bytes_t
 from io import StringIO as io_string_t
 from pathlib import PurePath as path_t
 from typing import Any
 from typing import NamedTuple as named_tuple_t
 from typing import Sequence
 from uuid import UUID as uuid_t
@@ -88,15 +90,17 @@
         JSON_TYPE[type_] = f"{type_.__module__}{MODULE_TYPE_SEPARATOR}{type_.__name__}"
 
 
 _AddJsonTypes(
     (
         date_t,
         date_time_t,
+        decimal_t,
         enum_t,
+        fraction_t,
         io_bytes_t,
         io_string_t,
         named_tuple_t,
         py_array_t,
         time_delta_t,
         time_t,
         time_zone_t,
```

### Comparing `json-any-2023.8/json_any/constant.py` & `json-any-2023.9/json_any/constant.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/extension/module.py` & `json-any-2023.9/json_any/extension/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/extension/numpy.py` & `json-any-2023.9/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/extension/type.py` & `json-any-2023.9/json_any/extension/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/json_to_object.py` & `json-any-2023.9/json_any/json_to_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     JSON_TYPE_NUMPY_SCALAR,
     JSON_TYPE_PREFIX_PATHLIB,
     ContainerWithName,
     TypeIsInModule,
     TypeNameOf,
     date_t,
     date_time_t,
+    decimal_t,
     enum_t,
+    fraction_t,
     io_bytes_t,
     io_string_t,
     named_tuple_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
@@ -169,14 +171,18 @@
         output = slice(*instance)
     elif json_type == JSON_TYPE[uuid_t]:
         output = uuid_t(int=instance)
     elif json_type == JSON_TYPE[date_t]:
         output = date_t(*instance)
     elif json_type == JSON_TYPE[time_delta_t]:
         output = time_delta_t(*instance)
+    elif json_type == JSON_TYPE[decimal_t]:
+        output = decimal_t(value=instance)
+    elif json_type == JSON_TYPE[fraction_t]:
+        output = fraction_t(numerator=instance[0], denominator=instance[1])
     elif json_type == JSON_TYPE[py_array_t]:
         as_list, typecode = instance
         output = py_array_t(typecode)
         output.fromlist(as_list)
     elif json_type == JSON_TYPE[io_bytes_t]:
         output = io_bytes_t(initial_bytes=instance.encode(encoding="iso-8859-1"))
     elif json_type == JSON_TYPE[io_string_t]:
```

### Comparing `json-any-2023.8/json_any/object_to_json.py` & `json-any-2023.9/json_any/object_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,17 @@
     MATPLOTLIB_CLASSES,
     NETWORKX_CLASSES,
     NUMPY_ARRAY_CLASSES,
     PANDAS_CLASSES,
     SCIPY_ARRAY_CLASSES,
     date_t,
     date_time_t,
+    decimal_t,
     enum_t,
+    fraction_t,
     io_bytes_t,
     io_string_t,
     named_tuple_t,
     path_t,
     py_array_t,
     time_delta_t,
     time_t,
@@ -173,14 +175,20 @@
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is date_t:
         jsonable = (instance.year, instance.month, instance.day)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is time_delta_t:
         jsonable = (instance.days, instance.seconds, instance.microseconds)
         history.append(f"{history_level}{json_type}:{jsonable}")
+    elif instance_type is decimal_t:
+        jsonable = instance.as_tuple()
+        history.append(f"{history_level}{json_type}:{jsonable}")
+    elif instance_type is fraction_t:
+        jsonable = (instance.numerator, instance.denominator)
+        history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is py_array_t:
         jsonable = (instance.tolist(), instance.typecode)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is io_bytes_t:
         # Buffer is assumed to be open (i.e. no instance.closed check).
         jsonable = instance.getvalue().decode(encoding="iso-8859-1")
         history.append(f"{history_level}{json_type}:{jsonable}")
```

### Comparing `json-any-2023.8/json_any/task/compression.py` & `json-any-2023.9/json_any/task/compression.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/task/storage.py` & `json-any-2023.9/json_any/task/storage.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/json_any/version.py` & `json-any-2023.9/json_any/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.8"
+__version__ = "2023.9"
```

### Comparing `json-any-2023.8/json_any.egg-info/PKG-INFO` & `json-any-2023.9/json_any.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.8
+Version: 2023.9
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.8/json_any.egg-info/SOURCES.txt` & `json-any-2023.9/json_any.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.8/setup.py` & `json-any-2023.9/setup.py`

 * *Files identical despite different names*

