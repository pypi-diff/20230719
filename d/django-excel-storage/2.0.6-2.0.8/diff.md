# Comparing `tmp/django-excel-storage-2.0.6.tar.gz` & `tmp/django-excel-storage-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-excel-storage-2.0.6.tar", last modified: Wed Feb 22 04:09:15 2023, max compression
+gzip compressed data, was "django-excel-storage-2.0.8.tar", last modified: Thu Feb 23 07:21:34 2023, max compression
```

## Comparing `django-excel-storage-2.0.6.tar` & `django-excel-storage-2.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-22 04:09:15.463838 django-excel-storage-2.0.6/
--rw-r--r--   0 huangqimin   (501) staff       (20)     2539 2023-02-22 04:09:15.463981 django-excel-storage-2.0.6/PKG-INFO
--rw-r--r--   0 huangqimin   (501) staff       (20)     1896 2021-01-14 15:42:28.000000 django-excel-storage-2.0.6/README.md
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-22 04:09:15.461437 django-excel-storage-2.0.6/django_excel_storage/
--rw-r--r--   0 huangqimin   (501) staff       (20)       85 2020-03-12 07:11:02.000000 django-excel-storage-2.0.6/django_excel_storage/__init__.py
--rw-r--r--   0 huangqimin   (501) staff       (20)     4464 2023-02-21 09:23:24.000000 django-excel-storage-2.0.6/django_excel_storage/excel_storage.py
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-22 04:09:15.463175 django-excel-storage-2.0.6/django_excel_storage.egg-info/
--rw-r--r--   0 huangqimin   (501) staff       (20)     2539 2023-02-22 04:09:15.000000 django-excel-storage-2.0.6/django_excel_storage.egg-info/PKG-INFO
--rw-r--r--   0 huangqimin   (501) staff       (20)      353 2023-02-22 04:09:15.000000 django-excel-storage-2.0.6/django_excel_storage.egg-info/SOURCES.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)        1 2023-02-22 04:09:15.000000 django-excel-storage-2.0.6/django_excel_storage.egg-info/dependency_links.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)       43 2023-02-22 04:09:15.000000 django-excel-storage-2.0.6/django_excel_storage.egg-info/requires.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)       21 2023-02-22 04:09:15.000000 django-excel-storage-2.0.6/django_excel_storage.egg-info/top_level.txt
--rw-r--r--   0 huangqimin   (501) staff       (20)       61 2023-02-22 04:09:15.464524 django-excel-storage-2.0.6/setup.cfg
--rw-r--r--   0 huangqimin   (501) staff       (20)      994 2023-02-22 04:09:13.000000 django-excel-storage-2.0.6/setup.py
-drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-22 04:09:15.463537 django-excel-storage-2.0.6/tests/
--rw-r--r--   0 huangqimin   (501) staff       (20)     6758 2023-02-21 10:51:14.000000 django-excel-storage-2.0.6/tests/test_django_excel_storage.py
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-23 07:21:34.346790 django-excel-storage-2.0.8/
+-rw-r--r--   0 huangqimin   (501) staff       (20)     4882 2023-02-23 07:21:34.347005 django-excel-storage-2.0.8/PKG-INFO
+-rw-r--r--   0 huangqimin   (501) staff       (20)     4239 2023-02-22 09:48:34.000000 django-excel-storage-2.0.8/README.md
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-23 07:21:34.337941 django-excel-storage-2.0.8/django_excel_storage/
+-rw-r--r--   0 huangqimin   (501) staff       (20)      154 2023-02-23 07:11:42.000000 django-excel-storage-2.0.8/django_excel_storage/__init__.py
+-rw-r--r--   0 huangqimin   (501) staff       (20)     4851 2023-02-23 06:57:06.000000 django-excel-storage-2.0.8/django_excel_storage/excel_storage.py
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-23 07:21:34.344232 django-excel-storage-2.0.8/django_excel_storage.egg-info/
+-rw-r--r--   0 huangqimin   (501) staff       (20)     4882 2023-02-23 07:21:34.000000 django-excel-storage-2.0.8/django_excel_storage.egg-info/PKG-INFO
+-rw-r--r--   0 huangqimin   (501) staff       (20)      353 2023-02-23 07:21:34.000000 django-excel-storage-2.0.8/django_excel_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)        1 2023-02-23 07:21:34.000000 django-excel-storage-2.0.8/django_excel_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)       43 2023-02-23 07:21:34.000000 django-excel-storage-2.0.8/django_excel_storage.egg-info/requires.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)       21 2023-02-23 07:21:34.000000 django-excel-storage-2.0.8/django_excel_storage.egg-info/top_level.txt
+-rw-r--r--   0 huangqimin   (501) staff       (20)       61 2023-02-23 07:21:34.348261 django-excel-storage-2.0.8/setup.cfg
+-rw-r--r--   0 huangqimin   (501) staff       (20)      994 2023-02-23 07:21:00.000000 django-excel-storage-2.0.8/setup.py
+drwxr-xr-x   0 huangqimin   (501) staff       (20)        0 2023-02-23 07:21:34.345865 django-excel-storage-2.0.8/tests/
+-rw-r--r--   0 huangqimin   (501) staff       (20)     6960 2023-02-23 07:17:30.000000 django-excel-storage-2.0.8/tests/test_django_excel_storage.py
```

### Comparing `django-excel-storage-2.0.6/django_excel_storage/excel_storage.py` & `django-excel-storage-2.0.8/django_excel_storage/excel_storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding:utf-8 -*-
 
 import datetime
 
 from django.core.files.storage import default_storage
 from django.db.models.query import QuerySet
 from django_excel_base import (BytesIO, StringIO, as_csv, as_dict_row_merge_xls, as_list_row_merge_xls,
-                               as_row_merge_xls, as_xls, is_py2)
+                               as_row_merge_xls, as_xls, is_py2, use_xls_or_not)
 from django_six import Support_ValuesQuerySet, ValuesQuerySet
 
 
 # Min (Max. Rows) for Widely Used Excel
 # http://superuser.com/questions/366468/what-is-the-maximum-allowed-rows-in-a-microsoft-excel-xls-or-xlsx
 EXCEL_MAXIMUM_ALLOWED_ROWS = 65536
 # Column Width Limit For ``xlwt``
 # https://github.com/python-excel/xlwt/blob/master/xlwt/Column.py#L22
 EXCEL_MAXIMUM_ALLOWED_COLUMN_WIDTH = 65535
 
 
