# Comparing `tmp/nanorm-1.9.8.tar.gz` & `tmp/nanorm-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanorm-1.9.8.tar", last modified: Mon Mar  4 09:14:55 2019, max compression
+gzip compressed data, was "dist/nanorm-1.9.9.tar", last modified: Mon Mar  4 14:11:32 2019, max compression
```

## Comparing `nanorm-1.9.8.tar` & `nanorm-1.9.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 taojy123   (501) staff       (20)        0 2019-03-04 09:14:55.000000 nanorm-1.9.8/
--rw-r--r--   0 taojy123   (501) staff       (20)     2532 2019-03-04 09:14:55.000000 nanorm-1.9.8/PKG-INFO
--rw-r--r--   0 taojy123   (501) staff       (20)     4625 2019-03-04 09:10:33.000000 nanorm-1.9.8/nanorm_test.py
-drwxr-xr-x   0 taojy123   (501) staff       (20)        0 2019-03-04 09:14:55.000000 nanorm-1.9.8/nanorm.egg-info/
--rw-r--r--   0 taojy123   (501) staff       (20)     2532 2019-03-04 09:14:54.000000 nanorm-1.9.8/nanorm.egg-info/PKG-INFO
--rw-r--r--   0 taojy123   (501) staff       (20)      163 2019-03-04 09:14:55.000000 nanorm-1.9.8/nanorm.egg-info/SOURCES.txt
--rw-r--r--   0 taojy123   (501) staff       (20)       19 2019-03-04 09:14:54.000000 nanorm-1.9.8/nanorm.egg-info/top_level.txt
--rw-r--r--   0 taojy123   (501) staff       (20)        1 2019-03-04 09:14:54.000000 nanorm-1.9.8/nanorm.egg-info/dependency_links.txt
--rw-r--r--   0 taojy123   (501) staff       (20)     1620 2019-03-04 09:13:21.000000 nanorm-1.9.8/README.md
--rw-r--r--   0 taojy123   (501) staff       (20)      771 2018-08-13 02:41:45.000000 nanorm-1.9.8/setup.py
--rw-r--r--   0 taojy123   (501) staff       (20)       38 2019-03-04 09:14:55.000000 nanorm-1.9.8/setup.cfg
--rw-r--r--   0 taojy123   (501) staff       (20)    11675 2019-03-04 09:11:51.000000 nanorm-1.9.8/nanorm.py
+drwxr-xr-x   0 taojy123   (501) staff       (20)        0 2019-03-04 14:11:32.000000 nanorm-1.9.9/
+-rw-r--r--   0 taojy123   (501) staff       (20)     2492 2019-03-04 14:11:32.000000 nanorm-1.9.9/PKG-INFO
+-rw-r--r--   0 taojy123   (501) staff       (20)     4931 2019-03-04 14:09:00.000000 nanorm-1.9.9/nanorm_test.py
+drwxr-xr-x   0 taojy123   (501) staff       (20)        0 2019-03-04 14:11:32.000000 nanorm-1.9.9/nanorm.egg-info/
+-rw-r--r--   0 taojy123   (501) staff       (20)     2492 2019-03-04 14:11:32.000000 nanorm-1.9.9/nanorm.egg-info/PKG-INFO
+-rw-r--r--   0 taojy123   (501) staff       (20)      163 2019-03-04 14:11:32.000000 nanorm-1.9.9/nanorm.egg-info/SOURCES.txt
+-rw-r--r--   0 taojy123   (501) staff       (20)       19 2019-03-04 14:11:32.000000 nanorm-1.9.9/nanorm.egg-info/top_level.txt
+-rw-r--r--   0 taojy123   (501) staff       (20)        1 2019-03-04 14:11:32.000000 nanorm-1.9.9/nanorm.egg-info/dependency_links.txt
+-rw-r--r--   0 taojy123   (501) staff       (20)     1620 2019-03-04 09:13:21.000000 nanorm-1.9.9/README.md
+-rw-r--r--   0 taojy123   (501) staff       (20)      771 2018-08-13 02:41:45.000000 nanorm-1.9.9/setup.py
+-rw-r--r--   0 taojy123   (501) staff       (20)       59 2019-03-04 14:11:32.000000 nanorm-1.9.9/setup.cfg
+-rw-r--r--   0 taojy123   (501) staff       (20)    12687 2019-03-04 14:10:28.000000 nanorm-1.9.9/nanorm.py
```

### Comparing `nanorm-1.9.8/PKG-INFO` & `nanorm-1.9.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: nanorm
-Version: 1.9.8
+Version: 1.9.9
 Summary: A simple ORM framework for Python ( Nano ORM )
 Home-page: https://github.com/taojy123/nanorm
 Author: Tao Jiayuan
 Author-email: taojy123@163.com
 License: MIT
 Description: Nanorm : A simple ORM of Python
         =========================================
