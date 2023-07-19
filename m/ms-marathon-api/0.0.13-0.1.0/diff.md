# Comparing `tmp/ms_marathon_api-0.0.13.tar.gz` & `tmp/ms_marathon_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_marathon_api-0.0.13.tar", max compression
+gzip compressed data, was "ms_marathon_api-0.1.0.tar", max compression
```

## Comparing `ms_marathon_api-0.0.13.tar` & `ms_marathon_api-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/LICENSE
--rw-r--r--   0        0        0      614 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/README.md
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/marathon/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/marathon/__tests__/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/marathon/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/marathon/api/__tests__/__init__.py
--rw-r--r--   0        0        0     4368 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/marathon/api/__tests__/test_timereporting.py
--rw-r--r--   0        0        0     1587 2023-07-17 06:29:16.698908 ms_marathon_api-0.0.13/ms_marathon_api/marathon/api/timereporting.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/connection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/connection/__tests__/__init__.py
--rw-r--r--   0        0        0     2692 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py
--rw-r--r--   0        0        0     1167 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/connection/mysql.py
--rw-r--r--   0        0        0     1807 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/dto/TimeReportingDTO.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/dto/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/queries/__init__.py
--rw-r--r--   0        0        0      228 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/ms_marathon_api/marathon/queries/marathon.py
--rw-r--r--   0        0        0      960 2023-07-17 06:29:16.702909 ms_marathon_api-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 ms_marathon_api-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/LICENSE
+-rw-r--r--   0        0        0      614 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/__tests__/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__tests__/__init__.py
+-rw-r--r--   0        0        0     4368 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__tests__/test_timereporting.py
+-rw-r--r--   0        0        0     1579 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/timereporting.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__tests__/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py
+-rw-r--r--   0        0        0     1167 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/mysql.py
+-rw-r--r--   0        0        0     2300 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/dto/TimeReportingDTO.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/dto/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/queries/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/queries/marathon.py
+-rw-r--r--   0        0        0      959 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 ms_marathon_api-0.1.0/PKG-INFO
```

### Comparing `ms_marathon_api-0.0.13/LICENSE` & `ms_marathon_api-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.0.13/README.md` & `ms_marathon_api-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.0.13/ms_marathon_api/marathon/api/__tests__/test_timereporting.py` & `ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__tests__/test_timereporting.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.0.13/ms_marathon_api/marathon/api/timereporting.py` & `ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/timereporting.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 BIGQUERY_TABLE_SCHEMA = {
     "company": "STRING",
     "employee": "STRING",
     "msemail": "STRING",
     "client": "STRING",
     "clientname": "STRING",
-    "project": "STRING",
+    "project": "INTEGER",
     "mscode": "STRING",
-    "feecode": "STRING",
-    "accountingdate": "TIMESTAMP",
-    "recorddate": "TIMESTAMP",
+    "feecode": "INTEGER",
+    "accountingdate": "DATE",
+    "recorddate": "DATE",
     "minutes": "FLOAT",
 }
 
 
 class MarathonTimeReporting:
     def __init__(self, host, user, password, database):
         self.mysql_connection = MySQLConnection(host, user, password, database)
```

### Comparing `ms_marathon_api-0.0.13/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py` & `ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.0.13/ms_marathon_api/marathon/connection/mysql.py` & `ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/mysql.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.0.13/PKG-INFO` & `ms_marathon_api-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ms-marathon-api
-Version: 0.0.13
+Version: 0.1.0
 Summary: API to connect with Marathon system and migrate data to Bigquery
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coverage (>=7.2.2,<8.0.0)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
-Requires-Dist: gc-google-services-api (>=1.2.9,<2.0.0)
+Requires-Dist: gc-google-services-api (>=1.3.0,<2.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
 Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # How to contribute
 After clone repository
```

