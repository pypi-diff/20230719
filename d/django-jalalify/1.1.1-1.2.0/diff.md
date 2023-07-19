# Comparing `tmp/django-jalalify-1.1.1.tar.gz` & `tmp/django-jalalify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jalalify-1.1.1.tar", last modified: Sat Jun 10 21:13:32 2023, max compression
+gzip compressed data, was "django-jalalify-1.2.0.tar", last modified: Wed Jul 19 06:46:46 2023, max compression
```

## Comparing `django-jalalify-1.1.1.tar` & `django-jalalify-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:13:32.367201 django-jalalify-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-10 21:13:32.367201 django-jalalify-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:13:32.363201 django-jalalify-1.1.1/django_jalalify/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:13:32.367201 django-jalalify-1.1.1/django_jalalify/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/timezone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/django_jalalify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:13:32.363201 django-jalalify-1.1.1/django_jalalify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-10 21:13:32.000000 django-jalalify-1.1.1/django_jalalify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-10 21:13:32.000000 django-jalalify-1.1.1/django_jalalify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 21:13:32.000000 django-jalalify-1.1.1/django_jalalify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 21:13:32.000000 django-jalalify-1.1.1/django_jalalify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 21:13:32.000000 django-jalalify-1.1.1/django_jalalify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-10 21:13:32.367201 django-jalalify-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-10 21:13:20.000000 django-jalalify-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/django_jalalify/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/django_jalalify/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/admin/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/django_jalalify/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/django_jalalify/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/templatetags/rangefilter_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/django_jalalify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/django_jalalify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-19 06:46:46.000000 django-jalalify-1.2.0/django_jalalify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-19 06:46:46.000000 django-jalalify-1.2.0/django_jalalify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:46:46.000000 django-jalalify-1.2.0/django_jalalify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 06:46:46.000000 django-jalalify-1.2.0/django_jalalify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 06:46:46.000000 django-jalalify-1.2.0/django_jalalify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-19 06:46:46.945601 django-jalalify-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-19 06:46:33.000000 django-jalalify-1.2.0/setup.py
```

### Comparing `django-jalalify-1.1.1/LICENSE` & `django-jalalify-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-jalalify-1.1.1/PKG-INFO` & `django-jalalify-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jalalify
-Version: 1.1.1
+Version: 1.2.0
 Summary: Pluggable django app to provide some utilities for jalali solar calendar for your Django projects.
 Home-page: https://github.com/javadnikbakht/django-jalalify
 Author: Mohammad Javad Nikbakht
 Author-email: javadnikbakht@mail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-jalalify-1.1.1/django_jalalify/fields.py` & `django-jalalify-1.2.0/django_jalalify/fields.py`

 * *Files identical despite different names*

### Comparing `django-jalalify-1.1.1/django_jalalify/filters.py` & `django-jalalify-1.2.0/django_jalalify/filters.py`

 * *Files identical despite different names*

### Comparing `django-jalalify-1.1.1/django_jalalify/tests.py` & `django-jalalify-1.2.0/django_jalalify/tests.py`

 * *Files identical despite different names*

### Comparing `django-jalalify-1.1.1/django_jalalify/timezone.py` & `django-jalalify-1.2.0/django_jalalify/timezone.py`

 * *Files identical despite different names*

### Comparing `django-jalalify-1.1.1/django_jalalify/utils.py` & `django-jalalify-1.2.0/django_jalalify/utils.py`

 * *Files identical despite different names*

### Comparing `django-jalalify-1.1.1/django_jalalify.egg-info/PKG-INFO` & `django-jalalify-1.2.0/django_jalalify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jalalify
-Version: 1.1.1
+Version: 1.2.0
 Summary: Pluggable django app to provide some utilities for jalali solar calendar for your Django projects.
 Home-page: https://github.com/javadnikbakht/django-jalalify
 Author: Mohammad Javad Nikbakht
 Author-email: javadnikbakht@mail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-jalalify-1.1.1/django_jalalify.egg-info/SOURCES.txt` & `django-jalalify-1.2.0/django_jalalify.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,12 @@
 django_jalalify/timezone.py
 django_jalalify/utils.py
 django_jalalify.egg-info/PKG-INFO
 django_jalalify.egg-info/SOURCES.txt
 django_jalalify.egg-info/dependency_links.txt
 django_jalalify.egg-info/requires.txt
 django_jalalify.egg-info/top_level.txt
-django_jalalify/migrations/__init__.py
+django_jalalify/admin/__init__.py
+django_jalalify/admin/filters.py
+django_jalalify/migrations/__init__.py
+django_jalalify/templatetags/__init__.py
+django_jalalify/templatetags/rangefilter_compat.py
```

### Comparing `django-jalalify-1.1.1/setup.cfg` & `django-jalalify-1.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-jalalify
-version = 1.1.1
+version = 1.2.0
 description = Pluggable django app to provide some utilities for jalali solar calendar for your Django projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/javadnikbakht/django-jalalify
 author = Mohammad Javad Nikbakht
 author_email = javadnikbakht@mail.com
 license = GNU General Public License v3 (GPLv3)
```

