# Comparing `tmp/minddatapack-0.9.1.tar.gz` & `tmp/minddatapack-0.9.2.tar.gz`

## Comparing `minddatapack-0.9.1.tar` & `minddatapack-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 minddatapack-0.9.1/minddatapack/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 minddatapack-0.9.1/minddatapack/arweaveconnector.py
--rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 minddatapack-0.9.1/minddatapack/localfileconnector.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 minddatapack-0.9.1/minddatapack/mindlakeconnector.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 minddatapack-0.9.1/minddatapack/utils.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 minddatapack-0.9.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 minddatapack-0.9.1/LICENSE
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 minddatapack-0.9.1/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 minddatapack-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 minddatapack-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 minddatapack-0.9.2/minddatapack/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 minddatapack-0.9.2/minddatapack/arweaveconnector.py
+-rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 minddatapack-0.9.2/minddatapack/localfileconnector.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 minddatapack-0.9.2/minddatapack/mindlakeconnector.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 minddatapack-0.9.2/minddatapack/utils.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 minddatapack-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 minddatapack-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 minddatapack-0.9.2/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 minddatapack-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 minddatapack-0.9.2/PKG-INFO
```

### Comparing `minddatapack-0.9.1/minddatapack/__init__.py` & `minddatapack-0.9.2/minddatapack/__init__.py`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/minddatapack/arweaveconnector.py` & `minddatapack-0.9.2/minddatapack/arweaveconnector.py`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/minddatapack/localfileconnector.py` & `minddatapack-0.9.2/minddatapack/localfileconnector.py`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/minddatapack/mindlakeconnector.py` & `minddatapack-0.9.2/minddatapack/mindlakeconnector.py`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/minddatapack/utils.py` & `minddatapack-0.9.2/minddatapack/utils.py`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/.gitignore` & `minddatapack-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/LICENSE` & `minddatapack-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/README.md` & `minddatapack-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `minddatapack-0.9.1/pyproject.toml` & `minddatapack-0.9.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "minddatapack"
-version = "v0.9.1"
+version = "v0.9.2"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to migrate data between Mind Lake and other storages"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["web3", "encryption", "datalake"]
 dependencies = [
     "mindlakesdk",
-    "arseeding",
-    "web3 < 6.0.0"
+    "arseeding"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mind-network/mind-lake-sdk-python"
 "Bug Tracker" = "https://github.com/mind-network/mind-lake-sdk-python/issues"
 
 [tool.hatch.build]
```

### Comparing `minddatapack-0.9.1/PKG-INFO` & `minddatapack-0.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: minddatapack
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python SDK to migrate data between Mind Lake and other storages
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: arseeding
 Requires-Dist: mindlakesdk
-Requires-Dist: web3<6.0.0
 Description-Content-Type: text/markdown
 
 # Mind DataPack Python SDK
 
 An Python implementation for Mind DataPack
 
 ## Description
```