@@ -60,8 +60,7 @@
         
         
 Keywords: orm namo mini sample database sqlite nanorm nanoorm
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
```

### Comparing `nanorm-1.9.8/nanorm_test.py` & `nanorm-1.9.9/nanorm_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 # -*- coding: utf-8 -*-
 
 # ==================================
 # testcase and user guide with Nanorm
 # ==================================
 
 from nanorm import *
+import datetime
 
 
 class Area(Model):
     name = CharField()
 
 
 class User(Model):
     name = CharField(128)           # CharField default="" max_length=255
     age = IntegerField()            # IntegerField default=0
     score = FloatField(default=6.8) # FloatField default=0.0
     sex = BooleanField()            # BooleanField default=True
-    area = ForeignKey(Area)         # ForeignKey can not be null
-    leader = SelfForeignKey() 
+    area = ForeignKey(Area)         # ForeignKey
+    leader = SelfForeignKey()
+    join_date = DateField()
+    finish_time = DateTimeField()
+
 
     def __str__(self):
         return "%s_%s_%s_%s_%s" % (self.__class__.__name__, self.id, self.name, self.age, self.sex)
 
 
 
 # ==============================================
@@ -160,15 +164,29 @@
 auto_commit_open()              # open auto commit, and commit at the same time
 
 assert len(Area.gets()) == 4
 
 # ==============================================
 
 
+now = datetime.datetime.now()
+
+sandy.join_date = now.date()
+sandy.finish_time = now
+sandy.save()
+
+sandy = sandy.refresh()
+
 
+assert sandy.join_date == now.date()
+assert sandy.finish_time == now
+
+
+
+# ==============================================
 
 
 
 # ==============================================
 
 print(User.gets())
 print("Success!")
```

### Comparing `nanorm-1.9.8/nanorm.egg-info/PKG-INFO` & `nanorm-1.9.9/nanorm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: nanorm
-Version: 1.9.8
+Version: 1.9.9
 Summary: A simple ORM framework for Python ( Nano ORM )
 Home-page: https://github.com/taojy123/nanorm
 Author: Tao Jiayuan
 Author-email: taojy123@163.com
 License: MIT
 Description: Nanorm : A simple ORM of Python
         =========================================
@@ -60,8 +60,7 @@
         
         
 Keywords: orm namo mini sample database sqlite nanorm nanoorm
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
```

### Comparing `nanorm-1.9.8/README.md` & `nanorm-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `nanorm-1.9.8/setup.py` & `nanorm-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `nanorm-1.9.8/nanorm.py` & `nanorm-1.9.9/nanorm.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 # ==================================
 # Nanorm - Nano ORM
 # ==================================
 
 import sqlite3
 import time
+import datetime
 try:
     import thread
 except ImportError as e:
     # Compatible with python3
     import _thread as thread
     unicode = str
 
 
-__VERSION__ = "1.9.8"
+__VERSION__ = "1.9.9"
 
 """
 New Feature
 
+1.9.9:
+1. add DateTimeField and DateField
+
 1.9.8:
 1. add SelfForeignKey field
 
 1.9.7:
 1. add thread lock
 """
 
@@ -89,18 +93,18 @@
         print('---------------------------------')
         raise e
 
 
 class Field(object):
     field_type = ""
     field_level = 0
-    default = ""
+    default = None
 
     def field_sql(self, field_name):
-        return '"%s" %s' % (field_name, self.field_type)
+        return '"%s" %s null' % (field_name, self.field_type)
 
 
 class CharField(Field):
     def __init__(self, max_length=255, default=""):
         self.field_type = "varchar(%d)" % max_length
         self.default = default
         self.max_length = max_length
