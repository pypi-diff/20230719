# Comparing `tmp/pydantic_db_backend-0.6.1.tar.gz` & `tmp/pydantic_db_backend-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.6.1.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.7.0.tar", max compression
```

## Comparing `pydantic_db_backend-0.6.1.tar` & `pydantic_db_backend-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.6.1/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     7842 2023-07-18 09:42:27.492675 pydantic_db_backend-0.6.1/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.6.1/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     8681 2023-07-18 09:52:14.583217 pydantic_db_backend-0.6.1/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.6.1/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      990 2023-07-14 09:23:03.448444 pydantic_db_backend-0.6.1/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      768 2023-07-12 13:44:19.743864 pydantic_db_backend-0.6.1/pydantic_db_backend/indexes.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.6.1/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-18 09:52:39.482977 pydantic_db_backend-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.7.0/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     7309 2023-07-19 14:38:49.532351 pydantic_db_backend-0.7.0/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.7.0/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0    10063 2023-07-19 14:56:36.237269 pydantic_db_backend-0.7.0/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.7.0/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      990 2023-07-14 09:23:03.448444 pydantic_db_backend-0.7.0/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      768 2023-07-12 13:44:19.743864 pydantic_db_backend-0.7.0/pydantic_db_backend/indexes.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.7.0/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-19 14:59:35.712050 pydantic_db_backend-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.7.0/PKG-INFO
```

### Comparing `pydantic_db_backend-0.6.1/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.7.0/pydantic_db_backend/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -206,34 +206,15 @@
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 0,
         query_filter: dict = None,
         sort: List = None,
         max_results: bool = False,
     ) -> Tuple[List[BackendModel], int] | List[BackendModel]:
-        params = dict(
-            model=model,
-            skip=skip,
-            limit=limit,
-            query_filter=query_filter,
-            sort=sort,
-            max_results=max_results
-        )
-        max_results_value = None
-        if max_results:
-            ids, max_results_value = cls.get_uids(**params)
-        else:
-            ids = cls.get_uids(**params)
-
-        instances = [cls.get_instance(model, uid=x) for x in ids]
-
-        if max_results is True:
-            return instances, max_results_value
-        else:
-            return instances
+        raise NotImplementedError
 
     @classmethod
     def delete_uid(cls, model: Type[BackendModel], uid: str) -> None:
         raise NotImplementedError
 
     @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
```

### Comparing `pydantic_db_backend-0.6.1/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.7.0/pydantic_db_backend/backends/couchdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
-from typing import Dict, Type, List, Tuple
+from typing import Dict, Type, List, Tuple, Callable, Any
 
 import pydash
 from couchdb import ResourceConflict, ServerError
 from pydantic import BaseModel, Field
 
 import couchdb
 from pydantic_db_backend.backend import BackendBase, BackendModel
@@ -165,24 +165,25 @@
         db = cls.get_db(model)
         if uid in db:
             del db[uid]
         else:
             raise NotFound(uid=uid)
 
     @classmethod
-    def get_uids(
+    def find(
         cls,
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 25,
         query_filter: dict = None,
         sort: List = None,
-        max_results: bool | None = False
-    ) -> Tuple[List[str], int] | List[str]:
-
+        fields: List[str] = None,
+        max_results: bool | None = False,
+        func: Callable = None
+    ) -> Tuple[List[Any], int] | List[Any]:
         # fix 0 limit, since couchdb does not know this
         limit = 9999999 if limit == 0 else limit
 
         if query_filter is None:
             query_filter = {}
 
         # convert to json and back again, to have iso datetime strings
@@ -190,16 +191,21 @@
 
         db = cls.get_db(model)
 
         find_dict = {
             "selector": query_filter,
             "skip": skip,
             "limit": limit,
-            "fields": ['_id']
         }
+
+        if fields is not None:
+            find_dict |= {
+                "fields": fields
+            }
+
         if sort is not None:
             find_dict["sort"] = sort
 
         try:
             find_result = db.find(find_dict)
         except ServerError as e:
 
@@ -208,23 +214,67 @@
             if error_code == 400:
                 # @asc:  not what I expected the system to do. Better would be to modify the
                 # index cache and initiate a new get_db... and a loop
                 cls.indexes(model, dict(db=db), force_index_creation=True)
                 find_result = db.find(find_dict)
             else:
                 raise e
-
-        result = [x["_id"] for x in find_result]
+        result = [func(x) for x in find_result]
         if max_results:
             max_results = cls.get_max_results(model, query_filter)
             return result, max_results
         else:
             return result
 
     @classmethod
+    def get_uids(
+        cls,
+        model: Type[BackendModel],
+        skip: int = 0,
+        limit: int = 25,
+        query_filter: dict = None,
+        sort: List = None,
+        max_results: bool | None = False
+    ) -> Tuple[List[str], int] | List[str]:
+        r = cls.find(
+            model=model,
+            skip=skip,
+            limit=limit,
+            query_filter=query_filter,
+            sort=sort,
+            fields=['_id'],
+            max_results=max_results,
+            func=lambda x: x['_id']
+        )
+        r: Tuple[List[str], int] | List[str]
+        return r
+
+    @classmethod
+    def get_instances(
+        cls,
+        model: Type[BackendModel],
+        skip: int = 0,
+        limit: int = 0,
+        query_filter: dict = None,
+        sort: List = None,
+        max_results: bool = False
+    ) -> Tuple[List[BackendModel], int] | List[BackendModel]:
+        r = cls.find(
+            model=model,
+            skip=skip,
+            limit=limit,
+            query_filter=query_filter,
+            sort=sort,
+            max_results=max_results,
+            func=lambda x: model.parse_obj(x)
+        )
+        r: Tuple[List[BackendModel], int] | List[BackendModel]
+        return r
+
+    @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
         with cls.alias() as alias:
             server = cls._connections[alias].server
             name = cls.collection_name(model)
             if name in server:
                 server.delete(name)
 
@@ -249,15 +299,14 @@
                     else:
                         return 0
                 if v == row.key:
                     ret = row.value
                     return ret
 
 
-
 class CouchDbConnectionModel(BaseModel):
     alias: str
     uri: str
     server: couchdb.Server
     dbs: Dict[str, couchdb.Database] = Field(default_factory=dict)
 
     class Config():
```

### Comparing `pydantic_db_backend-0.6.1/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.7.0/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.6.1/pydantic_db_backend/indexes.py` & `pydantic_db_backend-0.7.0/pydantic_db_backend/indexes.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.6.1/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.7.0/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.6.1/pyproject.toml` & `pydantic_db_backend-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.6.1"
+version = "0.7.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.6.1/PKG-INFO` & `pydantic_db_backend-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.6.1
+Version: 0.7.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

