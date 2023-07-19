# Comparing `tmp/adafri-0.0.19.44.tar.gz` & `tmp/adafri-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.44.tar", last modified: Tue Jul 18 21:42:03 2023, max compression
+gzip compressed data, was "adafri-0.0.20.tar", last modified: Wed Jul 19 01:10:02 2023, max compression
```

## Comparing `adafri-0.0.19.44.tar` & `adafri-0.0.20.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.405754 adafri-0.0.19.44/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-18 21:42:03.405199 adafri-0.0.19.44/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.376405 adafri-0.0.19.44/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-18 21:41:47.000000 adafri-0.0.19.44/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.381420 adafri-0.0.19.44/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.44/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.44/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15537 2023-07-18 21:41:25.000000 adafri-0.0.19.44/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.383139 adafri-0.0.19.44/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.44/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.384103 adafri-0.0.19.44/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.44/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.386676 adafri-0.0.19.44/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.44/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.44/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.44/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.387459 adafri-0.0.19.44/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.44/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.389050 adafri-0.0.19.44/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.44/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.44/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.389874 adafri-0.0.19.44/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.44/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.390610 adafri-0.0.19.44/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.396694 adafri-0.0.19.44/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    14112 2023-07-17 04:35:50.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9130 2023-07-18 00:36:13.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.399232 adafri-0.0.19.44/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1345 2023-07-18 00:33:08.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2655 2023-07-18 00:34:16.000000 adafri-0.0.19.44/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.400861 adafri-0.0.19.44/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.44/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.44/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.401687 adafri-0.0.19.44/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.44/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.404079 adafri-0.0.19.44/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.44/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.44/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.44/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 21:42:03.378946 adafri-0.0.19.44/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-18 21:42:03.000000 adafri-0.0.19.44/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-18 21:42:03.000000 adafri-0.0.19.44/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-18 21:42:03.000000 adafri-0.0.19.44/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-18 21:42:03.000000 adafri-0.0.19.44/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-18 21:42:03.406005 adafri-0.0.19.44/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.44/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.220259 adafri-0.0.20/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:10:02.219881 adafri-0.0.20/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.179476 adafri-0.0.20/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-19 01:09:56.000000 adafri-0.0.20/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.188059 adafri-0.0.20/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.20/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.20/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15537 2023-07-18 21:41:25.000000 adafri-0.0.20/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.189022 adafri-0.0.20/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.20/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.191135 adafri-0.0.20/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.20/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.201111 adafri-0.0.20/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.20/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.20/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.20/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.202596 adafri-0.0.20/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.20/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.204169 adafri-0.0.20/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.20/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.20/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.205077 adafri-0.0.20/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.20/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.205596 adafri-0.0.20/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.20/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.211393 adafri-0.0.20/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    14107 2023-07-19 01:08:51.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3390 2023-07-19 01:05:15.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9108 2023-07-19 01:09:43.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:02:50.000000 adafri-0.0.20/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.213586 adafri-0.0.20/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.20/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1345 2023-07-18 00:33:08.000000 adafri-0.0.20/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2655 2023-07-18 00:34:16.000000 adafri-0.0.20/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.215486 adafri-0.0.20/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.20/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.20/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.216090 adafri-0.0.20/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.20/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.218850 adafri-0.0.20/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.20/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.20/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.20/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:10:02.181844 adafri-0.0.20/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-19 01:10:02.000000 adafri-0.0.20/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-19 01:10:02.220397 adafri-0.0.20/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.20/setup.py
```

### Comparing `adafri-0.0.19.44/adafri/utils/response.py` & `adafri-0.0.20/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/utils/utils.py` & `adafri-0.0.20/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/account/models/account.py` & `adafri-0.0.20/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/account/models/account_fields.py` & `adafri-0.0.20/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.20/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.20/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.20/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.20/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.20/adafri/v1/auth/oauth/models/grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,25 +153,26 @@
         'client_secret_post',
         'none'
     ]
     def save_authorization_code(self, code, request):
         code_challenge = request.data.get('code_challenge')
         code_challenge_method = request.data.get('code_challenge_method')
         redirect_uri = request.redirect_uri;
