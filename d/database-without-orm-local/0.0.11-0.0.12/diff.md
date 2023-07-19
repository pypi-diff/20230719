# Comparing `tmp/database-without-orm-local-0.0.11.tar.gz` & `tmp/database-without-orm-local-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-without-orm-local-0.0.11.tar", last modified: Tue Jul 18 12:38:30 2023, max compression
+gzip compressed data, was "database-without-orm-local-0.0.12.tar", last modified: Wed Jul 19 16:02:07 2023, max compression
```

## Comparing `database-without-orm-local-0.0.11.tar` & `database-without-orm-local-0.0.12.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:38:30.634686 database-without-orm-local-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:38:06.000000 database-without-orm-local-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 12:38:30.634686 database-without-orm-local-0.0.11/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:38:30.634686 database-without-orm-local-0.0.11/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:38:06.000000 database-without-orm-local-0.0.11/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-18 12:38:06.000000 database-without-orm-local-0.0.11/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:38:30.634686 database-without-orm-local-0.0.11/database_without_orm_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 12:38:30.000000 database-without-orm-local-0.0.11/database_without_orm_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 12:38:30.000000 database-without-orm-local-0.0.11/database_without_orm_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:38:30.000000 database-without-orm-local-0.0.11/database_without_orm_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 12:38:30.000000 database-without-orm-local-0.0.11/database_without_orm_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-18 12:38:06.000000 database-without-orm-local-0.0.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:38:30.634686 database-without-orm-local-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-18 12:38:06.000000 database-without-orm-local-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:02:07.730109 database-without-orm-local-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 16:01:43.000000 database-without-orm-local-0.0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-19 16:02:07.730109 database-without-orm-local-0.0.12/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:02:07.726109 database-without-orm-local-0.0.12/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 16:01:43.000000 database-without-orm-local-0.0.12/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-19 16:01:43.000000 database-without-orm-local-0.0.12/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:02:07.730109 database-without-orm-local-0.0.12/database_without_orm_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-19 16:02:07.000000 database-without-orm-local-0.0.12/database_without_orm_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-19 16:02:07.000000 database-without-orm-local-0.0.12/database_without_orm_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 16:02:07.000000 database-without-orm-local-0.0.12/database_without_orm_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 16:02:07.000000 database-without-orm-local-0.0.12/database_without_orm_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-19 16:01:43.000000 database-without-orm-local-0.0.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 16:02:07.730109 database-without-orm-local-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-19 16:01:43.000000 database-without-orm-local-0.0.12/setup.py
```

### Comparing `database-without-orm-local-0.0.11/circles_local_database_python/database.py` & `database-without-orm-local-0.0.12/circles_local_database_python/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import mysql.connector
 import os
 from dotenv import load_dotenv
-from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
+from logger_local_python_package.localLogger import _local_logger as local_logger
 load_dotenv()
 
-local_logger=_Local_Logger
+
 
 
 class database():
     
     def connect_to_database(self):
         try:
             host=os.getenv("RDS_HOSTNAME")
```

### Comparing `database-without-orm-local-0.0.11/setup.py` & `database-without-orm-local-0.0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
      name='database-without-orm-local',  
-     version='0.0.11', # https://pypi.org/project/database-without-orm-local/
+     version='0.0.12', # https://pypi.org/project/database-without-orm-local/
      author="Circles",
      author_email="info@circles.life",
      description="Circles Local Database without ORM Python PyPI Package",
      long_description="This is a package for sharing common Database methods",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

