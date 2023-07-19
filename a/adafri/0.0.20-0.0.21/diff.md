# Comparing `tmp/adafri-0.0.20.tar.gz` & `tmp/adafri-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.20.tar", last modified: Wed Jul 19 01:10:02 2023, max compression
+gzip compressed data, was "adafri-0.0.21.tar", last modified: Wed Jul 19 01:14:12 2023, max compression
```

## Comparing `adafri-0.0.20.tar` & `adafri-0.0.21.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.220259 adafri-0.0.20/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:10:02.219881 adafri-0.0.20/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.179476 adafri-0.0.20/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-19 01:09:56.000000 adafri-0.0.20/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.188059 adafri-0.0.20/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.20/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.20/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15537 2023-07-18 21:41:25.000000 adafri-0.0.20/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.189022 adafri-0.0.20/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.20/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.191135 adafri-0.0.20/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.20/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.201111 adafri-0.0.20/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.20/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.20/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.20/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.202596 adafri-0.0.20/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.20/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.204169 adafri-0.0.20/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.20/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.20/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.205077 adafri-0.0.20/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.20/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.205596 adafri-0.0.20/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.20/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.211393 adafri-0.0.20/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    14107 2023-07-19 01:08:51.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3390 2023-07-19 01:05:15.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9108 2023-07-19 01:09:43.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:02:50.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.213586 adafri-0.0.20/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.20/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1345 2023-07-18 00:33:08.000000 adafri-0.0.20/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2655 2023-07-18 00:34:16.000000 adafri-0.0.20/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.215486 adafri-0.0.20/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.20/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.20/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.216090 adafri-0.0.20/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.20/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.218850 adafri-0.0.20/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.20/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.20/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.20/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.181844 adafri-0.0.20/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-19 01:10:02.220397 adafri-0.0.20/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.20/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.065880 adafri-0.0.21/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:14:12.065300 adafri-0.0.21/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.007830 adafri-0.0.21/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-19 01:14:07.000000 adafri-0.0.21/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.015353 adafri-0.0.21/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.21/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.21/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15537 2023-07-18 21:41:25.000000 adafri-0.0.21/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.016936 adafri-0.0.21/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.21/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.018239 adafri-0.0.21/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.21/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.026561 adafri-0.0.21/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.21/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.21/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.21/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.027700 adafri-0.0.21/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.21/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.030409 adafri-0.0.21/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.21/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.21/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.032539 adafri-0.0.21/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.21/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.033216 adafri-0.0.21/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.21/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.041375 adafri-0.0.21/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    14107 2023-07-19 01:08:51.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3390 2023-07-19 01:05:15.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9108 2023-07-19 01:09:43.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:02:50.000000 adafri-0.0.21/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.045487 adafri-0.0.21/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.21/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1355 2023-07-19 01:13:12.000000 adafri-0.0.21/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2663 2023-07-19 01:13:55.000000 adafri-0.0.21/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.048831 adafri-0.0.21/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.21/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.21/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.050616 adafri-0.0.21/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.21/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.063852 adafri-0.0.21/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.21/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.21/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.21/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:14:12.011526 adafri-0.0.21/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:14:11.000000 adafri-0.0.21/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-19 01:14:11.000000 adafri-0.0.21/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-19 01:14:11.000000 adafri-0.0.21/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-19 01:14:11.000000 adafri-0.0.21/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-19 01:14:12.066130 adafri-0.0.21/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.21/setup.py
```

### Comparing `adafri-0.0.20/adafri/utils/response.py` & `adafri-0.0.21/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/utils/utils.py` & `adafri-0.0.21/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/account/models/account.py` & `adafri-0.0.21/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/account/models/account_fields.py` & `adafri-0.0.21/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.21/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.21/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.21/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.21/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.21/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.21/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.21/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.21/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.21/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 )
 from ...oauth import (OAuthClient, OAuthToken, OpenIDAuthorizationCodeGrant as AuthCodeGrant,TokenValidator)
 from ...oauth import OpenIDImplicitGrant, OpenIDHybridGrant, OpenIDCode
 
 oidc_authorization_server = AuthorizationServer()
 require_oidc_oauth = ResourceProtector()
 
-def config_oidc_oauth(app, query_client=None, save_token=None, token_generator=None):
+def config_oidc_oauth(app, query_client=None, save_token=None, token_generators=[]):
     if query_client is None:
         query_client = OAuthClient().get_by_client_id
     if save_token is None:
         save_token = OAuthToken().save
     oidc_authorization_server.query_client = query_client
     oidc_authorization_server.save_token = save_token
     oidc_authorization_server.init_app(app)
     oidc_authorization_server.register_grant(AuthCodeGrant, [
         OpenIDCode(require_nonce=True),
     ])
     oidc_authorization_server.register_grant(OpenIDImplicitGrant)
     oidc_authorization_server.register_grant(OpenIDHybridGrant)
-    if token_generator is not None:
+    for token_generator in token_generators:
         type = getattr(token_generator, 'type', None);
         generator = getattr(token_generator, 'generator', None);
         if None not in [type, generator]:
             oidc_authorization_server.register_token_generator(type, generator)
-    require_oidc_oauth.register_token_validator(TokenValidator())
+    require_oidc_oauth.register_token_validator(TokenValidator())
+
```

### Comparing `adafri-0.0.20/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.21/adafri/v1/auth/oauth/server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #     save_token=OAuthToken().save,
 # )
 authorization_server = AuthorizationServer()
 require_oauth = ResourceProtector()
 
 require_oauth = ResourceProtector()
 
-def config_oauth(app, query_client=None, save_token=None, token_generator=None):
+def config_oauth(app, query_client=None, save_token=None, token_generators=[]):
     if query_client is None:
         query_client = OAuthClient().get_by_client_id
     if save_token is None:
         save_token = OAuthToken().save
     authorization_server.query_client = query_client
     authorization_server.save_token = save_token
     authorization_server.init_app(app)
@@ -46,15 +46,15 @@
     authorization_server.register_grant(AuthCodeGrant, [CodeChallenge(required=True)])
     
     # authorization_server.register_grant(PasswordGrant)
     authorization_server.register_grant(RefreshTokenGrant)
     # support revocation
     # revocation_cls = create_revocation_endpoint()
     authorization_server.register_endpoint(TokenRevocationEndpoint)
-    if token_generator is not None:
+    for token_generator in token_generators:
         type = getattr(token_generator, 'type', None);
         generator = getattr(token_generator, 'generator', None);
         if None not in [type, generator]:
             authorization_server.register_token_generator(type, generator)
     # authorization_server.register_token_generator("default", TokenGenerator.generate)
     # authorization_server.register_token_generator("client_credentials", TokenGenerator.generate)
     # protect resource
```

### Comparing `adafri-0.0.20/adafri/v1/base/firebase_collection.py` & `adafri-0.0.21/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/user/models/user.py` & `adafri-0.0.21/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri/v1/user/models/user_fields.py` & `adafri-0.0.21/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/adafri.egg-info/SOURCES.txt` & `adafri-0.0.21/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.20/setup.py` & `adafri-0.0.21/setup.py`

 * *Files identical despite different names*