+        scope = request.args.get("scope")
         if request.args.get("redirect_uri") is not None:
             redirect_uri = request.args.get("redirect_uri");
         if redirect_uri is None:
             default_redirect_uri =os.environ.get('DEFAULT_REDIRECT_URI')
             redirect_uri = default_redirect_uri
         model = {
             "client_id": request.client.client_id,
             "code": code,
             "redirect_uri": redirect_uri,
-            "scopes": ArrayUtils.join_string_to_array(request.args.get("scope"), ","),
-            "scope": request.args.get("scope"),
+            "scopes": scope_to_list(scope),
+            "scope": scope,
             "uid": request.user.uid,
             "code_challenge": code_challenge,
             "code_challenge_method": code_challenge_method
         }
         auth_code_request = OAuthGrant.create(**model)
         auth_code = auth_code_request.data
         return auth_code
@@ -255,30 +256,32 @@
         'none'
     ]
     def save_authorization_code(self, code, request):
         code_challenge = request.data.get('code_challenge')
         code_challenge_method = request.data.get('code_challenge_method')
         redirect_uri = request.redirect_uri;
         nonce = request.data.get('nonce')
+        scope = request.args.get("scope")
         if request.args.get("redirect_uri") is not None:
             redirect_uri = request.args.get("redirect_uri");
         if redirect_uri is None:
             default_redirect_uri =os.environ.get('DEFAULT_REDIRECT_URI')
             redirect_uri = default_redirect_uri
         model = {
             "client_id": request.client.client_id,
             "code": code,
             "redirect_uri": redirect_uri,
-            "scopes": ArrayUtils.join_string_to_array(request.args.get("scope"), ","),
-            "scope": request.args.get("scope"),
+            "scopes": scope_to_list(scope),
+            "scope": scope,
             "uid": request.user.uid,
             "code_challenge": code_challenge,
             "code_challenge_method": code_challenge_method,
-            "nonce": nonce,
         }
+        if nonce is not None:
+            model['nonce'] = nonce
         auth_code_request = OAuthGrant.create(**model)
         auth_code = auth_code_request.data
         return auth_code
     
     def create_authorization_code(self, client, grant_user, request):
         return create_authorization_code(client, grant_user, request)
```

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.20/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 
 from dataclasses import dataclass
 from .....utils.utils import DictUtils
+from datetime import datetime, timedelta
 
 GRANT_COLLECTION = "clients_grant_collection";
+
+def get_grant_expire_at(expires_in):
+    return datetime.now() + timedelta(seconds=expires_in)
 @dataclass
 class GrantFields:
     id = "id"
     code = "code"
     uid = "uid"
     client_id = "client_id"
     redirect_uri = "redirect_uri"
@@ -74,24 +78,24 @@
     },
     GrantFields.scopes: {
         "type": list,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
-        "default_value": "",
+        "default_value": [],
         "pickable": True
     },
     GrantFields.expires: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
-        "default_value": "",
+        "default_value": get_grant_expire_at(120).isoformat(),
         "pickable": True
     },
     GrantFields.scope: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
```

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.20/adafri/v1/auth/oauth/models/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from .....utils import DictUtils, Crypto, get_object_model_class, pydash, init_class_kwargs
 from ....base.firebase_collection import (FirebaseCollectionBase, getTimestamp)
-from .token_fields import TokenFields, TokenFieldsProps, STANDARD_FIELDS, TOKEN_COLLECTION
+from .token_fields import TokenFields, TokenFieldsProps, STANDARD_FIELDS, TOKEN_COLLECTION, get_token_expire_at, is_expired
 from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
 from typing import Any
 from dataclasses import dataclass
 from ....user import User
 from authlib.oauth2.rfc7009 import RevocationEndpoint
 from authlib.oauth2.rfc6750 import BearerTokenValidator
 from authlib.oauth2.rfc6749 import grants
 from authlib.oauth2.rfc6749 import TokenMixin, scope_to_list
 from authlib.oauth2.rfc6750 import BearerTokenGenerator