-def __init__(self, data, output_name='excel_data', format='%Y%m%d%H%M%S', headers=None, force_csv=False, encoding='utf-8-sig', font='', sheet_name='Sheet 1', blanks_for_none=True, auto_adjust_width=True, min_cell_width=1000, vert=0x01, horz=0x01, row_merge=False, list_row_merge=False, dict_row_merge=False, mapping=None):
+def __init__(self, data, output_name='excel_data', format='%Y%m%d%H%M%S', headers=None, force_csv=False, encoding='utf-8-sig', font='', sheet_name='Sheet 1', blanks_for_none=True, auto_adjust_width=True, min_cell_width=1000, vert=0x01, horz=0x01, hvert=0x01, hhorz=0x02, merge_type=None, mapping=None):
     self.data = data
     self.output_name = output_name
     self.format = format
     self.headers = headers
     self.force_csv = force_csv
     self.encoding = encoding
     self.font = font
@@ -34,53 +34,60 @@
     # VERT_CENTER  = 0x01    居中对齐（垂直方向上）
     # VERT_BOTTOM  = 0x02    底端对齐
     # HORZ_LEFT    = 0x01    左端对齐
     # HORZ_CENTER  = 0x02    居中对齐（水平方向上）
     # HORZ_RIGHT   = 0x03    右端对齐
     self.vert = vert
     self.horz = horz
