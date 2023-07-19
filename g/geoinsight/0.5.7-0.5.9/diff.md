# Comparing `tmp/geoinsight-0.5.7.tar.gz` & `tmp/geoinsight-0.5.9.tar.gz`

## Comparing `geoinsight-0.5.7.tar` & `geoinsight-0.5.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.7/geoinsight/src/__init__.py
--rw-r--r--   0        0        0    75327 2020-02-02 00:00:00.000000 geoinsight-0.5.7/geoinsight/src/api.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.7/geoinsight/src/geoinsight.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.7/geoinsight/src/util.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geoinsight-0.5.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.7/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.7/README.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 geoinsight-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.9/geoinsight/src/__init__.py
+-rw-r--r--   0        0        0    75512 2020-02-02 00:00:00.000000 geoinsight-0.5.9/geoinsight/src/api.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.9/geoinsight/src/geoinsight.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.9/geoinsight/src/util.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geoinsight-0.5.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.9/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.9/README.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 geoinsight-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.9/PKG-INFO
```

### Comparing `geoinsight-0.5.7/geoinsight/src/api.py` & `geoinsight-0.5.9/geoinsight/src/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,19 @@
         return requests.get(self.url + endpoint, headers=self.headers)
 
     def destination_source_overview(self):
         """API endpoint for destination_source_overview"""
         endpoint = '/destination_source_overview'
         return requests.get(self.url + endpoint, headers=self.headers)
 
+    def is_token_valid(self):
+        """API endpoint for is_token_valid"""
+        endpoint = '/is_token_valid'
+        return requests.get(self.url + endpoint, headers=self.headers)
+
     def isea3h_data_aoi(self):
         """API endpoint for isea3h_data_aoi"""
         endpoint = '/isea3h_data_aoi'
         return requests.get(self.url + endpoint, headers=self.headers)
 
     def isea3h_data_destination(self):
         """API endpoint for isea3h_data_destination"""
```

### Comparing `geoinsight-0.5.7/geoinsight/src/geoinsight.py` & `geoinsight-0.5.9/geoinsight/src/geoinsight.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.7/geoinsight/src/util.py` & `geoinsight-0.5.9/geoinsight/src/util.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.7/.gitignore` & `geoinsight-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.7/README.md` & `geoinsight-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.7/PKG-INFO` & `geoinsight-0.5.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoinsight
-Version: 0.5.7
+Version: 0.5.9
 Summary: GeoInsight Python Package
 Author-email: GeoInsight <info@geoinsight.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

