# Comparing `tmp/rom-1.0.6.tar.gz` & `tmp/rom-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rom-1.0.6.tar", last modified: Wed May  3 04:05:06 2023, max compression
+gzip compressed data, was "dist/rom-1.0.7.tar", last modified: Sun Jul  2 23:38:18 2023, max compression
```

## Comparing `rom-1.0.6.tar` & `rom-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)        5 2023-05-03 03:40:57.000000 rom-1.0.6/VERSION
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)      328 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/SOURCES.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)        1 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/dependency_links.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       10 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/requires.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       47 2018-09-26 03:30:44.000000 rom-1.0.6/rom.egg-info/pbr.json
--rw-rw-r--   0 josiah    (1000) josiah    (1000)        4 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/top_level.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     8585 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/PKG-INFO
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     8585 2023-05-03 04:05:06.000000 rom-1.0.6/PKG-INFO
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     1300 2022-11-05 00:00:22.000000 rom-1.0.6/setup.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     6229 2023-05-03 03:40:37.000000 rom-1.0.6/README.rst
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       35 2018-09-26 03:27:59.000000 rom-1.0.6/MANIFEST.in
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       38 2023-05-03 04:05:06.000000 rom-1.0.6/setup.cfg
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/rom/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    28748 2023-05-03 03:40:37.000000 rom-1.0.6/rom/query.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    36133 2023-05-03 03:40:37.000000 rom-1.0.6/rom/util.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     8063 2023-05-03 03:40:57.000000 rom-1.0.6/rom/__init__.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     1743 2023-05-03 04:04:46.000000 rom-1.0.6/rom/exceptions.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)    19323 2020-07-12 04:36:14.000000 rom-1.0.6/rom/index.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     6975 2021-08-20 01:25:13.000000 rom-1.0.6/rom/wrappers.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    36972 2023-05-03 04:04:46.000000 rom-1.0.6/rom/columns.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    44929 2023-05-03 04:04:46.000000 rom-1.0.6/rom/model.py
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/test/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    74178 2023-05-03 03:40:57.000000 rom-1.0.6/test/test_rom.py
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-07-02 23:38:17.000000 rom-1.0.7/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       38 2023-07-02 23:38:17.000000 rom-1.0.7/setup.cfg
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     8585 2023-07-02 23:38:17.000000 rom-1.0.7/PKG-INFO
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     1300 2022-11-05 00:00:22.000000 rom-1.0.7/setup.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       35 2018-09-26 03:27:59.000000 rom-1.0.7/MANIFEST.in
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-07-02 23:38:17.000000 rom-1.0.7/test/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    74178 2023-05-03 03:40:57.000000 rom-1.0.7/test/test_rom.py
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-07-02 23:38:17.000000 rom-1.0.7/rom.egg-info/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       10 2023-07-02 23:38:17.000000 rom-1.0.7/rom.egg-info/requires.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)      328 2023-07-02 23:38:17.000000 rom-1.0.7/rom.egg-info/SOURCES.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       47 2018-09-26 03:30:44.000000 rom-1.0.7/rom.egg-info/pbr.json
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     8585 2023-07-02 23:38:17.000000 rom-1.0.7/rom.egg-info/PKG-INFO
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        1 2023-07-02 23:38:17.000000 rom-1.0.7/rom.egg-info/dependency_links.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        4 2023-07-02 23:38:17.000000 rom-1.0.7/rom.egg-info/top_level.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     6229 2023-07-02 23:35:32.000000 rom-1.0.7/README.rst
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        5 2023-07-02 23:35:32.000000 rom-1.0.7/VERSION
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-07-02 23:38:17.000000 rom-1.0.7/rom/
+-rw-r--r--   0 josiah    (1000) josiah    (1000)    19323 2020-07-12 04:36:14.000000 rom-1.0.7/rom/index.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     8063 2023-07-02 23:33:48.000000 rom-1.0.7/rom/__init__.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    36133 2023-05-03 03:40:37.000000 rom-1.0.7/rom/util.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    45395 2023-07-02 23:32:51.000000 rom-1.0.7/rom/model.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    36972 2023-05-03 04:04:46.000000 rom-1.0.7/rom/columns.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     6975 2021-08-20 01:25:13.000000 rom-1.0.7/rom/wrappers.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    28748 2023-05-03 03:40:37.000000 rom-1.0.7/rom/query.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     1743 2023-05-03 04:04:46.000000 rom-1.0.7/rom/exceptions.py
```

### Comparing `rom-1.0.6/rom.egg-info/PKG-INFO` & `rom-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rom
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Redis object mapper for Python
 Home-page: https://github.com/josiahcarlson/rom
 Author: Josiah Carlson
 Author-email: josiah.carlson@gmail.com
 License: GNU LGPL v2.1
 Description: 
         Rom - the Redis object mapper for Python
