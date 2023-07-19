# Comparing `tmp/elefanto_webkassa-0.2.0.tar.gz` & `tmp/elefanto_webkassa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.2.0.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.2.1.tar", max compression
```

## Comparing `elefanto_webkassa-0.2.0.tar` & `elefanto_webkassa-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.2.0/README.md
--rw-r--r--   0        0        0      847 2023-07-19 09:37:05.807374 elefanto_webkassa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.2.0/webkassa/__init__.py
--rw-r--r--   0        0        0     1384 2023-07-19 08:43:13.901335 elefanto_webkassa-0.2.0/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.2.0/webkassa/apps.py
--rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.2.0/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.2.0/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.2.0/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.2.0/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.2.0/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6849 2023-07-19 09:36:43.771822 elefanto_webkassa-0.2.0/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.2.0/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.2.1/README.md
+-rw-r--r--   0        0        0      847 2023-07-19 09:42:59.844150 elefanto_webkassa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.2.1/webkassa/__init__.py
+-rw-r--r--   0        0        0     1656 2023-07-19 09:42:52.628298 elefanto_webkassa-0.2.1/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.2.1/webkassa/apps.py
+-rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.2.1/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.2.1/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.2.1/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.2.1/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.2.1/webkassa/services/__init__.py
+-rw-r--r--   0        0        0     6849 2023-07-19 09:36:43.771822 elefanto_webkassa-0.2.1/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.2.1/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.2.1/PKG-INFO
```

### Comparing `elefanto_webkassa-0.2.0/pyproject.toml` & `elefanto_webkassa-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.2.0/webkassa/admin.py` & `elefanto_webkassa-0.2.1/webkassa/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from django.contrib import admin
+from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 
 from webkassa.models import Check, WebKassaAccount, WebkassaErrorLog
 
 
 @admin.register(Check)
 class CheckAdmin(admin.ModelAdmin):
-    list_display = ('id', 'date_time', 'ticket_url', 'check_order_number')
+    list_display = ('id', 'date_time', 'show_ticket_url', 'check_order_number')
     list_display_links = ('id', 'date_time', 'check_order_number')
 
+    def show_ticket_url(self, obj):
+        return format_html("<a href='{url}'>{url}</a>", url=obj.ticket_url)
+
+    show_ticket_url.short_description = _('Ticket URL')
+
     def has_add_permission(self, request):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
 
     def has_change_permission(self, request, obj=None):
```

### Comparing `elefanto_webkassa-0.2.0/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.2.1/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.0/webkassa/models.py` & `elefanto_webkassa-0.2.1/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.0/webkassa/serializers.py` & `elefanto_webkassa-0.2.1/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.0/webkassa/services/manager.py` & `elefanto_webkassa-0.2.1/webkassa/services/manager.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.2.0/PKG-INFO` & `elefanto_webkassa-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

