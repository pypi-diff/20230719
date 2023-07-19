# Comparing `tmp/django_dynamic_storage-0.1.4.tar.gz` & `tmp/django_dynamic_storage-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_storage-0.1.4.tar", max compression
+gzip compressed data, was "django_dynamic_storage-0.1.5.tar", max compression
```

## Comparing `django_dynamic_storage-0.1.4.tar` & `django_dynamic_storage-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3241 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/__init__.py
--rw-r--r--   0        0        0     5418 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/models.py
--rw-r--r--   0        0        0      120 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/signals.py
--rw-r--r--   0        0        0     1492 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/storage.py
--rw-r--r--   0        0        0     1064 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/test/storage.py
--rw-r--r--   0        0        0     1188 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4409 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3544 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/dynamic_storage/__init__.py
+-rw-r--r--   0        0        0     5954 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/dynamic_storage/models.py
+-rw-r--r--   0        0        0      120 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/dynamic_storage/signals.py
+-rw-r--r--   0        0        0     1492 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/dynamic_storage/storage.py
+-rw-r--r--   0        0        0     1064 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/dynamic_storage/test/storage.py
+-rw-r--r--   0        0        0     1234 2023-07-19 14:54:45.888949 django_dynamic_storage-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4758 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.5/PKG-INFO
```

### Comparing `django_dynamic_storage-0.1.4/README.md` & `django_dynamic_storage-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 ![tox CI](https://github.com/engAmirEng/django-dynamic-storage/actions/workflows/tox.yml/badge.svg)
+![PyPi Version](https://img.shields.io/pypi/v/django-dynamic-storage)
 ![Python Versions](https://img.shields.io/pypi/pyversions/poetry)
-![Python Versionfs](https://img.shields.io/badge/django-2.2_|_3.0_|_3.1_|_3.2_|_4.0_|_4.1_|_4.2-green)
+![Django Versions](https://img.shields.io/badge/django-2.2_|_3.0_|_3.1_|_3.2_|_4.0_|_4.1_|_4.2-green)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/engAmirEng/django-dynamic-storage/main.svg)](https://results.pre-commit.ci/latest/github/engAmirEng/django-dynamic-storage/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## django-dynamic-storage
 
+Have you ever wanted not to store every instance of FileFileds or ImageFileds of a model in one storage or one bucket of a storage?
+
+Now you can, because I wanted that for [my project](https://github.com/SayIfOrg/say_wagtail).
+
 ### prerequisites:
 
-If your django version is earlier than 3.1 (<=3.0) then your database should be PostgreSQL otherwise you are good to go
+If your django version is earlier than 3.1 (<=3.0) then your database should be PostgreSQL otherwise you are good to go.
 
 ### Usage:
 
 ```plaintext
 pip install django-dynamic-storage
 ```
 
@@ -28,15 +33,15 @@
 		"""
 		here you should return a dictionary of key value pairs that 
 		later django-dynamic-storage could instantiate this class with
 		"""
 		return {"named_param1": self.named_param1, "named_param2": self.named_param2, ...}
 ```
 
-`AnyStorage` can be a storage that you define yourself or import from [django-storages](https://pypi.org/project/django-storages/)
+`AnyStorage` can be a storage that you define yourself or import from [django-storages](https://pypi.org/project/django-storages/).
 
 in models.py:
 
 ```python
 from dynamic_storage.models import DynamicFileField, DynamicImageField
 
 class MyModel(models.Model):
@@ -70,21 +75,21 @@
 , to_storage
 , *args,
  **kwargs
 ):
     if not to_storage:
     	# destination_storage is not set, so we set it here
         field_file.destination_storage = MyDynamicStorage(named_param1="something", named_param2="another_thing")
-	elif to_storage == wrong_storage:
+    elif to_storage == wrong_storage:
 		# override the destination_storage set earlier
 		field_file.destination_storage = MyAnotherDynamicStorage(named_param1="foo", named_param2="bar")
 ```
 
 #### Performance penalty?!
 
 Not even a bit!
 
-#### how?
+#### HOW?
 
-we are just using the django's built in `JsonField` instead of `CharField`  to store more data (init\_params output) in addition to the path to the file,
+We are just using the django's built in `JsonField` instead of `CharField`  to store more data (init\_params output) in addition to the path to the file.
 
-so no extra queries, no extra steps, no performance penalty
+so no extra queries, no extra steps, no performance penalty.
```

### Comparing `django_dynamic_storage-0.1.4/dynamic_storage/models.py` & `django_dynamic_storage-0.1.5/dynamic_storage/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,19 +109,33 @@
 class DynamicFileField(JSONField, models.FileField):
     """FileField with json db representation that contain info for dynamic behavior"""
 
     attr_class = DynamicFieldFile
 
     descriptor_class = DynamicFileDescriptor
 
+    call_prep_or_db_pred = (
+        "db_prep" if (4, 2, 0) <= django.VERSION[:3] < (4, 2, 2) else "prep"
+    )
+
+    def get_prep_value(self, value):
+        if self.call_prep_or_db_pred == "prep":
+            if value is None:
+                return value
+            if not isinstance(value, dict):
+                value = value.dictionary()
+            return JSONField.get_prep_value(self, value)
+        return super(DynamicFileField, self).get_prep_value(value)
+
     def get_db_prep_value(self, value, connection, prepared=False):
-        if value is None:
-            return value
-        if not isinstance(value, dict):
-            value = value.dictionary()
+        if self.call_prep_or_db_pred == "db_prep":
+            if value is None:
+                return value
+            if not isinstance(value, dict):
+                value = value.dictionary()
         return super(DynamicFileField, self).get_db_prep_value(
             value, connection, prepared
         )
 
     def formfield(self, **kwargs):
         return models.FileField.formfield(self, **kwargs)
```

### Comparing `django_dynamic_storage-0.1.4/dynamic_storage/storage.py` & `django_dynamic_storage-0.1.5/dynamic_storage/storage.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_storage-0.1.4/dynamic_storage/test/storage.py` & `django_dynamic_storage-0.1.5/dynamic_storage/test/storage.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_storage-0.1.4/pyproject.toml` & `django_dynamic_storage-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-dynamic-storage"
-version = "0.1.4"
-description = "Use and choose storages at runtime based on your logic"
+version = "0.1.5"
+description = "Use and choose storages at runtime based on your logic for each model FileField instance separately."
 authors = ["Amir Khalife <eng.amir.bu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/engAmirEng/django-dynamic-storage"
 keywords = ["django", "django-storages", "djangostorage"]
 classifiers = [
     "Framework :: Django",
```

### Comparing `django_dynamic_storage-0.1.4/PKG-INFO` & `django_dynamic_storage-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-dynamic-storage
-Version: 0.1.4
-Summary: Use and choose storages at runtime based on your logic
+Version: 0.1.5
+Summary: Use and choose storages at runtime based on your logic for each model FileField instance separately.
 Home-page: https://github.com/engAmirEng/django-dynamic-storage
 License: Apache-2.0
 Keywords: django,django-storages,djangostorage
 Author: Amir Khalife
 Author-email: eng.amir.bu@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Framework :: Django
@@ -24,25 +24,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=2.2,<5)
 Project-URL: Repository, https://github.com/engAmirEng/django-dynamic-storage
 Description-Content-Type: text/markdown
 
 ![tox CI](https://github.com/engAmirEng/django-dynamic-storage/actions/workflows/tox.yml/badge.svg)
+![PyPi Version](https://img.shields.io/pypi/v/django-dynamic-storage)
 ![Python Versions](https://img.shields.io/pypi/pyversions/poetry)
-![Python Versionfs](https://img.shields.io/badge/django-2.2_|_3.0_|_3.1_|_3.2_|_4.0_|_4.1_|_4.2-green)
+![Django Versions](https://img.shields.io/badge/django-2.2_|_3.0_|_3.1_|_3.2_|_4.0_|_4.1_|_4.2-green)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/engAmirEng/django-dynamic-storage/main.svg)](https://results.pre-commit.ci/latest/github/engAmirEng/django-dynamic-storage/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## django-dynamic-storage
 
+Have you ever wanted not to store every instance of FileFileds or ImageFileds of a model in one storage or one bucket of a storage?
+
+Now you can, because I wanted that for [my project](https://github.com/SayIfOrg/say_wagtail).
+
 ### prerequisites:
 
-If your django version is earlier than 3.1 (<=3.0) then your database should be PostgreSQL otherwise you are good to go
+If your django version is earlier than 3.1 (<=3.0) then your database should be PostgreSQL otherwise you are good to go.
 
 ### Usage:
 
 ```plaintext
 pip install django-dynamic-storage
 ```
 
@@ -57,15 +62,15 @@
 		"""
 		here you should return a dictionary of key value pairs that 
 		later django-dynamic-storage could instantiate this class with
 		"""
 		return {"named_param1": self.named_param1, "named_param2": self.named_param2, ...}
 ```
 
-`AnyStorage` can be a storage that you define yourself or import from [django-storages](https://pypi.org/project/django-storages/)
+`AnyStorage` can be a storage that you define yourself or import from [django-storages](https://pypi.org/project/django-storages/).
 
 in models.py:
 
 ```python
 from dynamic_storage.models import DynamicFileField, DynamicImageField
 
 class MyModel(models.Model):
@@ -99,21 +104,21 @@
 , to_storage
 , *args,
  **kwargs
 ):
     if not to_storage:
     	# destination_storage is not set, so we set it here
         field_file.destination_storage = MyDynamicStorage(named_param1="something", named_param2="another_thing")
-	elif to_storage == wrong_storage:
+    elif to_storage == wrong_storage:
 		# override the destination_storage set earlier
 		field_file.destination_storage = MyAnotherDynamicStorage(named_param1="foo", named_param2="bar")
 ```
 
 #### Performance penalty?!
 
 Not even a bit!
 
-#### how?
+#### HOW?
 
-we are just using the django's built in `JsonField` instead of `CharField`  to store more data (init\_params output) in addition to the path to the file,
+We are just using the django's built in `JsonField` instead of `CharField`  to store more data (init\_params output) in addition to the path to the file.
 
-so no extra queries, no extra steps, no performance penalty
+so no extra queries, no extra steps, no performance penalty.
```