+    self.hvert = hvert
+    self.hhorz = hhorz
     self.mapping = mapping
 
-    if not dict_row_merge:
+    if merge_type != 'dict_row_merge':
         if not isinstance(self.data, dict):
-            self.data = {self.sheet_name: self.data}
+            self.data = {self.sheet_name: {'data': self.data, 'headers': self.headers}}
 
         # Make sure we've got the right type of data to work with
         # ``list index out of range`` if data is ``[]``
         valid_data = True
-        for sheet_name, sheet_data in self.data.items():
+        for sheet_name, sheet_info in self.data.items():
+            sheet_data = sheet_info.get('data') or []
+            sheet_headers = sheet_info.get('headers')
             if Support_ValuesQuerySet and isinstance(sheet_data, ValuesQuerySet):
                 sheet_data = list(sheet_data)
             elif isinstance(sheet_data, QuerySet):
                 sheet_data = list(sheet_data.values())
             if not hasattr(sheet_data, '__getitem__'):
                 valid_data = False
                 break
             if isinstance(sheet_data[0], dict):
-                if headers is None:
-                    headers = list(sheet_data[0].keys())
-                sheet_data = [[row[col] for col in headers] for row in sheet_data]
-                sheet_data.insert(0, headers)
+                if sheet_headers is None:
+                    sheet_headers = list(sheet_data[0].keys())
+                sheet_data = [[row[col] for col in sheet_headers] for row in sheet_data]
             if not hasattr(sheet_data[0], '__getitem__'):
                 valid_data = False
                 break
-            self.data[sheet_name] = sheet_data
+            if sheet_headers and not hasattr(sheet_headers[0], '__getitem__'):
+                valid_data = False
+                break
+            sheet_info['data'] = sheet_data
+            sheet_info['headers'] = sheet_headers
+            self.data[sheet_name] = sheet_info
         assert valid_data is True, 'ExcelStorage requires a sequence of sequences'
 
     self.output = StringIO() if is_py2 else BytesIO()
-    if row_merge:
+    if merge_type == 'row_merge':
         _, file_ext = (self.as_row_merge_xls, 'xls')
-    elif list_row_merge:
+    elif merge_type == 'list_row_merge':
         _, file_ext = (self.as_list_row_merge_xls, 'xls')
-    elif dict_row_merge:
+    elif merge_type == 'dict_row_merge':
         _, file_ext = (self.as_dict_row_merge_xls, 'xls')
     else:
         # Excel has a limit on number of rows; if we have more than that, make a csv
-        use_xls = True if len(self.data) <= self.EXCEL_MAXIMUM_ALLOWED_ROWS and not self.force_csv else False
-        _, file_ext = (self.as_xls, 'xls') if use_xls else (self.as_csv, 'csv')
+        _, file_ext = (self.as_xls, 'xls') if self.use_xls_or_not else (self.as_csv, 'csv')
     self.output.seek(0)
 
     self.file_ext = file_ext
 
 
 def save(self):
     file_name_ext = '_{0}'.format(datetime.datetime.now().strftime(self.format)) if self.format else ''
@@ -93,14 +100,15 @@
     return final_file_name
 
 
 clsdict = {
     'EXCEL_MAXIMUM_ALLOWED_ROWS': EXCEL_MAXIMUM_ALLOWED_ROWS,
     'EXCEL_MAXIMUM_ALLOWED_COLUMN_WIDTH': EXCEL_MAXIMUM_ALLOWED_COLUMN_WIDTH,
     '__init__': __init__,
+    'use_xls_or_not': use_xls_or_not,
     'as_xls': as_xls,
     'as_row_merge_xls': as_row_merge_xls,
     'as_list_row_merge_xls': as_list_row_merge_xls,
     'as_dict_row_merge_xls': as_dict_row_merge_xls,
     'as_csv': as_csv,
     'save': save,
 }
