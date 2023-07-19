# Comparing `tmp/elefanto_webkassa-0.2.2.tar.gz` & `tmp/elefanto_webkassa-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.2.2.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.2.3.tar", max compression
```

## Comparing `elefanto_webkassa-0.2.2.tar` & `elefanto_webkassa-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.2.2/README.md
--rw-r--r--   0        0        0      847 2023-07-19 09:46:10.964239 elefanto_webkassa-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.2.2/webkassa/__init__.py
--rw-r--r--   0        0        0     1656 2023-07-19 09:42:52.628298 elefanto_webkassa-0.2.2/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.2.2/webkassa/apps.py
--rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.2.2/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.2.2/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.2.2/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.2.2/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.2.2/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6762 2023-07-19 09:46:03.768386 elefanto_webkassa-0.2.2/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.2.2/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.2.3/README.md
+-rw-r--r--   0        0        0      847 2023-07-19 09:51:12.249888 elefanto_webkassa-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.2.3/webkassa/__init__.py
+-rw-r--r--   0        0        0     1656 2023-07-19 09:42:52.628298 elefanto_webkassa-0.2.3/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.2.3/webkassa/apps.py
+-rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.2.3/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.2.3/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.2.3/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.2.3/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.2.3/webkassa/services/__init__.py
+-rw-r--r--   0        0        0     6897 2023-07-19 09:50:59.682160 elefanto_webkassa-0.2.3/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.2.3/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.2.3/PKG-INFO
```

### Comparing `elefanto_webkassa-0.2.2/pyproject.toml` & `elefanto_webkassa-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.2.2/webkassa/admin.py` & `elefanto_webkassa-0.2.3/webkassa/admin.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.2/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.2.3/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.2/webkassa/models.py` & `elefanto_webkassa-0.2.3/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.2/webkassa/serializers.py` & `elefanto_webkassa-0.2.3/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.2/webkassa/services/manager.py` & `elefanto_webkassa-0.2.3/webkassa/services/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,21 +116,22 @@
                 new_modifiers.append(modifier)
             data.update({
                 'TicketModifiers': new_modifiers,
             })
         return data
 
     @staticmethod
-    def _prepare_check():
-        return Check.objects.create()
+    def _prepare_check(check_order_number):
+        check_obj, created = Check.objects.get_or_create(check_order_number=check_order_number) # noqa
+        return check_obj
 
     def _create_check(self, data, check_obj=None):
 
         if not check_obj:
-            check_obj = self._prepare_check()
+            check_obj = self._prepare_check(data['ExternalCheckNumber'])
 
         url = f'{self._url}/api/Check'
         try:
             response = self._client.post(url, json=data, headers=HEADERS, timeout=30).json()
             if 'Data' in response:
                 check = response['Data']
                 check_serializer = CheckSerializer(check_obj, data=check, partial=True)
```

### Comparing `elefanto_webkassa-0.2.2/PKG-INFO` & `elefanto_webkassa-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

