# Comparing `tmp/sqlsynthgen-0.3.0.tar.gz` & `tmp/sqlsynthgen-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsynthgen-0.3.0.tar", max compression
+gzip compressed data, was "sqlsynthgen-0.3.1.tar", max compression
```

## Comparing `sqlsynthgen-0.3.0.tar` & `sqlsynthgen-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-06 13:13:39.539871 sqlsynthgen-0.3.0/LICENSE
--rw-r--r--   0        0        0      247 2023-07-06 13:13:39.539871 sqlsynthgen-0.3.0/README.md
--rw-r--r--   0        0        0     1263 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/base.py
--rw-r--r--   0        0        0     5171 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/create.py
--rw-r--r--   0        0        0     3146 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/json_schemas/config_schema.json
--rw-r--r--   0        0        0     8755 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/main.py
--rw-r--r--   0        0        0    18739 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/make.py
--rw-r--r--   0        0        0     3117 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/providers.py
--rw-r--r--   0        0        0     1817 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/remove.py
--rw-r--r--   0        0        0     2418 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/settings.py
--rw-r--r--   0        0        0     2815 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/templates/ssg.py.j2
--rw-r--r--   0        0        0     5256 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/unique_generator.py
--rw-r--r--   0        0        0     2559 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/utils.py
--rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 sqlsynthgen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-19 15:44:20.115359 sqlsynthgen-0.3.1/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-19 15:44:20.115359 sqlsynthgen-0.3.1/README.md
+-rw-r--r--   0        0        0     1625 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/base.py
+-rw-r--r--   0        0        0     5171 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/create.py
+-rw-r--r--   0        0        0     3146 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/json_schemas/config_schema.json
+-rw-r--r--   0        0        0     8755 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/main.py
+-rw-r--r--   0        0        0    18739 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/make.py
+-rw-r--r--   0        0        0     3117 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/providers.py
+-rw-r--r--   0        0        0     1817 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/remove.py
+-rw-r--r--   0        0        0     2418 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/settings.py
+-rw-r--r--   0        0        0     2815 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/templates/ssg.py.j2
+-rw-r--r--   0        0        0     5256 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/unique_generator.py
+-rw-r--r--   0        0        0     2559 2023-07-19 15:44:20.123359 sqlsynthgen-0.3.1/sqlsynthgen/utils.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 sqlsynthgen-0.3.1/PKG-INFO
```

### Comparing `sqlsynthgen-0.3.0/LICENSE` & `sqlsynthgen-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/base.py` & `sqlsynthgen-0.3.1/sqlsynthgen/base.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/create.py` & `sqlsynthgen-0.3.1/sqlsynthgen/create.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/json_schemas/config_schema.json` & `sqlsynthgen-0.3.1/sqlsynthgen/json_schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/main.py` & `sqlsynthgen-0.3.1/sqlsynthgen/main.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/make.py` & `sqlsynthgen-0.3.1/sqlsynthgen/make.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/providers.py` & `sqlsynthgen-0.3.1/sqlsynthgen/providers.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/remove.py` & `sqlsynthgen-0.3.1/sqlsynthgen/remove.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/settings.py` & `sqlsynthgen-0.3.1/sqlsynthgen/settings.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/templates/ssg.py.j2` & `sqlsynthgen-0.3.1/sqlsynthgen/templates/ssg.py.j2`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/unique_generator.py` & `sqlsynthgen-0.3.1/sqlsynthgen/unique_generator.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/sqlsynthgen/utils.py` & `sqlsynthgen-0.3.1/sqlsynthgen/utils.py`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.3.0/PKG-INFO` & `sqlsynthgen-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: sqlsynthgen
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: Synthetic SQL data generator
 License: MIT
 Author: Iain
 Author-email: 25081046+Iain-S@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Database
+Classifier: Topic :: Utilities
 Provides-Extra: docs
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: greenlet (>=2.0.2,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: mimesis (>=6.1.1,<7.0.0)
```

