# Comparing `tmp/trustedtwin-3.3.20230717090114.tar.gz` & `tmp/trustedtwin-3.3.20230718090121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustedtwin-3.3.20230717090114.tar", last modified: Mon Jul 17 09:01:30 2023, max compression
+gzip compressed data, was "trustedtwin-3.3.20230718090121.tar", last modified: Tue Jul 18 09:01:37 2023, max compression
```

## Comparing `trustedtwin-3.3.20230717090114.tar` & `trustedtwin-3.3.20230718090121.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 09:01:30.456393 trustedtwin-3.3.20230717090114/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/LICENSE
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-17 09:01:30.456393 trustedtwin-3.3.20230717090114/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-17 09:01:30.457393 trustedtwin-3.3.20230717090114/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 09:01:30.455393 trustedtwin-3.3.20230717090114/trustedtwin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/trustedtwin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2340 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/trustedtwin/tt_api.py
--rw-r--r--   0 root         (0) root         (0)   105771 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin/tt_api.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/trustedtwin/tt_api_async.py
--rw-r--r--   0 root         (0) root         (0)   126701 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin/tt_api_async.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-17 09:01:10.000000 trustedtwin-3.3.20230717090114/trustedtwin/tt_api_base.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-07-17 09:01:29.000000 trustedtwin-3.3.20230717090114/trustedtwin/tt_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 09:01:30.456393 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 09:01:30.000000 trustedtwin-3.3.20230717090114/trustedtwin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:37.891753 trustedtwin-3.3.20230718090121/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-18 09:01:37.891753 trustedtwin-3.3.20230718090121/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-18 09:01:37.891753 trustedtwin-3.3.20230718090121/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:37.889753 trustedtwin-3.3.20230718090121/trustedtwin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/trustedtwin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/trustedtwin/tt_api.py
+-rw-r--r--   0 root         (0) root         (0)   105771 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin/tt_api.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/trustedtwin/tt_api_async.py
+-rw-r--r--   0 root         (0) root         (0)   126701 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin/tt_api_async.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-18 09:01:17.000000 trustedtwin-3.3.20230718090121/trustedtwin/tt_api_base.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin/tt_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:37.891753 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 09:01:37.000000 trustedtwin-3.3.20230718090121/trustedtwin.egg-info/top_level.txt
```

### Comparing `trustedtwin-3.3.20230717090114/LICENSE` & `trustedtwin-3.3.20230718090121/LICENSE`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/PKG-INFO` & `trustedtwin-3.3.20230718090121/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 3.3.20230717090114
+Version: 3.3.20230718090121
 Summary: Trusted Twin Python client
 Home-page: https://gitlab.com/trustedtwin/trustedtwin-python
 Author: TrustedTwin
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
```

### Comparing `trustedtwin-3.3.20230717090114/README.md` & `trustedtwin-3.3.20230718090121/README.md`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/setup.py` & `trustedtwin-3.3.20230718090121/setup.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin/tt_api.py` & `trustedtwin-3.3.20230718090121/trustedtwin/tt_api.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin/tt_api.pyi` & `trustedtwin-3.3.20230718090121/trustedtwin/tt_api.pyi`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin/tt_api_async.py` & `trustedtwin-3.3.20230718090121/trustedtwin/tt_api_async.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin/tt_api_async.pyi` & `trustedtwin-3.3.20230718090121/trustedtwin/tt_api_async.pyi`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin/tt_api_base.py` & `trustedtwin-3.3.20230718090121/trustedtwin/tt_api_base.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin/tt_endpoints.py` & `trustedtwin-3.3.20230718090121/trustedtwin/tt_endpoints.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20230717090114/trustedtwin.egg-info/PKG-INFO` & `trustedtwin-3.3.20230718090121/trustedtwin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 3.3.20230717090114
+Version: 3.3.20230718090121
 Summary: Trusted Twin Python client
 Home-page: https://gitlab.com/trustedtwin/trustedtwin-python
 Author: TrustedTwin
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
```

