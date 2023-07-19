# Comparing `tmp/django-simple-sso.naudit-1.0.5.tar.gz` & `tmp/django-simple-sso.naudit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-sso.naudit-1.0.5.tar", last modified: Wed Jul 28 08:58:04 2021, max compression
+gzip compressed data, was "django-simple-sso.naudit-1.2.1.tar", last modified: Wed Jul 19 15:09:01 2023, max compression
```

## Comparing `django-simple-sso.naudit-1.0.5.tar` & `django-simple-sso.naudit-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.599243 django-simple-sso.naudit-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10164 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8967 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10164 2021-07-28 08:58:04.000000 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-07-28 08:58:04.000000 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 08:58:04.000000 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 08:58:04.000000 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-07-28 08:58:04.000000 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-07-28 08:58:04.000000 django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-28 08:58:04.599243 django-simple-sso.naudit-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/simple_sso/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/simple_sso/sso_client/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_client/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_client/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/0002_consumer_name_max_length.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/0003_token_session.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8499 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/sso_server/server.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/simple_sso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8258 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 08:58:04.595243 django-simple-sso.naudit-1.0.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-07-28 08:57:58.000000 django-simple-sso.naudit-1.0.5/tests/utils/context_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10335 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8967 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10335 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/simple_sso/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0002_consumer_name_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0003_token_redirect_to_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0003_token_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8499 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/utils/context_managers.py
```

### Comparing `django-simple-sso.naudit-1.0.5/LICENSE` & `django-simple-sso.naudit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/PKG-INFO` & `django-simple-sso.naudit-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: django-simple-sso.naudit
-Version: 1.0.5
+Version: 1.2.1
 Summary: Simple SSO for Django
 Home-page: http://github.com/naudit/django-simple-sso
 Author: Rafael Leira
 Author-email: rafael.leira@naudit.es
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.0
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -276,9 +279,7 @@
 .. |coverage| image:: https://codecov.io/gh/divio/django-simple.sso/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/django-simple.sso
 
 .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
     :target: https://pypi.org/project/django-simple.sso/
 .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
     :target: https://www.djangoproject.com/
-
-
```

### Comparing `django-simple-sso.naudit-1.0.5/README.rst` & `django-simple-sso.naudit-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/PKG-INFO` & `django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: django-simple-sso.naudit
-Version: 1.0.5
+Version: 1.2.1
 Summary: Simple SSO for Django
 Home-page: http://github.com/naudit/django-simple-sso
 Author: Rafael Leira
 Author-email: rafael.leira@naudit.es
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.0
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -276,9 +279,7 @@
 .. |coverage| image:: https://codecov.io/gh/divio/django-simple.sso/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/django-simple.sso
 
 .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
     :target: https://pypi.org/project/django-simple.sso/
 .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
     :target: https://www.djangoproject.com/
-
-
```

### Comparing `django-simple-sso.naudit-1.0.5/django_simple_sso.naudit.egg-info/SOURCES.txt` & `django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 django_simple_sso.naudit.egg-info/dependency_links.txt
 django_simple_sso.naudit.egg-info/not-zip-safe
 django_simple_sso.naudit.egg-info/requires.txt
 django_simple_sso.naudit.egg-info/top_level.txt
 simple_sso/__init__.py
 simple_sso/models.py
 simple_sso/settings.py
+simple_sso/signals.py
 simple_sso/utils.py
 simple_sso/sso_client/__init__.py
 simple_sso/sso_client/apps.py
 simple_sso/sso_client/client.py
 simple_sso/sso_client/middleware.py
-simple_sso/sso_client/models.py
 simple_sso/sso_server/__init__.py
 simple_sso/sso_server/apps.py
 simple_sso/sso_server/models.py
 simple_sso/sso_server/server.py
 simple_sso/sso_server/migrations/0001_initial.py
 simple_sso/sso_server/migrations/0002_consumer_name_max_length.py
+simple_sso/sso_server/migrations/0003_token_redirect_to_max_length.py
 simple_sso/sso_server/migrations/0003_token_session.py
 simple_sso/sso_server/migrations/__init__.py
 tests/__init__.py
 tests/settings.py
 tests/test_core.py
 tests/test_migrations.py
 tests/urls.py
```

### Comparing `django-simple-sso.naudit-1.0.5/setup.py` & `django-simple-sso.naudit-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from simple_sso import __version__
 
 
 REQUIREMENTS = [
     'Django>=2.2',
     'itsdangerous~=2.0',
-    'webservices[django]',
+    'webservices.naudit[django]',
 ]
 
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
@@ -19,18 +19,22 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Framework :: Django',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
+    'Framework :: Django :: 4.0',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
 ]
```

### Comparing `django-simple-sso.naudit-1.0.5/simple_sso/sso_client/client.py` & `django-simple-sso.naudit-1.2.1/simple_sso/sso_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import copy
 from urllib.parse import urlparse, urlunparse, urljoin, urlencode
 
 from django.urls import re_path
 from django.contrib.auth import login
 from django.contrib.auth.backends import ModelBackend
 from django.contrib.auth.models import Group, User
 from django.http import HttpResponseRedirect