@@ -120,14 +124,26 @@
 
 class BooleanField(Field):
     def __init__(self, default=True):
         self.field_type = "boolean"
         self.default = default
 
 
+class DateField(Field):
+    def __init__(self, default=None):
+        self.field_type = "date"
+        self.default = default
+
+
+class DateTimeField(Field):
+    def __init__(self, default=None):
+        self.field_type = "datetime"
+        self.default = default
+
+
 class ForeignKey(Field):
     def __init__(self, model_class):
         self.field_type = "foreignkey"
         self.field_level = 1
         self.model_class = model_class
 
     def field_sql(self, field_name):
@@ -181,29 +197,38 @@
                 names.append("`%s`" % name)
         return names
 
     @property
     def field_values(self):
         values = []
         for name in self.field_names:
-            value = getattr(self, name.replace("`", ""))
-            if isinstance(value, Model):
-                if isinstance(value, self.__class__) and self.id:
-                    assert self.id != value.id, 'SelfForeignKey can not set the self instance!'
-                value = value.id
+            name = name.replace("`", "")
+            value = getattr(self, name)
+            field = getattr(self.__class__, name)
+
             if isinstance(value, str) or isinstance(value, unicode):
                 value = value.replace("'", "''")
                 try:
                     value = value.decode("gbk")
                 except Exception as e:
                     pass
                 try:
                     value = value.decode("utf8")
                 except Exception as e:
                     pass
+            if isinstance(value, Model):
+                value = value.id
+
+            if field.field_type == 'datetime' and value:
+                value = value.strftime('%Y-%m-%d %H:%M:%S.%f')
+            if field.field_type == 'date' and value:
+                value = value.strftime('%Y-%m-%d')
+            if field.field_type == 'selfforeignkey' and value:
+                assert self.id != value, 'SelfForeignKey can not set the self instance!'
+
             values.append("'%s'" % value)
         return values
 
     def insert(self):
         cu = get_cursor()
 
         field_names_sql = ", ".join(self.field_names)
@@ -238,14 +263,18 @@
 
     def delete(self):
         cu = get_cursor()
         sql = "delete from `%s` where id = %d" % (self.table_name, self.id)
         execute_sql(cu, sql)
         db_commit()
 
+    def refresh(self):
+        assert self.id, 'only saved instance can be refreshed'
+        return self.__class__.get(id=self.id)
+
     @classmethod
     def try_create_table(cls):
         table_name = cls.__name__.lower()
 
         cu = get_cursor()
         sql = "select * from sqlite_master where type='table' AND name='%s';" % table_name
         execute_sql(cu, sql)
@@ -351,31 +380,36 @@
         rid = r[0]
         ob = self.model_class(rid=rid)
         for i in range(1, len(r)):
             name = self.field_names[i - 1]
             field = getattr(self.model_class, name.replace("`", ""))
 
             if field.field_level == 0:
+                value = r[i]
+                value = None if value == 'None' else value
+
                 if field.field_type == "boolean":
-                    value = eval(r[i])
+                    value = eval(value)
                     try:
                         value = bool(value)
                     except Exception as e:
                         pass
-                else:
-                    value = r[i]
+                if field.field_type == "datetime" and value:
+                    value = datetime.datetime.strptime(value, '%Y-%m-%d %H:%M:%S.%f') if value else None
+                if field.field_type == "date" and value:
+                    value = datetime.datetime.strptime(value, '%Y-%m-%d').date() if value else None
+
             elif field.field_level == 1:
-                if field.field_type in ["foreignkey", "selfforeignkey"]:
-                    if field.field_type == "selfforeignkey":
-                        field.model_class = self.model_class
-                    fid = r[i]
-                    if fid:
-                        value = field.model_class.get(id=fid)
-                    else:
-                        value = None
+                if field.field_type == "selfforeignkey":
+                    field.model_class = self.model_class
+                fid = r[i]
+                if fid:
+                    value = field.model_class.get(id=fid)
+                else:
+                    value = None
 
             setattr(ob, name.replace("`", ""), value)
         return ob
 
     def all(self):
         cu = get_cursor()
         sql = self.query_sql
```

