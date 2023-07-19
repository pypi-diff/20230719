# Comparing `tmp/idbadapter-1.9.tar.gz` & `tmp/idbadapter-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.tar", last modified: Thu Jul 13 10:57:44 2023, max compression
+gzip compressed data, was "idbadapter-1.9.1.tar", last modified: Wed Jul 19 12:49:53 2023, max compression
```

## Comparing `idbadapter-1.9.tar` & `idbadapter-1.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 10:57:44.647962 idbadapter-1.9/
--rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.9/LICENSE
--rw-rw-rw-   0        0        0      695 2023-07-13 10:57:44.648967 idbadapter-1.9/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 10:57:44.617864 idbadapter-1.9/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.9/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    12028 2023-07-13 10:56:58.000000 idbadapter-1.9/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:57:44.646959 idbadapter-1.9/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 10:57:44.651978 idbadapter-1.9/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-07-13 10:57:42.000000 idbadapter-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:49:53.165595 idbadapter-1.9.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.1/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-07-19 12:49:53.165595 idbadapter-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 12:49:53.148597 idbadapter-1.9.1/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.1/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    11816 2023-07-19 12:47:26.000000 idbadapter-1.9.1/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:49:53.163596 idbadapter-1.9.1/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:49:53.166595 idbadapter-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-19 12:49:49.000000 idbadapter-1.9.1/setup.py
```

### Comparing `idbadapter-1.9/LICENSE` & `idbadapter-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9/PKG-INFO` & `idbadapter-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9
+Version: 1.9.1
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9/idbadapter/schedule_loader.py` & `idbadapter-1.9.1/idbadapter/schedule_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pandas as pd
 import requests
 import json
 from urllib.parse import urljoin
 
-GRANULARY = {"column": "granulary_name", "table": "granulary_works", "id": "id_granulary_work"}
+GRANULARY = {"column": "granulary_name", "table": "granulary_works", "id": "id_granulary_work", "res_table": "granulary_resources"}
 
-PROCESSED = {"column": "processed_name", "table": "processed_works", "id": "id_processed_work"}
+PROCESSED = {"column": "processed_name", "table": "processed_works", "id": "id_processed_work", "res_table": "processed_resourcesobje"}
 
-TYPEDLVL2 = {"column": "typed_lvl2_name", "table": "typed_lvl2_works", "id": "id_typed_lvl2_work"}
+TYPEDLVL2 = {"column": "typed_lvl2_name", "table": "typed_lvl2_works", "id": "id_typed_lvl2_work", "res_table": "typed_lvl2_resources"}
 
 ALL = "all"
 
 
 class Schedules:
     """Get schedules from database service
     """
@@ -75,25 +75,19 @@
             self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_names(key)})
             
         if len(self.objects) == 0:
             raise Exception("Objects not found")
         
         return self
            
-    def get_resources_names(self, res_type="granulary"):
-        queries = {
-            "granulary": "SELECT DISTINCT name FROM basic_resources",
-        }
-        if res_type not in queries:
-            raise ValueError(f"Incorrect work_type argument. {res_type}")
-        
-        data = json.dumps({"body": queries[res_type]})        
-        response = self.session.post(urljoin(self.url, "query/select"), data=data)
-        
-        return response.json()
+    def get_resources_names(self, res_type=GRANULARY):
+        query = f"SELECT DISTINCT name FROM {res_type['res_table']}"
+        print(query)
+        df = self._execute_query(query)
+        return df
         
     def get_works_names(self, work_type=GRANULARY):
         query = f"SELECT DISTINCT name FROM {work_type['table']}"
         df = self._execute_query(query)
         return df
     
     def _get_works_ids_by_names(self, work_name_list):
@@ -193,22 +187,20 @@
                 
             if len(resource_list) != 0:
                 query += f""" and rnm.name in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
             try:
                 df = self._execute_query(query)
             except ValueError:
                 print("jsondecodeerror occurred", pull)
-                yield None
                 continue 
 
             if df.empty:
                 with open(self.path_to_log, "a", encoding="UTF-8") as f:
                     print("pull not found", pull, file=f)
                     print("empty df. pull not found")
-                    yield None
                 continue
                 
             df["full_fraction"] = df["physical_volume"]
                       
                 
             yield SchedulesIterator.convert_df(df)
```

### Comparing `idbadapter-1.9/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.1/idbadapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9
+Version: 1.9.1
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9/setup.py` & `idbadapter-1.9.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9'
+version = '1.9.1'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9',
+      version='1.9.1',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

