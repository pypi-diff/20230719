# Comparing `tmp/importer-local-0.0.7.tar.gz` & `tmp/importer-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.7.tar", last modified: Tue Jul 18 08:43:19 2023, max compression
+gzip compressed data, was "importer-local-0.0.8.tar", last modified: Tue Jul 18 10:47:22 2023, max compression
```

## Comparing `importer-local-0.0.7.tar` & `importer-local-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/CirclesImporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:02.000000 importer-local-0.0.7/CirclesImporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-18 08:43:02.000000 importer-local-0.0.7/CirclesImporter/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 08:43:19.556270 importer-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 08:43:02.000000 importer-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:43:19.556270 importer-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-18 08:43:02.000000 importer-local-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-18 08:43:02.000000 importer-local-0.0.7/tests/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.389577 importer-local-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.385576 importer-local-0.0.8/CirclesImporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:05.000000 importer-local-0.0.8/CirclesImporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-18 10:47:05.000000 importer-local-0.0.8/CirclesImporter/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 10:47:22.389577 importer-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 10:47:05.000000 importer-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.385576 importer-local-0.0.8/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:47:22.389577 importer-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-18 10:47:05.000000 importer-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.385576 importer-local-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-18 10:47:05.000000 importer-local-0.0.8/tests/test_importer.py
```

### Comparing `importer-local-0.0.7/CirclesImporter/importer.py` & `importer-local-0.0.8/CirclesImporter/importer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from circles_local_database_python.database import database
 from CirclesGetCountryName.opencage_get_country_name import Country
 from dotenv import load_dotenv
-from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
+from LoggerLocalPythonPackage import LocalLogger
 from functools import wraps
 load_dotenv()
 
-
+Local_Logger=LocalLogger._Local_Logger
 def log_function_execution(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
-        start_message = "Function %s started." % func.__name__
-        _Local_Logger.start(start_message)
-
+        Local_Logger.start("Function %s started." % func.__name__)
         result = func(*args, **kwargs)  # Execute the function
-
-        finish_message = "Function %s completed." % func.__name__
-        _Local_Logger.end(finish_message)
+        Local_Logger.end("Function %s completed." % func.__name__)
         return result
     return wrapper
 
 
 class Importer:
     def __init__(self, source):
         self.source_name = source
 
     @log_function_execution
     def insert_new_entity(self, entity_type_name):
+        Local_Logger.start("Start Insert Entity %s ." % entity_type_name)
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT entity_type_id FROM {} WHERE entity_type_name = '{}'".format('entity_type.entity_type_ml_table', entity_type_name))
         entity_type_id = cursor.fetchone()
 
@@ -39,23 +36,23 @@
             cursor.execute(query_entity)
             db.commit()
 
             last_inserted_id = cursor.lastrowid
             query_entity_ml = "INSERT INTO {}(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, %s, 1, 1)".format('entity_type.entity_type_ml_table')
             cursor.execute(query_entity_ml, (entity_type_name, last_inserted_id, 'en'))
-
+            Local_Logger.end("End Inserted Entity %s ." % entity_type_name)
             db.commit()
         else:
-            source_message = "Entity %s already exist." % entity_type_name
-            _Local_Logger.end(source_message)
+            Local_Logger.end("Entity %s already exist." % entity_type_name)
         db.close()
 
     @log_function_execution
     def insert_new_source(self):
+        Local_Logger.start("Start insert_new_source()")
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT source_id FROM {} WHERE source_name = '{}'".format('source.source_ml_table', self.source_name))
         source_id = cursor.fetchone()
 
@@ -65,23 +62,23 @@
             cursor.execute(query_importer_source)
             db.commit()
 
             last_inserted_id = cursor.lastrowid
             query_importer_source_ml = "INSERT INTO {}(`source_name`,`source_id`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, 1, 1)".format('source.source_ml_table')
             cursor.execute(query_importer_source_ml, (self.source_name, last_inserted_id))
-
             db.commit()
+            Local_Logger.end("end insert_new_source %s."%self.source_name)
         else:
-            source_message = "Source %s already exist." % self.source_name
-            _Local_Logger.end(source_message)
+            Local_Logger.end("Source %s already exist." % self.source_name)
         db.close()
 
     @log_function_execution
     def insert_record_source(self, location, entity_type_name, entity_id, url):
+        Local_Logger.start("Function insert_record_source() started")
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT source_id FROM {} WHERE source_name = '{}'".format('source.source_ml_table', self.source_name))
         source_id = cursor.fetchone()
 
@@ -97,12 +94,13 @@
         query_importer = "INSERT INTO {}(`source_id`,`country_id`,`entity_type_id`,`entity_id`,`url`,`created_user_id`,`updated_user_id`)" \
                           " VALUES (%s, %s, %s, %s, %s, 1, 1)".format('importer.importer_table')
 
         cursor.execute(query_importer, (source_id[0], country_id[0], entity_type_id[0], entity_id, url))
 
         db.commit()
         db.close()
+        Local_Logger.end("Function insert_record_source() ended")
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `importer-local-0.0.7/README.md` & `importer-local-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `importer-local-0.0.7/setup.py` & `importer-local-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='importer-local',  
-     version='0.0.7',
+     version='0.0.8',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles <project-name> Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `importer-local-0.0.7/tests/test_importer.py` & `importer-local-0.0.8/tests/test_importer.py`

 * *Files identical despite different names*

