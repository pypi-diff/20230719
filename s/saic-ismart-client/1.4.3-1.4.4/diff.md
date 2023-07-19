# Comparing `tmp/saic_ismart_client-1.4.3.tar.gz` & `tmp/saic_ismart_client-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.3.tar", last modified: Tue Jul 18 18:02:11 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.4.tar", last modified: Tue Jul 18 18:21:32 2023, max compression
```

## Comparing `saic_ismart_client-1.4.3.tar` & `saic_ismart_client-1.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.937383 saic_ismart_client-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.937383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    44179 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.307329 saic_ismart_client-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:21:32.307329 saic_ismart_client-1.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.299329 saic_ismart_client-1.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.299329 saic_ismart_client-1.4.4/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.299329 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44089 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 18:21:32.000000 saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-18 18:21:32.000000 saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:21:32.000000 saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 18:21:32.000000 saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 18:21:32.000000 saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:21:32.303329 saic_ismart_client-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-18 18:21:20.000000 saic_ismart_client-1.4.4/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.3/LICENSE` & `saic_ismart_client-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/PKG-INFO` & `saic_ismart_client-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.4.3
+Version: 1.4.4
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.3/README.md` & `saic_ismart_client-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/pyproject.toml` & `saic_ismart_client-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/common_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,69 @@
 FIELD_MNC_SIM = 'mncSim'
 FIELD_MCC_SIM = 'mccSim'
 FIELD_MNC_NETWORK = 'mncNetwork'
 FIELD_MCC_NETWORK = 'mccNetwork'
 FIELD_SIGNAL_STRENGTH = 'signalStrength'
 
 
+class ScheduledChargingMode(Enum):
+    DISABLED = 2
+    UNTIL_CONFIGURED_SOC = 3
+    UNTIL_CONFIGURED_TIME = 1
+
+
+class TargetBatteryCode(Enum):
+    P_40 = 1
+    P_50 = 2
+    P_60 = 3
+    P_70 = 4
+    P_80 = 5
+    P_90 = 6
+    P_100 = 7
+
+    def get_percentage(self) -> int:
+        match self:
+            case TargetBatteryCode.P_40:
+                return 40
+            case TargetBatteryCode.P_50:
+                return 50
+            case TargetBatteryCode.P_60:
+                return 60
+            case TargetBatteryCode.P_70:
+                return 70
+            case TargetBatteryCode.P_80:
+                return 80
+            case TargetBatteryCode.P_90:
+                return 90
+            case TargetBatteryCode.P_100:
+                return 100
+            case _:
+                raise ValueError(f'Unknown target battery code: {self}')
+
+    @staticmethod
+    def from_percentage(percentage: int):
+        match percentage:
+            case 40:
+                return TargetBatteryCode.P_40
+            case 50:
+                return TargetBatteryCode.P_50
+            case 60:
+                return TargetBatteryCode.P_60
+            case 70:
+                return TargetBatteryCode.P_70
+            case 80:
+                return TargetBatteryCode.P_80
+            case 90:
+                return TargetBatteryCode.P_90
+            case 100:
+                return TargetBatteryCode.P_100
+            case _:  # default
+                raise ValueError(f'Unknown target battery percentage: {percentage}')
+
+
 class Header:
     def __init__(self):
         self.protocol_version = None
         self.security_context = None
         self.dispatcher_message_length = None
         self.dispatcher_body_encoding = None
 
@@ -480,15 +535,15 @@
         self.uplink_counter = data.get(FIELD_UPLINK_COUNTER)
         self.downlink_counter = data.get(FIELD_DOWNLINK_COUNTER)
 
 
 class BasicPosition(Asn1Type):
     def __init__(self):
         super().__init__('BasicPosition')
-        self. latitude = None
+        self.latitude = None
         self.longitude = None
 
     def get_data(self) -> dict:
         return {
             FIELD_LATITUDE: self.latitude,
             FIELD_LONGITUDE: self.longitude
         }
```

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.4/src/saic_ismart_client/saic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import urllib.parse
 from enum import Enum
 from typing import cast
 
 import requests as requests
 
 from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2, \
-    TargetBatteryCode
+    ScheduledChargingMode, TargetBatteryCode
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
 from saic_ismart_client.ota_v1_1.data_model import AbortSendMessageReq, AlarmSwitch, AlarmSwitchReq, Message, \
     MessageBodyV11, MessageListReq, MessageListResp, MessageV11, MpAlarmSettingType, MpUserLoggingInReq, \
     MpUserLoggingInRsp, StartEndNumber, Timestamp, VinInfo
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
 from saic_ismart_client.ota_v2_1.data_model import OtaRvcReq, OtaRvcStatus25857, OtaRvmVehicleStatusReq, \
     OtaRvmVehicleStatusResp25857, RvcReqParam
@@ -22,20 +22,14 @@
     OtaChrgHeatResp, OtaChrgMangDataResp, OtaChrgRsvanReq, OtaChrgSetngReq, OtaChrgSetngResp, OtaChrgRsvanResp
 
 UID_INIT = '0000000000000000000000000000000000000000000000000#'
 AVG_SMS_DELIVERY_TIME = 15
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.INFO)
 
 
-class ScheduledChargingMode(Enum):
-    DISABLED = 2
-    UNTIL_CONFIGURED_SOC = 3
-    UNTIL_CONFIGURED_TIME = 1
-
-
 class SaicMessage:
     def __init__(self, message_id: int, message_type: str, title: str, message_time: datetime, sender: str,
                  content: str, read_status: int, vin: str):
         self.message_id = message_id
         self.message_type = message_type
         self.title = title
         self.message_time = message_time
```

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.4.3
+Version: 1.4.4
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.4/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.4/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.4/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.4/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/tests/test_abrp_api.py` & `saic_ismart_client-1.4.4/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.3/tests/test_saic_api.py` & `saic_ismart_client-1.4.4/tests/test_saic_api.py`

 * *Files identical despite different names*

