# Comparing `tmp/elefanto_webkassa-0.1.5.tar.gz` & `tmp/elefanto_webkassa-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.1.5.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.1.6.tar", max compression
```

## Comparing `elefanto_webkassa-0.1.5.tar` & `elefanto_webkassa-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.5/README.md
--rw-r--r--   0        0        0      847 2023-07-19 08:02:09.960629 elefanto_webkassa-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.1.5/webkassa/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-19 06:14:33.158762 elefanto_webkassa-0.1.5/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.5/webkassa/apps.py
--rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.1.5/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.5/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.1.5/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.5/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.5/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6024 2023-07-19 07:41:47.463341 elefanto_webkassa-0.1.5/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.5/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.6/README.md
+-rw-r--r--   0        0        0      847 2023-07-19 08:43:19.261221 elefanto_webkassa-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.1.6/webkassa/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-19 08:43:13.901335 elefanto_webkassa-0.1.6/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.6/webkassa/apps.py
+-rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.1.6/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.6/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.1.6/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.6/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.6/webkassa/services/__init__.py
+-rw-r--r--   0        0        0     6024 2023-07-19 07:41:47.463341 elefanto_webkassa-0.1.6/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.6/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.6/PKG-INFO
```

### Comparing `elefanto_webkassa-0.1.5/pyproject.toml` & `elefanto_webkassa-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.1.5/webkassa/admin.py` & `elefanto_webkassa-0.1.6/webkassa/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     def has_delete_permission(self, request, obj=None):
         return False
 
     def has_change_permission(self, request, obj=None):
         return False
 
     def get_queryset(self, request):
-        return super().get_queryset(request).select_related('check')
+        return super().get_queryset(request).select_related('check_obj')
```

### Comparing `elefanto_webkassa-0.1.5/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.1.6/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.5/webkassa/models.py` & `elefanto_webkassa-0.1.6/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.5/webkassa/serializers.py` & `elefanto_webkassa-0.1.6/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.5/webkassa/services/manager.py` & `elefanto_webkassa-0.1.6/webkassa/services/manager.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.5/PKG-INFO` & `elefanto_webkassa-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

