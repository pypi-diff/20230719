# Comparing `tmp/omigo_core-0.5.3.tar.gz` & `tmp/omigo_core-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_core-0.5.3.tar", last modified: Tue Jul 18 22:40:12 2023, max compression
+gzip compressed data, was "omigo_core-0.5.4.tar", last modified: Tue Jul 18 23:32:53 2023, max compression
```

## Comparing `omigo_core-0.5.3.tar` & `omigo_core-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 22:40:12.535642 omigo_core-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_core-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 22:39:56.000000 omigo_core-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 22:40:12.535642 omigo_core-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.531643 omigo_core-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/src/omigo_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_paths_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_paths_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_paths_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/funclib.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/local_fs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/s3_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/s3io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)   214991 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/tsvutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/src/omigo_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 22:39:56.000000 omigo_core-0.5.3/test/test_tsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:53.006817 omigo_core-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 23:32:53.006817 omigo_core-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:36.000000 omigo_core-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 23:32:36.000000 omigo_core-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 23:32:53.006817 omigo_core-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:52.998817 omigo_core-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:53.002817 omigo_core-0.5.4/src/omigo_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/file_io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/file_paths_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/file_paths_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/file_paths_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/funclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/local_fs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/s3_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/s3io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214991 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/tsvutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-07-18 23:32:36.000000 omigo_core-0.5.4/src/omigo_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:53.006817 omigo_core-0.5.4/src/omigo_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 23:32:52.000000 omigo_core-0.5.4/src/omigo_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-18 23:32:52.000000 omigo_core-0.5.4/src/omigo_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:32:52.000000 omigo_core-0.5.4/src/omigo_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 23:32:52.000000 omigo_core-0.5.4/src/omigo_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 23:32:52.000000 omigo_core-0.5.4/src/omigo_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:53.006817 omigo_core-0.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 23:32:36.000000 omigo_core-0.5.4/test/test_tsv.py
```

### Comparing `omigo_core-0.5.3/PKG-INFO` & `omigo_core-0.5.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_core
-Version: 0.5.3
+Version: 0.5.4
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.3/setup.cfg` & `omigo_core-0.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_core
-version = 0.5.3
+version = 0.5.4
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_core-0.5.3/src/omigo_core/etl.py` & `omigo_core-0.5.4/src/omigo_core/etl.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/file_io_wrapper.py` & `omigo_core-0.5.4/src/omigo_core/file_io_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/file_paths_data_reader.py` & `omigo_core-0.5.4/src/omigo_core/file_paths_data_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/file_paths_reader.py` & `omigo_core-0.5.4/src/omigo_core/file_paths_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/file_paths_util.py` & `omigo_core-0.5.4/src/omigo_core/file_paths_util.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/funclib.py` & `omigo_core-0.5.4/src/omigo_core/funclib.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/graph_traversal.py` & `omigo_core-0.5.4/src/omigo_core/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/local_fs_wrapper.py` & `omigo_core-0.5.4/src/omigo_core/local_fs_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/s3_wrapper.py` & `omigo_core-0.5.4/src/omigo_core/s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/s3io_wrapper.py` & `omigo_core-0.5.4/src/omigo_core/s3io_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/tsv.py` & `omigo_core-0.5.4/src/omigo_core/tsv.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/tsvutils.py` & `omigo_core-0.5.4/src/omigo_core/tsvutils.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core/utils.py` & `omigo_core-0.5.4/src/omigo_core/utils.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.3/src/omigo_core.egg-info/PKG-INFO` & `omigo_core-0.5.4/src/omigo_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo-core
-Version: 0.5.3
+Version: 0.5.4
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.3/src/omigo_core.egg-info/SOURCES.txt` & `omigo_core-0.5.4/src/omigo_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

