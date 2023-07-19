# Comparing `tmp/iorclient-0.0.1.tar.gz` & `tmp/iorclient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iorclient-0.0.1.tar", last modified: Tue Jul 18 17:53:22 2023, max compression
+gzip compressed data, was "iorclient-0.0.2.tar", last modified: Tue Jul 18 18:09:12 2023, max compression
```

## Comparing `iorclient-0.0.1.tar` & `iorclient-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:53:22.101567 iorclient-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      965 2023-07-18 17:53:22.100574 iorclient-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 17:53:22.073664 iorclient-0.0.1/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-0.0.1/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:53:22.081633 iorclient-0.0.1/ior/client/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-0.0.1/ior/client/__init__.py
--rw-rw-rw-   0        0        0    10753 2023-07-18 17:46:25.000000 iorclient-0.0.1/ior/client/certificate_service.py
--rw-rw-rw-   0        0        0     4396 2023-07-18 16:29:10.000000 iorclient-0.0.1/ior/client/contract_template_service.py
--rw-rw-rw-   0        0        0     4553 2023-07-18 17:25:05.000000 iorclient-0.0.1/ior/client/permission_control_service.py
--rw-rw-rw-   0        0        0     5260 2023-07-18 17:29:42.000000 iorclient-0.0.1/ior/client/role_control_service.py
--rw-rw-rw-   0        0        0     4920 2023-07-18 17:05:02.000000 iorclient-0.0.1/ior/client/template_control_service.py
--rw-rw-rw-   0        0        0     2287 2023-07-18 16:30:34.000000 iorclient-0.0.1/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:53:22.086618 iorclient-0.0.1/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-0.0.1/ior/util/__init__.py
--rw-rw-rw-   0        0        0     1603 2023-07-17 15:27:53.000000 iorclient-0.0.1/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-0.0.1/ior/util/web3_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:53:22.092597 iorclient-0.0.1/iorclient.egg-info/
--rw-rw-rw-   0        0        0      965 2023-07-18 17:53:21.000000 iorclient-0.0.1/iorclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-07-18 17:53:21.000000 iorclient-0.0.1/iorclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:53:21.000000 iorclient-0.0.1/iorclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 17:53:21.000000 iorclient-0.0.1/iorclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:53:22.102569 iorclient-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-18 17:51:31.000000 iorclient-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:53:22.097580 iorclient-0.0.1/test/
--rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0      873 2023-07-18 16:43:49.000000 iorclient-0.0.1/test/test_cert.py
--rw-rw-rw-   0        0        0        0 2023-07-18 16:25:02.000000 iorclient-0.0.1/test/test_role.py
--rw-rw-rw-   0        0        0        0 2023-07-18 16:25:05.000000 iorclient-0.0.1/test/test_template.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:12.394496 iorclient-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      965 2023-07-18 18:09:12.394496 iorclient-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:12.368537 iorclient-0.0.2/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-0.0.2/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:12.376519 iorclient-0.0.2/ior/client/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-0.0.2/ior/client/__init__.py
+-rw-rw-rw-   0        0        0    10753 2023-07-18 17:46:25.000000 iorclient-0.0.2/ior/client/certificate_service.py
+-rw-rw-rw-   0        0        0     4396 2023-07-18 16:29:10.000000 iorclient-0.0.2/ior/client/contract_template_service.py
+-rw-rw-rw-   0        0        0     2117 2023-07-18 18:05:19.000000 iorclient-0.0.2/ior/client/exchange_service.py
+-rw-rw-rw-   0        0        0     4553 2023-07-18 17:25:05.000000 iorclient-0.0.2/ior/client/permission_control_service.py
+-rw-rw-rw-   0        0        0     5260 2023-07-18 17:29:42.000000 iorclient-0.0.2/ior/client/role_control_service.py
+-rw-rw-rw-   0        0        0     4920 2023-07-18 17:05:02.000000 iorclient-0.0.2/ior/client/template_control_service.py
+-rw-rw-rw-   0        0        0     2287 2023-07-18 16:30:34.000000 iorclient-0.0.2/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:12.381507 iorclient-0.0.2/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-0.0.2/ior/util/__init__.py
+-rw-rw-rw-   0        0        0     1603 2023-07-17 15:27:53.000000 iorclient-0.0.2/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-0.0.2/ior/util/web3_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:12.386492 iorclient-0.0.2/iorclient.egg-info/
+-rw-rw-rw-   0        0        0      965 2023-07-18 18:09:12.000000 iorclient-0.0.2/iorclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-07-18 18:09:12.000000 iorclient-0.0.2/iorclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:09:12.000000 iorclient-0.0.2/iorclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 18:09:12.000000 iorclient-0.0.2/iorclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:09:12.394496 iorclient-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-18 18:09:05.000000 iorclient-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:12.391464 iorclient-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0      873 2023-07-18 16:43:49.000000 iorclient-0.0.2/test/test_cert.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 16:25:02.000000 iorclient-0.0.2/test/test_role.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 16:25:05.000000 iorclient-0.0.2/test/test_template.py
```

### Comparing `iorclient-0.0.1/LICENSE` & `iorclient-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/PKG-INFO` & `iorclient-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 0.0.1
+Version: 0.0.2
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iorclient-0.0.1/ior/client/certificate_service.py` & `iorclient-0.0.2/ior/client/certificate_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/client/contract_template_service.py` & `iorclient-0.0.2/ior/client/contract_template_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/client/permission_control_service.py` & `iorclient-0.0.2/ior/client/permission_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/client/role_control_service.py` & `iorclient-0.0.2/ior/client/role_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/client/template_control_service.py` & `iorclient-0.0.2/ior/client/template_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/iorsdk.py` & `iorclient-0.0.2/ior/iorsdk.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/util/result_utils.py` & `iorclient-0.0.2/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/ior/util/web3_utils.py` & `iorclient-0.0.2/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.1/iorclient.egg-info/PKG-INFO` & `iorclient-0.0.2/iorclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 0.0.1
+Version: 0.0.2
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iorclient-0.0.1/iorclient.egg-info/SOURCES.txt` & `iorclient-0.0.2/iorclient.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 setup.py
 ior/__init__.py
 ior/iorsdk.py
 ior/client/__init__.py
 ior/client/certificate_service.py
 ior/client/contract_template_service.py
+ior/client/exchange_service.py
 ior/client/permission_control_service.py
 ior/client/role_control_service.py
 ior/client/template_control_service.py
 ior/util/__init__.py
 ior/util/result_utils.py
 ior/util/web3_utils.py
 iorclient.egg-info/PKG-INFO
```

### Comparing `iorclient-0.0.1/setup.py` & `iorclient-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="iorclient",
-  version="0.0.1",
+  version="0.0.2",
   author="Jie Guan",
   author_email="jguanisme@163.com",
   description="ior client sdk for ior standard",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/tzspace-ior/iorclient",
   packages=setuptools.find_packages(),
```

### Comparing `iorclient-0.0.1/test/test_cert.py` & `iorclient-0.0.2/test/test_cert.py`

 * *Files identical despite different names*

