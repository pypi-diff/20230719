# Comparing `tmp/query_everywhere-0.1.2.tar.gz` & `tmp/query_everywhere-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "query_everywhere-0.1.2.tar", max compression
+gzip compressed data, was "query_everywhere-0.1.3.tar", max compression
```

## Comparing `query_everywhere-0.1.2.tar` & `query_everywhere-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1321 2023-07-19 12:14:45.404626 query_everywhere-0.1.2/README.md
--rw-r--r--   0        0        0      376 2023-07-19 12:15:09.751492 query_everywhere-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4343 2023-07-19 12:13:52.953588 query_everywhere-0.1.2/query_everywhere/__init__.py
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 query_everywhere-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1218 2023-07-19 13:00:49.124830 query_everywhere-0.1.3/README.md
+-rw-r--r--   0        0        0      376 2023-07-19 13:01:08.557182 query_everywhere-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4216 2023-07-19 12:59:25.186911 query_everywhere-0.1.3/query_everywhere/__init__.py
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 query_everywhere-0.1.3/PKG-INFO
```

### Comparing `query_everywhere-0.1.2/README.md` & `query_everywhere-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,48 +8,46 @@
 
 ## Example
 
 ```python
 from query_everywhere import Queryer
 
 # Create a Queryer with DSN
-dsn = "sqlite:///test.db"
+dsn = "sqlite:///db.sqlite3"
 queryer = Queryer(dsn)
 
 
 # Query
 filters = [
     ("name__contains", "part of name"),
     ("age__gte", 20),
     ("age__lt", 30),
-    ("status__in", ["running", "waiting"]),
     ("address__neq", "beijing"),
     ("address__eq", "shanghai"),
     ("address__icontains", "beijing"),
 ]
 order = "create_time desc"
 limit = 10
 offset = 0
-data = queryer.query("users", filters, order, limit, offset)
+data = queryer.query("people", filters, order, limit, offset)
 print(data)
+
 # It where do 
-# SELECT * FROM "users" WHERE name LIKE ? AND age >= ? AND age < ? AND status IN ?
-# AND address != ? AND address = ? AND LOWER("address") LIKE ?("address")__6
-# ORDER BY ? LIMIT ? OFFSET ?
+# SELECT * FROM "people" WHERE name LIKE ? AND age >= ? AND age < ?
+# AND address != ? AND address = ? AND LOWER(address) LIKE ? ORDER BY ? LIMIT ? OFFSET ?
 ```
 
 ## Supported operators
 
 | Operator | Comment |
 | --- | --- |
 | eq | equal to |
 | neq | not equal to |
 | ne | not equal to |
 | lt | less than |
 | gt | greater than |
 | lte | less than or equal to |
 | gte | greater than or equal to |
-| in | in the list of values |
 | startswith | starts with the given value |
 | endswith | ends with the given value |
 | contains | contains the given value |
 | icontains | contains the given value in the case-insensitive way |
```

### Comparing `query_everywhere-0.1.2/PKG-INFO` & `query_everywhere-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: query-everywhere
-Version: 0.1.2
+Version: 0.1.3
 Summary: Query every resource in RDBMS for REST
 Author: -LAN-
 Author-email: laipz8200@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
@@ -20,49 +20,47 @@
 
 ## Example
 
 ```python
 from query_everywhere import Queryer
 
 # Create a Queryer with DSN
-dsn = "sqlite:///test.db"
+dsn = "sqlite:///db.sqlite3"
 queryer = Queryer(dsn)
 
 
 # Query
 filters = [
     ("name__contains", "part of name"),
     ("age__gte", 20),
     ("age__lt", 30),
-    ("status__in", ["running", "waiting"]),
     ("address__neq", "beijing"),
     ("address__eq", "shanghai"),
     ("address__icontains", "beijing"),
 ]
 order = "create_time desc"
 limit = 10
 offset = 0
-data = queryer.query("users", filters, order, limit, offset)
+data = queryer.query("people", filters, order, limit, offset)
 print(data)
+
 # It where do 
-# SELECT * FROM "users" WHERE name LIKE ? AND age >= ? AND age < ? AND status IN ?
-# AND address != ? AND address = ? AND LOWER("address") LIKE ?("address")__6
-# ORDER BY ? LIMIT ? OFFSET ?
+# SELECT * FROM "people" WHERE name LIKE ? AND age >= ? AND age < ?
+# AND address != ? AND address = ? AND LOWER(address) LIKE ? ORDER BY ? LIMIT ? OFFSET ?
 ```
 
 ## Supported operators
 
 | Operator | Comment |
 | --- | --- |
 | eq | equal to |
 | neq | not equal to |
 | ne | not equal to |
 | lt | less than |
 | gt | greater than |
 | lte | less than or equal to |
 | gte | greater than or equal to |
-| in | in the list of values |
 | startswith | starts with the given value |
 | endswith | ends with the given value |
 | contains | contains the given value |
 | icontains | contains the given value in the case-insensitive way |
```