@@ -117,16 +118,18 @@
             server_groups = user_data['groups']
             del user_data['groups']
 
         # Build the base user
         try:
             user = User.objects.get(username=user_data['username'])
             # Update user data, excluding username changes
-            del user_data['username']
-            for _attr, _val in user_data.items():
+            # Work on copied _tmp dict to keep an untouched user_data
+            user_data_tmp = copy(user_data)
+            del user_data_tmp['username']
+            for _attr, _val in user_data_tmp.items():
                 setattr(user, _attr, _val)
         except User.DoesNotExist:
             user = User(**user_data)
         user.set_unusable_password()
 
         user.save()
```

### Comparing `django-simple-sso.naudit-1.0.5/simple_sso/sso_client/middleware.py` & `django-simple-sso.naudit-1.2.1/simple_sso/sso_client/middleware.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/0001_initial.py` & `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/simple_sso/sso_server/migrations/0003_token_session.py` & `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0003_token_session.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/simple_sso/sso_server/models.py` & `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,24 +49,14 @@
 
     def rotate_keys(self):
         self.secret = ConsumerSecretKeyGenerator('private_key')()
         self.key = ConsumerSecretKeyGenerator('public_key')()
         self.save()
 
 
-def logout_token(sender, request, **kwargs):
-    """
-    A signal receiver which removes a token when its users logs out.
-    """
-    tokens = Token.objects.select_related('session').filter(session__session_key=request.session.session_key)
-
-    for token in tokens:
-        token.delete()
-
-
 class Token(models.Model):
     consumer = models.ForeignKey(
         Consumer,
         related_name='tokens',
         on_delete=models.CASCADE,
     )
     request_token = models.CharField(
@@ -74,15 +64,15 @@
         default=TokenSecretKeyGenerator('request_token')
     )
     access_token = models.CharField(
         unique=True, max_length=64,
         default=TokenSecretKeyGenerator('access_token')
     )
     timestamp = models.DateTimeField(default=timezone.now)
-    redirect_to = models.CharField(max_length=255)
+    redirect_to = models.CharField(max_length=1023)
     user = models.ForeignKey(
         getattr(settings, 'AUTH_USER_MODEL', 'auth.User'),
         null=True,
         on_delete=models.CASCADE,
     )
     session = models.ForeignKey(
         Session,
```

### Comparing `django-simple-sso.naudit-1.0.5/simple_sso/sso_server/server.py` & `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/server.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/tests/settings.py` & `django-simple-sso.naudit-1.2.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/tests/test_core.py` & `django-simple-sso.naudit-1.2.1/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,48 +143,13 @@
         with UserLoginContext(self, server_user):
             # Second login
             self.client.get(reverse('simple-sso-login'), follow=True)
             client_user = get_user(self.client)
             for key in ['username', 'email', 'first_name', 'last_name']:
                 self.assertEqual(getattr(client_user, key), getattr(server_user, key))
 
-    def test_user_groups(self):
-        """ User data update test
-
-        Tests whether sso server user data changes will be forwared to the client on the user's next login.
-
-        """
-        USERNAME = PASSWORD = 'myuser'
-        server_user = User.objects.create_user(
-            USERNAME,
-            'bob@bobster.org',
-            PASSWORD
-        )
-        test_group, created = Group.objects.get_or_create(name='SSO_SUPERADMIN')
-        server_user.groups.add(test_group)
-
-        self._get_consumer()
-
-        with UserLoginContext(self, server_user):
-            # First login
-            # try logging in and auto-follow all 302s
-            self.client.get(reverse('simple-sso-login'), follow=True)
-            # check the user
-            client_user = get_user(self.client)
-            for key in ['username', 'email', 'groups']:
-                self.assertEqual(getattr(client_user, key), getattr(server_user, key))
-
-            # Check the groups
-            client_groups = client_user.groups.all()
-            server_groups = server_user.groups.all()
-
-            # NOTE: This test does/tests anything, as DB is shared across client/server so on .all operation always groups are present without anything special.
-            # If you are reading this and know how to implement a "good" test, please, feel free to PR.
-            for group in server_groups:
-                self.assertTrue(group in client_groups)
-
     def test_custom_keygen(self):
         # WARNING: The following test uses a key generator function that is
         # highly insecure and should never under any circumstances be used in
         # a production enivornment
         with SettingsOverride(SIMPLE_SSO_KEYGENERATOR=lambda length: 'test'):
             self.assertEqual(gen_secret_key(40), 'test')
```

### Comparing `django-simple-sso.naudit-1.0.5/tests/test_migrations.py` & `django-simple-sso.naudit-1.2.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/tests/urls.py` & `django-simple-sso.naudit-1.2.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.0.5/tests/utils/context_managers.py` & `django-simple-sso.naudit-1.2.1/tests/utils/context_managers.py`

 * *Files identical despite different names*