```

### Comparing `django-excel-storage-2.0.6/setup.py` & `django-excel-storage-2.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import with_statement
 
 from setuptools import setup
 
 
-version = '2.0.6'
+version = '2.0.8'
 
 
 setup(
     name='django-excel-storage',
     version=version,
     keywords='django-excel-storage',
     description='Django Excel Storage',
@@ -19,15 +19,15 @@
     url='https://github.com/django-xxx/django-excel-storage',
 
     author='Hackathon',
     author_email='kimi.huang@brightcells.com',
 
     packages=['django_excel_storage'],
     py_modules=[],
-    install_requires=['django-excel-base>=1.0.6', 'django-six>=1.0.4'],
+    install_requires=['django-excel-base>=1.0.7', 'django-six>=1.0.4'],
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
```

### Comparing `django-excel-storage-2.0.6/tests/test_django_excel_storage.py` & `django-excel-storage-2.0.8/tests/test_django_excel_storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         self.content_type_csv = 'text/csv'
         self.content_type_xls = 'application/vnd.ms-excel'
 
         self.sheet_name1 = 'Sheet Name 1'
         self.sheet_name2 = 'Sheet Name 2'
         self.sheet_name3 = 'Sheet Name 3'
 
-        self.sheet_data1 = {'Sheet Name 1': [['Column 1', 'Column 2'], [1, 2], [3, 4]]}
-        self.sheet_data2 = {'Sheet Name 1': [['Column 1', 'Column 2'], [1, [2, 3]], [3, 4]]}
+        self.sheet_data1 = {'Sheet Name 1': {'data': [['Column 1', 'Column 2'], [1, 2], [3, 4]]}}
+        self.sheet_data2 = {'Sheet Name 1': {'data': [['Column 1', 'Column 2'], [1, [2, 3]], [3, 4]]}}
 
         self.headers = ['Column 1', 'Column 2', 'Column 3', 'Column 4', 'Column 5']
         self.mapping = {
             'field_key': 'Column 1',
             'data_key': 'Children 1',
             'next': {
                 'field_key': 'Column 2',
@@ -100,82 +100,82 @@
         xls2 = ExcelStorage(self.data2, 'my_data', font='name SimSum')
         assert isinstance(xls2, ExcelStorage)
 
         # xls3 = ExcelResponse(self.data3, 'my_data', font='name SimSum')
         # assert isinstance(xls3, ExcelStorage)
 
         xls11 = ExcelStorage({
-            self.sheet_name1: self.data1,
+            self.sheet_name1: {'data': self.data1},
         }, 'my_data', font='name SimSum')
         assert isinstance(xls11, ExcelStorage)
 
         xls22 = ExcelStorage({
-            self.sheet_name2: self.data2,
+            self.sheet_name2: {'data': self.data2},
         }, 'my_data', font='name SimSum')
         assert isinstance(xls22, ExcelStorage)
 
     def test_as_row_merge_xls(self):
-        xls1 = ExcelStorage(self.data1, 'my_data', font='name SimSum', row_merge=True)
+        xls1 = ExcelStorage(self.data1, 'my_data', font='name SimSum', merge_type='row_merge')
         assert isinstance(xls1, ExcelStorage)
 
-        xls2 = ExcelStorage(self.data2, 'my_data', font='name SimSum', row_merge=True)
+        xls2 = ExcelStorage(self.data2, 'my_data', font='name SimSum', merge_type='row_merge')
         assert isinstance(xls2, ExcelStorage)
 
-        xls3 = ExcelStorage(self.data3, 'my_data', font='name SimSum', row_merge=True)
+        xls3 = ExcelStorage(self.data3, 'my_data', font='name SimSum', merge_type='row_merge')
         assert isinstance(xls3, ExcelStorage)
 
         xls11 = ExcelStorage({
-            self.sheet_name1: self.data1,
-        }, 'my_data', font='name SimSum', row_merge=True)
+            self.sheet_name1: {'data': self.data1},
+        }, 'my_data', font='name SimSum', merge_type='row_merge')
         assert isinstance(xls11, ExcelStorage)
 
         xls22 = ExcelStorage({
-            self.sheet_name2: self.data2,
-        }, 'my_data', font='name SimSum', row_merge=True)
+            self.sheet_name2: {'data': self.data2},
+        }, 'my_data', font='name SimSum', merge_type='row_merge')
         assert isinstance(xls22, ExcelStorage)
 
         xls33 = ExcelStorage({
-            self.sheet_name3: self.data3,
-        }, 'my_data', font='name SimSum', row_merge=True)
+            self.sheet_name3: {'data': self.data3},
+        }, 'my_data', font='name SimSum', merge_type='row_merge')
         assert isinstance(xls33, ExcelStorage)
 
     def test_as_list_row_merge_xls(self):
