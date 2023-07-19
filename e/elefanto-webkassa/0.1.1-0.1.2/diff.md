# Comparing `tmp/elefanto_webkassa-0.1.1.tar.gz` & `tmp/elefanto_webkassa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.1.1.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.1.2.tar", max compression
```

## Comparing `elefanto_webkassa-0.1.1.tar` & `elefanto_webkassa-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.1/README.md
--rw-r--r--   0        0        0      847 2023-07-19 07:17:08.056758 elefanto_webkassa-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      506 2023-07-19 05:22:45.833486 elefanto_webkassa-0.1.1/webkassa/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-19 06:14:33.158762 elefanto_webkassa-0.1.1/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.1/webkassa/apps.py
--rw-r--r--   0        0        0     3455 2023-07-19 06:47:19.127943 elefanto_webkassa-0.1.1/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.1/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     2922 2023-07-19 06:45:36.974594 elefanto_webkassa-0.1.1/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.1/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.1/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6172 2023-07-19 07:05:40.343630 elefanto_webkassa-0.1.1/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.1/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.2/README.md
+-rw-r--r--   0        0        0      847 2023-07-19 07:42:03.179132 elefanto_webkassa-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-07-19 05:22:45.833486 elefanto_webkassa-0.1.2/webkassa/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-19 06:14:33.158762 elefanto_webkassa-0.1.2/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.2/webkassa/apps.py
+-rw-r--r--   0        0        0     3455 2023-07-19 06:47:19.127943 elefanto_webkassa-0.1.2/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.2/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     2922 2023-07-19 06:45:36.974594 elefanto_webkassa-0.1.2/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.2/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.2/webkassa/services/__init__.py
+-rw-r--r--   0        0        0     6024 2023-07-19 07:41:47.463341 elefanto_webkassa-0.1.2/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.2/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.2/PKG-INFO
```

### Comparing `elefanto_webkassa-0.1.1/pyproject.toml` & `elefanto_webkassa-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.1.1/webkassa/admin.py` & `elefanto_webkassa-0.1.2/webkassa/admin.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.1/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.1.2/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.1/webkassa/models.py` & `elefanto_webkassa-0.1.2/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.1/webkassa/serializers.py` & `elefanto_webkassa-0.1.2/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.1/webkassa/services/manager.py` & `elefanto_webkassa-0.1.2/webkassa/services/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 
 from rest_framework.exceptions import AuthenticationFailed, ValidationError
 
 from webkassa.models import Check, WebKassaAccount, WebkassaErrorLog
 from webkassa.serializers import CheckSerializer
 
 WEBKASSA_CONFIG = settings.WEBKASSA_CONFIG
-URL = WEBKASSA_CONFIG['url'] if WEBKASSA_CONFIG['is_prod'] else WEBKASSA_CONFIG['test_url']
-API_KEY = WEBKASSA_CONFIG['api_key'] if WEBKASSA_CONFIG['is_prod'] else WEBKASSA_CONFIG['test_api_key']
-HEADERS = {'X-API-KEY': API_KEY, 'Content-Type': 'application/json'}
+URL = WEBKASSA_CONFIG['url']
+HEADERS = {'X-API-KEY': WEBKASSA_CONFIG['api_key'], 'Content-Type': 'application/json'}
 
 
 class WebKassaManager:
     _token: str = None
     _email: str = None
     cashier: WebKassaAccount = None
     _client: httpx.Client = None
```

### Comparing `elefanto_webkassa-0.1.1/PKG-INFO` & `elefanto_webkassa-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

