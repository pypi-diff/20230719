# Comparing `tmp/django-excel-response2-3.0.5.tar.gz` & `tmp/django-excel-response2-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-excel-response2-3.0.5.tar", last modified: Fri Feb 24 08:48:50 2023, max compression
+gzip compressed data, was "django-excel-response2-3.0.6.tar", last modified: Wed Jul 19 07:59:57 2023, max compression
```

## Comparing `django-excel-response2-3.0.5.tar` & `django-excel-response2-3.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-24 08:48:50.244154 django-excel-response2-3.0.5/
--rw-r--r--   0 huangqimin   (501) staff       (20)     3924 2023-02-24 08:48:50.244297 django-excel-response2-3.0.5/PKG-INFO
--rw-r--r--   0 huangqimin   (501) staff       (20)     3221 2023-02-23 07:52:31.000000 django-excel-response2-3.0.5/README.md
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-24 08:48:50.241932 django-excel-response2-3.0.5/django_excel_response/
--rw-r--r--   0 huangqimin   (501) staff       (20)      150 2023-02-24 08:34:32.000000 django-excel-response2-3.0.5/django_excel_response/__init__.py
--rw-r--r--   0 huangqimin   (501) staff       (20)     5257 2023-02-24 08:43:19.000000 django-excel-response2-3.0.5/django_excel_response/excel_response.py
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-24 08:48:50.243465 django-excel-response2-3.0.5/django_excel_response2.egg-info/
--rw-r--r--   0 huangqimin   (501) staff       (20)     3924 2023-02-24 08:48:50.000000 django-excel-response2-3.0.5/django_excel_response2.egg-info/PKG-INFO
--rw-r--r--   0 huangqimin   (501) staff       (20)      368 2023-02-24 08:48:50.000000 django-excel-response2-3.0.5/django_excel_response2.egg-info/SOURCES.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)        1 2023-02-24 08:48:50.000000 django-excel-response2-3.0.5/django_excel_response2.egg-info/dependency_links.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)       36 2023-02-24 08:48:50.000000 django-excel-response2-3.0.5/django_excel_response2.egg-info/requires.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)       22 2023-02-24 08:48:50.000000 django-excel-response2-3.0.5/django_excel_response2.egg-info/top_level.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)       61 2023-02-24 08:48:50.244865 django-excel-response2-3.0.5/setup.cfg
--rw-r--r--   0 huangqimin   (501) staff       (20)     1048 2023-02-24 08:48:48.000000 django-excel-response2-3.0.5/setup.py
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-24 08:48:50.243755 django-excel-response2-3.0.5/tests/
--rw-r--r--   0 huangqimin   (501) staff       (20)     4277 2023-02-24 07:38:44.000000 django-excel-response2-3.0.5/tests/test_django_excel_response2.py
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-07-19 07:59:57.181527 django-excel-response2-3.0.6/
+-rw-r--r--   0 huangqimin   (501) staff       (20)     3924 2023-07-19 07:59:57.181679 django-excel-response2-3.0.6/PKG-INFO
+-rw-r--r--   0 huangqimin   (501) staff       (20)     3221 2023-02-23 07:52:31.000000 django-excel-response2-3.0.6/README.md
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-07-19 07:59:57.177678 django-excel-response2-3.0.6/django_excel_response/
+-rw-r--r--   0 huangqimin   (501) staff       (20)      150 2023-02-24 08:34:32.000000 django-excel-response2-3.0.6/django_excel_response/__init__.py
+-rw-r--r--   0 huangqimin   (501) staff       (20)     5312 2023-07-19 07:55:20.000000 django-excel-response2-3.0.6/django_excel_response/excel_response.py
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-07-19 07:59:57.180371 django-excel-response2-3.0.6/django_excel_response2.egg-info/
+-rw-r--r--   0 huangqimin   (501) staff       (20)     3924 2023-07-19 07:59:57.000000 django-excel-response2-3.0.6/django_excel_response2.egg-info/PKG-INFO
+-rw-r--r--   0 huangqimin   (501) staff       (20)      368 2023-07-19 07:59:57.000000 django-excel-response2-3.0.6/django_excel_response2.egg-info/SOURCES.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)        1 2023-07-19 07:59:57.000000 django-excel-response2-3.0.6/django_excel_response2.egg-info/dependency_links.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)       36 2023-07-19 07:59:57.000000 django-excel-response2-3.0.6/django_excel_response2.egg-info/requires.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)       22 2023-07-19 07:59:57.000000 django-excel-response2-3.0.6/django_excel_response2.egg-info/top_level.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)       61 2023-07-19 07:59:57.182195 django-excel-response2-3.0.6/setup.cfg
+-rw-r--r--   0 huangqimin   (501) staff       (20)     1048 2023-07-19 07:59:55.000000 django-excel-response2-3.0.6/setup.py
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-07-19 07:59:57.180690 django-excel-response2-3.0.6/tests/
+-rw-r--r--   0 huangqimin   (501) staff       (20)     4277 2023-02-24 07:38:44.000000 django-excel-response2-3.0.6/tests/test_django_excel_response2.py
```

### Comparing `django-excel-response2-3.0.5/PKG-INFO` & `django-excel-response2-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-excel-response2
-Version: 3.0.5
+Version: 3.0.6
 Summary: A function extends of Tarken's django-excel-response
 Home-page: https://github.com/django-xxx/django-excel-response2
 Author: Hackathon
 Author-email: kimi.huang@brightcells.com
 Keywords: django-excel-response django-excel-response2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-excel-response2-3.0.5/README.md` & `django-excel-response2-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django-excel-response2-3.0.5/django_excel_response/excel_response.py` & `django-excel-response2-3.0.6/django_excel_response/excel_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,22 @@
             if Support_ValuesQuerySet and isinstance(sheet_data, ValuesQuerySet):
                 sheet_data = list(sheet_data)
             elif isinstance(sheet_data, QuerySet):
                 sheet_data = list(sheet_data.values())
             if not hasattr(sheet_data, '__getitem__'):
                 valid_data = False
                 break