-        xls1 = ExcelStorage(self.preprocesseddata, 'my_data', font='name SimSum', list_row_merge=True)
+        xls1 = ExcelStorage(self.preprocesseddata, 'my_data', font='name SimSum', merge_type='list_row_merge')
         assert isinstance(xls1, ExcelStorage)
 
-        xls2 = ExcelStorage(self.preprocesseddata, 'my_data', font='name SimSum', list_row_merge=True, headers=self.headers)
+        xls2 = ExcelStorage(self.preprocesseddata, 'my_data', font='name SimSum', merge_type='list_row_merge', headers=self.headers)
         assert isinstance(xls2, ExcelStorage)
 
         xls11 = ExcelStorage({
-            self.sheet_name1: self.preprocesseddata,
-        }, 'my_data', font='name SimSum', list_row_merge=True)
+            self.sheet_name1: {'data': self.preprocesseddata},
+        }, 'my_data', font='name SimSum', merge_type='list_row_merge')
         assert isinstance(xls11, ExcelStorage)
 
         xls22 = ExcelStorage({
-            self.sheet_name2: self.preprocesseddata,
-        }, 'my_data', font='name SimSum', list_row_merge=True, headers=self.headers)
+            self.sheet_name2: {'data': self.preprocesseddata},
+        }, 'my_data', font='name SimSum', merge_type='list_row_merge', headers=self.headers)
         assert isinstance(xls22, ExcelStorage)
 
     def test_as_dict_row_merge_xls(self):
-        xls1 = ExcelStorage(self.rawdata, 'my_data', font='name SimSum', dict_row_merge=True, mapping=self.mapping)
+        xls1 = ExcelStorage(self.rawdata, 'my_data', font='name SimSum', merge_type='dict_row_merge', mapping=self.mapping)
         assert isinstance(xls1, ExcelStorage)
 
-        xls2 = ExcelStorage(self.rawdata, 'my_data', font='name SimSum', dict_row_merge=True, mapping=self.mapping, headers=self.headers)
+        xls2 = ExcelStorage(self.rawdata, 'my_data', font='name SimSum', merge_type='dict_row_merge', mapping=self.mapping, headers=self.headers)
         assert isinstance(xls2, ExcelStorage)
 
         xls11 = ExcelStorage({
             self.sheet_name2: {
                 'data': self.rawdata,
                 'mapping': self.mapping,
                 'headers': self.headers,
             },
-        }, 'my_data', font='name SimSum', dict_row_merge=True)
+        }, 'my_data', font='name SimSum', merge_type='dict_row_merge')
         assert isinstance(xls11, ExcelStorage)
 
         xls22 = ExcelStorage({
             self.sheet_name2: {
                 'data': self.rawdata,
                 'mapping': self.mapping,
                 'headers': self.headers,
             },
-        }, 'my_data', font='name SimSum', dict_row_merge=True, headers=self.headers)
+        }, 'my_data', font='name SimSum', merge_type='dict_row_merge', headers=self.headers)
         assert isinstance(xls22, ExcelStorage)
```