-from datetime import datetime, timedelta
 import json
 from flask import abort, Response
 
 @dataclass(init=False)
 class OAuthToken(TokenMixin, FirebaseCollectionBase):
     id: str
     client_id: str
@@ -84,15 +83,15 @@
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
 
         token_model.id = Crypto().generate_id(token_model.access_token+"~"+token_model.client_id);
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, token_model, None);
     
 
     def save(self, token, request):
-        model = {**token, "client_id": request.client.client_id, "uid": request.client.uid, "revoked": False}
+        model = {**token, "client_id": request.client.client_id, "uid": request.user.uid, "revoked": False}
         token_generate = OAuthToken.generate(**model);
         if token_generate.status == ResponseStatus.ERROR:
             return token_generate
         docRef = OAuthToken(token_generate.data.to_json()).document_reference();
         if docRef.get().exists:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
         
@@ -123,15 +122,15 @@
             deleted = self.document_reference().delete();
             return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Token {self.id} deleted"}, None);
         except:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id}","INVALID_REQUEST", 1));
 
 
     def is_expired(self):
-        return datetime.fromisoformat(self.expired_at) < datetime.now()
+        return is_expired(self.expired_at)
     
     def is_revoked(self):
         return self.revoked
     
 
 class TokenValidator(BearerTokenValidator):
     def authenticate_token(self, token_string):
@@ -185,14 +184,14 @@
     @staticmethod
     def generate(grant_type, client, user=None, scope=None, expires_in=None, include_refresh_token=True):
         if expires_in is None:
             expires_in = DEFAULT_EXPIRES_IN
         uid = client.uid;
         if user is not None:
             uid = user.uid
-        expires_at = datetime.now() + timedelta(seconds=expires_in)
-        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
+        expires_at = get_token_expire_at(expires_in).isoformat()
+        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": uid, 'scope': scope, 'scopes': scope_to_list(scope), 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at}
         access_token = Crypto().generate_token("access_token~"+json.dumps(token));
         token['access_token'] = access_token;
         if include_refresh_token:
             token['refresh_token'] = Crypto().generate_token("refresh_token~"+json.dumps(token));
         return token
```

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.20/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 from dataclasses import dataclass
 from .....utils import DictUtils
+from datetime import datetime, timedelta
 
 TOKEN_COLLECTION = "clients_token_collection";
+
+def get_token_expire_at(expires_in):
+    return datetime.now() + timedelta(seconds=expires_in)
+
+
+def is_expired(expired_at):
+    return datetime.fromisoformat(expired_at) < datetime.now()
+
 @dataclass
 class TokenFields:
     id = "id"
     client_id = "client_id"
     uid = "uid"
     token_type = "token_type"
     access_token = "access_token"
@@ -91,15 +100,15 @@
     },
     TokenFields.scopes: {
         "type": list,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
-        "default_value": "",
+        "default_value": [],
         "pickable": True
     },
     TokenFields.expires: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
@@ -118,13 +127,13 @@
     },
     TokenFields.expired_at: {
         "type": float,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
-        "default_value": 0,
+        "default_value": get_token_expire_at(3600).isoformat(),
         "pickable": True
     },
 }
 
 STANDARD_FIELDS = TokenFields.filtered_keys('pickable', True)
```

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.20/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.20/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/base/firebase_collection.py` & `adafri-0.0.20/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/user/models/user.py` & `adafri-0.0.20/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri/v1/user/models/user_fields.py` & `adafri-0.0.20/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/adafri.egg-info/SOURCES.txt` & `adafri-0.0.20/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.44/setup.py` & `adafri-0.0.20/setup.py`

 * *Files identical despite different names*

