# Comparing `tmp/bstk_datatables-0.1.7.tar.gz` & `tmp/bstk_datatables-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.1.7.tar", max compression
+gzip compressed data, was "bstk_datatables-0.1.8.tar", max compression
```

## Comparing `bstk_datatables-0.1.7.tar` & `bstk_datatables-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4244 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/README.md
--rw-r--r--   0        0        0     2358 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3248 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/merge.py
--rw-r--r--   0        0        0     7133 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-07-18 01:23:42.316528 bstk_datatables-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/README.md
+-rw-r--r--   0        0        0     2358 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3248 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     7552 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-19 12:15:49.975392 bstk_datatables-0.1.8/bstk_datatables/table.py
+-rw-r--r--   0        0        0      669 2023-07-19 12:16:16.363382 bstk_datatables-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.8/PKG-INFO
```

### Comparing `bstk_datatables-0.1.7/README.md` & `bstk_datatables-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.7/bstk_datatables/__init__.py` & `bstk_datatables-0.1.8/bstk_datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.7/bstk_datatables/entry.py` & `bstk_datatables-0.1.8/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.7/bstk_datatables/enum.py` & `bstk_datatables-0.1.8/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.7/bstk_datatables/merge.py` & `bstk_datatables-0.1.8/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.7/bstk_datatables/schema.py` & `bstk_datatables-0.1.8/bstk_datatables/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,31 @@
 from marshmallow import Schema as MarshmallowSchema
 from marshmallow import fields as marshmallow_fields
 
 from . import SCHEMAFIELD_EXTATTR, SCHEMAFIELD_MAP, name_to_code, schema_to_marshmallow
 from .enum import Enum, PyEnum
 
 
+class NestedSchemaField(marshmallow_fields.Field):
+    """
+    A little helper class to use if you're nesting a Schema as a field within another marshmallow schema.
+    """
+
+    def _serialize(
+        self,
+        value: typing.Any,
+        attr: typing.Union[str, None],
+        obj: typing.Any,
+        **kwargs,
+    ):
+        if isinstance(value, Schema):
+            return value.export()
+        return value
+
+
 class SchemaValuesError(Exception):
     errors: typing.Dict[typing.AnyStr, typing.List[typing.AnyStr]]
 
     def __init__(
         self,
         *args: object,
         errors: typing.Dict[typing.AnyStr, typing.List[typing.AnyStr]],
```

### Comparing `bstk_datatables-0.1.7/bstk_datatables/table.py` & `bstk_datatables-0.1.8/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.7/pyproject.toml` & `bstk_datatables-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.1.7"
+version = "0.1.8"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.1.7/PKG-INFO` & `bstk_datatables-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.1.7
+Version: 0.1.8
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

