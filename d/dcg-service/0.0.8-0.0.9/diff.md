# Comparing `tmp/dcg_service-0.0.8.tar.gz` & `tmp/dcg_service-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcg_service-0.0.8.tar", last modified: Tue Jul 18 12:26:48 2023, max compression
+gzip compressed data, was "dcg_service-0.0.9.tar", last modified: Tue Jul 18 13:00:52 2023, max compression
```

## Comparing `dcg_service-0.0.8.tar` & `dcg_service-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 12:26:48.608943 dcg_service-0.0.8/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-0.0.8/LICENCE
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-18 12:26:48.608943 dcg_service-0.0.8/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-0.0.8/README.md
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      629 2023-07-18 12:26:30.000000 dcg_service-0.0.8/pyproject.toml
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      103 2023-07-17 06:04:33.000000 dcg_service-0.0.8/requirement.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-18 12:26:48.608943 dcg_service-0.0.8/setup.cfg
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 12:26:48.596943 dcg_service-0.0.8/src/
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 12:26:48.600943 dcg_service-0.0.8/src/dcg_service/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-0.0.8/src/dcg_service/__init__.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 12:26:48.608943 dcg_service-0.0.8/src/dcg_service/core/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-0.0.8/src/dcg_service/core/__init__.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2683 2023-07-18 12:26:17.000000 dcg_service-0.0.8/src/dcg_service/core/authentication.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      833 2023-07-17 13:54:47.000000 dcg_service-0.0.8/src/dcg_service/core/encryption.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7591 2023-07-17 13:56:57.000000 dcg_service-0.0.8/src/dcg_service/core/events.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2889 2023-07-13 06:38:05.000000 dcg_service-0.0.8/src/dcg_service/core/exceptions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-0.0.8/src/dcg_service/core/filters.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-0.0.8/src/dcg_service/core/logger.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2800 2023-07-17 14:13:54.000000 dcg_service-0.0.8/src/dcg_service/core/permissions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     3038 2023-07-18 12:25:40.000000 dcg_service-0.0.8/src/dcg_service/core/request_client.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-0.0.8/src/dcg_service/core/response.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16189 2023-07-12 05:41:48.000000 dcg_service-0.0.8/src/dcg_service/core/services.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1077 2023-07-17 14:04:57.000000 dcg_service-0.0.8/src/dcg_service/core/utils.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 12:26:48.600943 dcg_service-0.0.8/src/dcg_service.egg-info/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-18 12:26:48.000000 dcg_service-0.0.8/src/dcg_service.egg-info/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      677 2023-07-18 12:26:48.000000 dcg_service-0.0.8/src/dcg_service.egg-info/SOURCES.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-18 12:26:48.000000 dcg_service-0.0.8/src/dcg_service.egg-info/dependency_links.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      104 2023-07-18 12:26:48.000000 dcg_service-0.0.8/src/dcg_service.egg-info/requires.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-18 12:26:48.000000 dcg_service-0.0.8/src/dcg_service.egg-info/top_level.txt
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.512735 dcg_service-0.0.9/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-0.0.9/LICENCE
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-18 13:00:52.500735 dcg_service-0.0.9/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-0.0.9/README.md
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      629 2023-07-18 12:55:13.000000 dcg_service-0.0.9/pyproject.toml
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      103 2023-07-17 06:04:33.000000 dcg_service-0.0.9/requirement.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-18 13:00:52.512735 dcg_service-0.0.9/setup.cfg
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.480736 dcg_service-0.0.9/src/
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.484736 dcg_service-0.0.9/src/dcg_service/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-0.0.9/src/dcg_service/__init__.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.500735 dcg_service-0.0.9/src/dcg_service/core/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-0.0.9/src/dcg_service/core/__init__.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2683 2023-07-18 12:26:17.000000 dcg_service-0.0.9/src/dcg_service/core/authentication.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      833 2023-07-17 13:54:47.000000 dcg_service-0.0.9/src/dcg_service/core/encryption.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7591 2023-07-17 13:56:57.000000 dcg_service-0.0.9/src/dcg_service/core/events.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2889 2023-07-13 06:38:05.000000 dcg_service-0.0.9/src/dcg_service/core/exceptions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-0.0.9/src/dcg_service/core/filters.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-0.0.9/src/dcg_service/core/logger.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2691 2023-07-18 12:54:48.000000 dcg_service-0.0.9/src/dcg_service/core/permissions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     3038 2023-07-18 12:25:40.000000 dcg_service-0.0.9/src/dcg_service/core/request_client.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-0.0.9/src/dcg_service/core/response.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16189 2023-07-12 05:41:48.000000 dcg_service-0.0.9/src/dcg_service/core/services.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1077 2023-07-17 14:04:57.000000 dcg_service-0.0.9/src/dcg_service/core/utils.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.488736 dcg_service-0.0.9/src/dcg_service.egg-info/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      677 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      104 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/requires.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/top_level.txt
```

### Comparing `dcg_service-0.0.8/LICENCE` & `dcg_service-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/PKG-INFO` & `dcg_service-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcg_service
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for DCG DOT Compliance Group, used for flask based projects.
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcg_service-0.0.8/README.md` & `dcg_service-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/pyproject.toml` & `dcg_service-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dcg_service"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Aman Kumar", email="amankumar@zapbuild.com" },
 ]
 description = "Package for DCG DOT Compliance Group, used for flask based projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcg_service-0.0.8/src/dcg_service/core/authentication.py` & `dcg_service-0.0.9/src/dcg_service/core/authentication.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/encryption.py` & `dcg_service-0.0.9/src/dcg_service/core/encryption.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/events.py` & `dcg_service-0.0.9/src/dcg_service/core/events.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/exceptions.py` & `dcg_service-0.0.9/src/dcg_service/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/filters.py` & `dcg_service-0.0.9/src/dcg_service/core/filters.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/logger.py` & `dcg_service-0.0.9/src/dcg_service/core/logger.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/permissions.py` & `dcg_service-0.0.9/src/dcg_service/core/permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,25 +68,19 @@
 def authenticated_request(allow_internal_request=False):
     """
     Decorator function to authorize the API request,
     this decorator authorize internal request and token request.
     """
 
     def internal_request_deco(func):
-        try:
-            headers = getattr(request, 'headers', {})
-        except:
-            headers = dict()
-
-        request_internal_key = get_internal_key_header(headers)
-
-        if allow_internal_request and request_internal_key:
+        if allow_internal_request:
             @wraps(func)
             def wrapper(*args, **kwargs):
-                if request_internal_key == INTERNAL_SERVICE_KEY:
+                request_internal_key = get_internal_key_header(request.headers)
+                if request_internal_key == os.environ['INTERNAL_SERVICE_KEY']:
                     setattr(request, 'is_internal_request', True)
                 else:
                     return is_authenticated(func)
                 return func(*args, **kwargs)
             return wrapper
         else:
             return is_authenticated(func)
```

### Comparing `dcg_service-0.0.8/src/dcg_service/core/request_client.py` & `dcg_service-0.0.9/src/dcg_service/core/request_client.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/response.py` & `dcg_service-0.0.9/src/dcg_service/core/response.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/services.py` & `dcg_service-0.0.9/src/dcg_service/core/services.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service/core/utils.py` & `dcg_service-0.0.9/src/dcg_service/core/utils.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.8/src/dcg_service.egg-info/PKG-INFO` & `dcg_service-0.0.9/src/dcg_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcg-service
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for DCG DOT Compliance Group, used for flask based projects.
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcg_service-0.0.8/src/dcg_service.egg-info/SOURCES.txt` & `dcg_service-0.0.9/src/dcg_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

