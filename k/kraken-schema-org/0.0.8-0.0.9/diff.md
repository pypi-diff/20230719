# Comparing `tmp/kraken-schema-org-0.0.8.tar.gz` & `tmp/kraken-schema-org-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken-schema-org-0.0.8.tar", last modified: Sun Dec 19 16:56:08 2021, max compression
+gzip compressed data, was "kraken-schema-org-0.0.9.tar", last modified: Mon Apr  4 12:46:20 2022, max compression
```

## Comparing `kraken-schema-org-0.0.8.tar` & `kraken-schema-org-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 16:56:08.490205 kraken-schema-org-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-12-19 16:56:08.490205 kraken-schema-org-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 16:56:08.490205 kraken-schema-org-0.0.8/kraken_schema_org/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/kraken_schema_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5921 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/kraken_schema_org/class_kraken_schema_org.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/kraken_schema_org/kraken_schema_org.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/kraken_schema_org/schema_org_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/kraken_schema_org/schema_org_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 16:56:08.490205 kraken-schema-org-0.0.8/kraken_schema_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-12-19 16:56:08.000000 kraken-schema-org-0.0.8/kraken_schema_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-12-19 16:56:08.000000 kraken-schema-org-0.0.8/kraken_schema_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-19 16:56:08.000000 kraken-schema-org-0.0.8/kraken_schema_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-12-19 16:56:08.000000 kraken-schema-org-0.0.8/kraken_schema_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-19 16:56:08.000000 kraken-schema-org-0.0.8/kraken_schema_org.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-19 16:56:08.490205 kraken-schema-org-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-12-19 16:55:58.000000 kraken-schema-org-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 12:46:20.631490 kraken-schema-org-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-04-04 12:46:20.631490 kraken-schema-org-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 12:46:20.631490 kraken-schema-org-0.0.9/kraken_schema_org/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6269 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/class_kraken_schema_org.py
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/kraken_schema_org.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/schema_org_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/schema_org_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/schema_org_normalize_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/kraken_schema_org/schema_org_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 12:46:20.631490 kraken-schema-org-0.0.9/kraken_schema_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-04-04 12:46:20.000000 kraken-schema-org-0.0.9/kraken_schema_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-04-04 12:46:20.000000 kraken-schema-org-0.0.9/kraken_schema_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 12:46:20.000000 kraken-schema-org-0.0.9/kraken_schema_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-04-04 12:46:20.000000 kraken-schema-org-0.0.9/kraken_schema_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-04 12:46:20.000000 kraken-schema-org-0.0.9/kraken_schema_org.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-04 12:46:20.631490 kraken-schema-org-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2022-04-04 12:46:03.000000 kraken-schema-org-0.0.9/setup.py
```

### Comparing `kraken-schema-org-0.0.8/PKG-INFO` & `kraken-schema-org-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-schema-org
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kraken schema.org
 Home-page: https://github.com/tactik8/kraken_datatype2
 Author: Tactik8
 Author-email: info@tactik8.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -16,25 +16,33 @@
 
 
 How to use:
 
 from kraken_schema_org import kraken_schema_org as k
 
 normalize_type:
+```
 record_type = 'person'
 normalized_type = k.normalize_type(record_type)
+```
 
 normalize_key:
+```
 key = 'givenname'
 normalized_key = k.normalize_key(key)
+```
 
 get_keys:
+```
 record_type = 'person'
 keys = k.get_keys(record_type)
+```
 
 get_datatype():
+```
 record_type = 'schema:Person'
 key = 'schema:givenName'
 datatypes = k.get_datatype(record_type, key)
+```
```

### Comparing `kraken-schema-org-0.0.8/kraken_schema_org/class_kraken_schema_org.py` & `kraken-schema-org-0.0.9/kraken_schema_org/class_kraken_schema_org.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import requests
 import json
 from kraken_schema_org import schema_org_data  
 from kraken_schema_org import schema_org_transform 
+from kraken_schema_org import schema_org_get_id 
+from kraken_schema_org import schema_org_normalize_record
 
 
 """
 Method to clean data following schema.org format
 """
 
 
@@ -83,14 +85,23 @@
     
     def get_datatype(self, record_type, key):
         """Given a key, returns the datatype (text, number, entity, etc)
         """
         return self._get_data_type(record_type, key)
 
 
+
+    def get_record_id(self, record):
+        return schema_org_get_id.get(record)
+        
+
+    def normalize_record(self, record, strict = False):
+        record = schema_org_normalize_record.get(record, strict)
+        return record
+    
     """
     Methods - Main
     """
 
     def _get_clean_record_type(self, record_type):
         """Returns the clean type of the schema
         """
```

### Comparing `kraken-schema-org-0.0.8/kraken_schema_org/schema_org_data.py` & `kraken-schema-org-0.0.9/kraken_schema_org/schema_org_data.py`

 * *Files identical despite different names*

### Comparing `kraken-schema-org-0.0.8/kraken_schema_org/schema_org_transform.py` & `kraken-schema-org-0.0.9/kraken_schema_org/schema_org_transform.py`

 * *Files identical despite different names*

### Comparing `kraken-schema-org-0.0.8/kraken_schema_org.egg-info/PKG-INFO` & `kraken-schema-org-0.0.9/kraken_schema_org.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-schema-org
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kraken schema.org
 Home-page: https://github.com/tactik8/kraken_datatype2
 Author: Tactik8
 Author-email: info@tactik8.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -16,25 +16,33 @@
 
 
 How to use:
 
 from kraken_schema_org import kraken_schema_org as k
 
 normalize_type:
+```
 record_type = 'person'
 normalized_type = k.normalize_type(record_type)
+```
 
 normalize_key:
+```
 key = 'givenname'
 normalized_key = k.normalize_key(key)
+```
 
 get_keys:
+```
 record_type = 'person'
 keys = k.get_keys(record_type)
+```
 
 get_datatype():
+```
 record_type = 'schema:Person'
 key = 'schema:givenName'
 datatypes = k.get_datatype(record_type, key)
+```
```

### Comparing `kraken-schema-org-0.0.8/setup.py` & `kraken-schema-org-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="kraken-schema-org",
-    version="0.0.8",
+    version="0.0.9",
     description="Kraken schema.org",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/tactik8/kraken_datatype2",
     author="Tactik8",
     author_email="info@tactik8.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=["kraken_schema_org"],
     include_package_data=True,
-    install_requires=['url-normalize', 'validators', 'dateparser', 'pycountry', 'email-normalize', 'cleanco', 'phonenumbers'],
+    install_requires=['url-normalize', 'validators', 'dateparser', 'pycountry', 'email-normalize', 'cleanco', 'phonenumbers', 'kraken-datatype'],
     
 )
```

