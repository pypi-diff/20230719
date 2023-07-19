# Comparing `tmp/gdata-vaas-3.2.0.tar.gz` & `tmp/gdata-vaas-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-3.2.0.tar", last modified: Thu Jul  6 12:40:32 2023, max compression
+gzip compressed data, was "gdata-vaas-3.2.1.tar", last modified: Wed Jul 19 08:02:53 2023, max compression
```

## Comparing `gdata-vaas-3.2.0.tar` & `gdata-vaas-3.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.003340 gdata-vaas-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.007341 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-06 12:40:32.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11337 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.753228 gdata-vaas-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.753228 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.753228 gdata-vaas-3.2.1/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11337 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/tests/test_vaas.py
```

### Comparing `gdata-vaas-3.2.0/LICENSE` & `gdata-vaas-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.0/PKG-INFO` & `gdata-vaas-3.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.2.0
+Version: 3.2.1
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.2.0/README.md` & `gdata-vaas-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.0/setup.cfg` & `gdata-vaas-3.2.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 3.2.0
+version = 3.2.1
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls = 
@@ -14,17 +14,17 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	websockets ==10.4
-	httpx[http2] ==0.23.3
+	httpx[http2] ==0.24.1
 	jwt == 1.3.1
-	authlib ==1.2.0
+	authlib ==1.2.1
 	aiofiles==23.1.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `gdata-vaas-3.2.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata-vaas-3.2.1/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.2.0
+Version: 3.2.1
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.2.0/src/vaas/__init__.py` & `gdata-vaas-3.2.1/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata-vaas-3.2.1/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.0/src/vaas/vaas.py` & `gdata-vaas-3.2.1/src/vaas/vaas.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.0/tests/test_client_credentials_grant_authenticator.py` & `gdata-vaas-3.2.1/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.0/tests/test_vaas.py` & `gdata-vaas-3.2.1/tests/test_vaas.py`

 * *Files identical despite different names*

