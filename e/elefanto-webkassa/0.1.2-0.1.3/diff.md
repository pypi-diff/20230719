# Comparing `tmp/elefanto_webkassa-0.1.2.tar.gz` & `tmp/elefanto_webkassa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.1.2.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.1.3.tar", max compression
```

## Comparing `elefanto_webkassa-0.1.2.tar` & `elefanto_webkassa-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.2/README.md
--rw-r--r--   0        0        0      847 2023-07-19 07:42:03.179132 elefanto_webkassa-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      506 2023-07-19 05:22:45.833486 elefanto_webkassa-0.1.2/webkassa/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-19 06:14:33.158762 elefanto_webkassa-0.1.2/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.2/webkassa/apps.py
--rw-r--r--   0        0        0     3455 2023-07-19 06:47:19.127943 elefanto_webkassa-0.1.2/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.2/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     2922 2023-07-19 06:45:36.974594 elefanto_webkassa-0.1.2/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.2/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.2/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6024 2023-07-19 07:41:47.463341 elefanto_webkassa-0.1.2/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.2/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.3/README.md
+-rw-r--r--   0        0        0      847 2023-07-19 07:44:01.145441 elefanto_webkassa-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.1.3/webkassa/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-19 06:14:33.158762 elefanto_webkassa-0.1.3/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.3/webkassa/apps.py
+-rw-r--r--   0        0        0     3455 2023-07-19 06:47:19.127943 elefanto_webkassa-0.1.3/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.3/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     2922 2023-07-19 06:45:36.974594 elefanto_webkassa-0.1.3/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.3/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.3/webkassa/services/__init__.py
+-rw-r--r--   0        0        0     6024 2023-07-19 07:41:47.463341 elefanto_webkassa-0.1.3/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.3/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.3/PKG-INFO
```

### Comparing `elefanto_webkassa-0.1.2/pyproject.toml` & `elefanto_webkassa-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.1.2/webkassa/admin.py` & `elefanto_webkassa-0.1.3/webkassa/admin.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.2/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.1.3/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.2/webkassa/models.py` & `elefanto_webkassa-0.1.3/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.2/webkassa/serializers.py` & `elefanto_webkassa-0.1.3/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.2/webkassa/services/manager.py` & `elefanto_webkassa-0.1.3/webkassa/services/manager.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.2/PKG-INFO` & `elefanto_webkassa-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