-            if isinstance(sheet_data[0], dict):
-                if sheet_headers is None:
-                    sheet_headers = list(sheet_data[0].keys())
-                sheet_data = [[row[col] for col in sheet_headers] for row in sheet_data]
-            if not hasattr(sheet_data[0], '__getitem__'):
-                valid_data = False
-                break
+            if sheet_data:
+                if isinstance(sheet_data[0], dict):
+                    if sheet_headers is None:
+                        sheet_headers = list(sheet_data[0].keys())
+                    sheet_data = [[row[col] for col in sheet_headers] for row in sheet_data]
+                if not hasattr(sheet_data[0], '__getitem__'):
+                    valid_data = False
+                    break
             if sheet_headers and not hasattr(sheet_headers[0], '__getitem__'):
                 valid_data = False
                 break
             sheet_info['data'] = sheet_data
             sheet_info['headers'] = sheet_headers
             self.data[sheet_name] = sheet_info
         assert valid_data is True, 'ExcelStorage requires a sequence of sequences'
```

### Comparing `django-excel-response2-3.0.5/django_excel_response2.egg-info/PKG-INFO` & `django-excel-response2-3.0.6/django_excel_response2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-excel-response2
-Version: 3.0.5
+Version: 3.0.6
 Summary: A function extends of Tarken's django-excel-response
 Home-page: https://github.com/django-xxx/django-excel-response2
 Author: Hackathon
 Author-email: kimi.huang@brightcells.com
 Keywords: django-excel-response django-excel-response2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-excel-response2-3.0.5/setup.py` & `django-excel-response2-3.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import with_statement
 
 from setuptools import setup
 
 
-version = '3.0.5'
+version = '3.0.6'
 
 
 setup(
     name='django-excel-response2',
     version=version,
     keywords='django-excel-response django-excel-response2',
     description="A function extends of Tarken's django-excel-response",
```

### Comparing `django-excel-response2-3.0.5/tests/test_django_excel_response2.py` & `django-excel-response2-3.0.6/tests/test_django_excel_response2.py`

 * *Files identical despite different names*

