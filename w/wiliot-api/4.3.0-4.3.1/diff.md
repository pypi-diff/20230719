# Comparing `tmp/wiliot-api-4.3.0.tar.gz` & `tmp/wiliot-api-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.3.0.tar", last modified: Mon Jun 26 23:48:12 2023, max compression
+gzip compressed data, was "wiliot-api-4.3.1.tar", last modified: Wed Jul 19 09:11:35 2023, max compression
```

## Comparing `wiliot-api-4.3.0.tar` & `wiliot-api-4.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3990 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7512 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11151 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15211 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14099 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35975 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3990 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4075 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3569 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9514 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.307638 wiliot-api-4.3.1/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11151 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15211 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    14099 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35975 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7223 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.311637 wiliot-api-4.3.1/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2023-07-19 09:11:18.000000 wiliot-api-4.3.1/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 09:11:35.307638 wiliot-api-4.3.1/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4075 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-07-19 09:11:35.000000 wiliot-api-4.3.1/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.3.0/LICENSE` & `wiliot-api-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/PKG-INFO` & `wiliot-api-4.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.3.0
+Version: 4.3.1
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,17 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.3.1:
+-----------------
+* Added a function for sending actions to a gateway
 
 Version 4.3.0:
 -----------------
 * Change code to match the changes in asset label API endpoint
 * All 2xx status code returned by the API are considered a success
 
 Version 4.2.0:
```

### Comparing `wiliot-api-4.3.0/README.md` & `wiliot-api-4.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.3.1:
+-----------------
+* Added a function for sending actions to a gateway
 
 Version 4.3.0:
 -----------------
 * Change code to match the changes in asset label API endpoint
 * All 2xx status code returned by the API are considered a success
 
 Version 4.2.0:
```

### Comparing `wiliot-api-4.3.0/setup.py` & `wiliot-api-4.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/__init__.py` & `wiliot-api-4.3.1/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/api_client.py` & `wiliot-api-4.3.1/wiliot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/edge/edge.py` & `wiliot-api-4.3.1/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.3.1/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.3.1/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.3.1/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.3.1/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/platform/platform.py` & `wiliot-api-4.3.1/wiliot_api/platform/platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/platform/platform_models.py` & `wiliot-api-4.3.1/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/security/security.py` & `wiliot-api-4.3.1/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api/utils/get_version.py` & `wiliot-api-4.3.1/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.0/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.3.1/wiliot_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.3.0
+Version: 4.3.1
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,17 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.3.1:
+-----------------
+* Added a function for sending actions to a gateway
 
 Version 4.3.0:
 -----------------
 * Change code to match the changes in asset label API endpoint
 * All 2xx status code returned by the API are considered a success
 
 Version 4.2.0:
```

### Comparing `wiliot-api-4.3.0/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.3.1/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

