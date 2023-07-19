# Comparing `tmp/query_everywhere-0.1.0.tar.gz` & `tmp/query_everywhere-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "query_everywhere-0.1.0.tar", max compression
+gzip compressed data, was "query_everywhere-0.1.1.tar", max compression
```

## Comparing `query_everywhere-0.1.0.tar` & `query_everywhere-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1221 2023-07-19 11:49:29.813757 query_everywhere-0.1.0/README.md
--rw-r--r--   0        0        0      376 2023-07-19 11:32:14.788376 query_everywhere-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4148 2023-07-19 12:01:07.420514 query_everywhere-0.1.0/query_everywhere/__init__.py
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 query_everywhere-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1291 2023-07-19 12:08:05.072708 query_everywhere-0.1.1/README.md
+-rw-r--r--   0        0        0      376 2023-07-19 12:09:52.524951 query_everywhere-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4341 2023-07-19 12:06:22.676107 query_everywhere-0.1.1/query_everywhere/__init__.py
+-rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 query_everywhere-0.1.1/PKG-INFO
```

### Comparing `query_everywhere-0.1.0/README.md` & `query_everywhere-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -45,8 +45,9 @@
 | lt | less than |
 | gt | greater than |
 | lte | less than or equal to |
 | gte | greater than or equal to |
 | in | in the list of values |
 | startswith | starts with the given value |
 | endswith | ends with the given value |
-| contains | contains the given value |
+| contains | contains the given value |
+| icontains | contains the given value in the case-insensitive way |
```

### Comparing `query_everywhere-0.1.0/query_everywhere/__init__.py` & `query_everywhere-0.1.1/query_everywhere/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "gt",
     "lte",
     "gte",
     "in",
     "startswith",
     "endswith",
     "contains",
+    "icontains",
 }
 
 
 class Queryer:
     def __init__(self, dsn: str) -> None:
         self.engine = create_engine(dsn, echo=True)
 
@@ -62,14 +63,18 @@
                     results.append((field, "IN", value))
                 case "startswith":
                     results.append((field, "LIKE", value + "%"))
                 case "endswith":
                     results.append((field, "LIKE", "%" + value))
                 case "contains":
                     results.append((field, "LIKE", "%" + value + "%"))
+                case "icontains":
+                    results.append(
+                        (f"LOWER({field})", "LIKE", "%" + str(value).lower() + "%")
+                    )
         return results
 
     def _build_where_conditions(self, conditions: list[tuple[str, str, Any]]) -> str:
         return " AND ".join(
             [
                 f"{condition[0]} {condition[1]} :{condition[0]}__{idx}"
                 for idx, condition in enumerate(conditions)
```

### Comparing `query_everywhere-0.1.0/PKG-INFO` & `query_everywhere-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: query-everywhere
-Version: 0.1.0
+Version: 0.1.1
 Summary: Query every resource in RDBMS for REST
 Author: -LAN-
 Author-email: laipz8200@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
@@ -58,7 +58,9 @@
 | gt | greater than |
 | lte | less than or equal to |
 | gte | greater than or equal to |
 | in | in the list of values |
 | startswith | starts with the given value |
 | endswith | ends with the given value |
 | contains | contains the given value |
+| icontains | contains the given value in the case-insensitive way |
+
```