```

### Comparing `rom-1.0.6/PKG-INFO` & `rom-1.0.7/rom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rom
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Redis object mapper for Python
 Home-page: https://github.com/josiahcarlson/rom
 Author: Josiah Carlson
 Author-email: josiah.carlson@gmail.com
 License: GNU LGPL v2.1
 Description: 
         Rom - the Redis object mapper for Python
```

### Comparing `rom-1.0.6/setup.py` & `rom-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/README.rst` & `rom-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/query.py` & `rom-1.0.7/rom/query.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/util.py` & `rom-1.0.7/rom/util.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/__init__.py` & `rom-1.0.7/rom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 from .index import GeneralIndex, GeoIndex, Pattern, Prefix, Suffix
 from .model import _ModelMetaclass, Model
 from .query import NOT_NULL, Query
 from .util import (ClassProperty, _connect, session,
     _prefix_score, _script_load, _encode_unique_constraint,
     FULL_TEXT, CASE_INSENSITIVE, SIMPLE, SIMPLE_CI, IDENTITY, IDENTITY_CI)
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 COLUMN_TYPES = [Column, Integer, Boolean, Float, Decimal, DateTime, Date,
 Time, String, Text, Json, PrimaryKey, ManyToOne, ForeignModel, OneToMany,
 OneToOne, IndexOnly]
 
 NUMERIC_TYPES = six.integer_types + (float, _Decimal, datetime, date, dtime)
```

### Comparing `rom-1.0.6/rom/exceptions.py` & `rom-1.0.7/rom/exceptions.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/index.py` & `rom-1.0.7/rom/index.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/wrappers.py` & `rom-1.0.7/rom/wrappers.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/columns.py` & `rom-1.0.7/rom/columns.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.6/rom/model.py` & `rom-1.0.7/rom/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 try:
     _Pipeline = client.BasePipeline
 except AttributeError:
     #redis-python client 3.0+ change
     _Pipeline = client.Pipeline
 
-from .columns import (Column, Text, PrimaryKey, ManyToOne, OneToOne, OneToMany,
-    MODELS, MODELS_REFERENCED, _on_delete, SKIP_ON_DELETE)
+from .columns import (Column, IndexOnly, Text, PrimaryKey, ManyToOne, OneToOne,
+    OneToMany, MODELS, MODELS_REFERENCED, _on_delete, SKIP_ON_DELETE)
 from .exceptions import (ORMError, UniqueKeyViolation, InvalidOperation,
     QueryError, ColumnError, InvalidColumnValue, DataRaceError,
     EntityDeletedError)
 from .index import GeneralIndex, GeoIndex, _ts
 from .query import Query, NUMERIC_TYPES
 from .util import (ClassProperty, _connect, session,
     _prefix_score, _script_load, _encode_unique_constraint,
@@ -646,15 +646,24 @@
             # handle unique index lookups
             if attr in cls._unique and (plain_attr not in cls._index or not _numeric):
                 if isinstance(value, tuple):
                     raise QueryError("Cannot query a unique index with a range of values")
                 single = not isinstance(value, list)
                 if single:
                     value = [value]
-                qvalues = list(map(cls._columns[attr]._to_redis, value))
+                if isinstance(cls._columns[attr], IndexOnly):
+                    def as_bytes(data) -> bytes:
+                        if isinstance(data, bytes):
+                            return data
+                        elif isinstance(data, str):
+                            return data.encode("latin-1")
+                        return str(data).encode("latin-1")
+                    qvalues = list(map(as_bytes, value))
+                else:
+                    qvalues = list(map(cls._columns[attr]._to_redis, value))
                 ids = [x for x in conn.hmget('%s:%s:uidx'%(model, attr), qvalues) if x]
                 if not ids:
                     return None if single else []
                 return cls.get(ids[0] if single else ids)
 
             if plain_attr not in cls._index:
                 raise QueryError("Cannot query on a column without an index")
```

### Comparing `rom-1.0.6/test/test_rom.py` & `rom-1.0.7/test/test_rom.py`

 * *Files identical despite different names*

