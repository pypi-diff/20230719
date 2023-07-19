# Comparing `tmp/ecallisto_ng-0.2.2.tar.gz` & `tmp/ecallisto_ng-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.2.tar", last modified: Tue Jul 18 19:06:52 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.3.tar", last modified: Tue Jul 18 20:20:10 2023, max compression
```

## Comparing `ecallisto_ng-0.2.2.tar` & `ecallisto_ng-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.2/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.2/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-18 19:06:25.000000 ecallisto_ng-0.2.2/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7758 2023-07-18 19:05:40.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2844 2023-07-18 19:00:07.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.3/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.3/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-18 20:19:56.000000 ecallisto_ng-0.2.3/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.101095 ecallisto_ng-0.2.3/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7760 2023-07-18 20:19:47.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2844 2023-07-18 19:00:07.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.2/LICENSE` & `ecallisto_ng-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.2/PKG-INFO` & `ecallisto_ng-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.2/README.md` & `ecallisto_ng-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.2/pyproject.toml` & `ecallisto_ng-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.2"
+version = "0.2.3"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 # Check the status of the json 
                 if 'status' in json_response.json():
                     if json_response.json()['status'] == 'processing':
                         # If the file is not found, sleep for a short period and try again
                         if verbose:
                             print(f"File {file_id} not ready yet, waiting...")
                         time.sleep(5)
-                    elif json_response.json['status'] == 'ok':
+                    elif json_response.json()['status'] == 'ok':
                         if verbose:
                             print(f'File {file_id} succesfully written! Will return file')
                     else:
                         raise ValueError(f"Error downloading file: {json_response.json()['status']}")
                 elif 'error' in json_response.json():
                     raise ValueError(f"Error downloading file: {json_response.json()['error']}")
             else:
```

### Comparing `ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

