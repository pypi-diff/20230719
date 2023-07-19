# Comparing `tmp/adafri-0.0.22.tar.gz` & `tmp/adafri-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.22.tar", last modified: Wed Jul 19 01:38:56 2023, max compression
+gzip compressed data, was "adafri-0.0.23.tar", last modified: Wed Jul 19 01:58:30 2023, max compression
```

## Comparing `adafri-0.0.22.tar` & `adafri-0.0.23.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.289659 adafri-0.0.22/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:38:56.289126 adafri-0.0.22/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.251576 adafri-0.0.22/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-19 01:38:51.000000 adafri-0.0.22/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.257249 adafri-0.0.22/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.22/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.22/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15537 2023-07-19 01:36:03.000000 adafri-0.0.22/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.257798 adafri-0.0.22/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.22/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.263681 adafri-0.0.22/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.22/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.266886 adafri-0.0.22/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.22/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.22/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.22/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.267906 adafri-0.0.22/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.22/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.269550 adafri-0.0.22/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.22/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.22/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.270568 adafri-0.0.22/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.22/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.270962 adafri-0.0.22/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.22/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.278676 adafri-0.0.22/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    14107 2023-07-19 01:08:51.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3390 2023-07-19 01:05:15.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9109 2023-07-19 01:33:29.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.22/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.281645 adafri-0.0.22/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.22/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1355 2023-07-19 01:13:12.000000 adafri-0.0.22/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2663 2023-07-19 01:13:55.000000 adafri-0.0.22/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.284221 adafri-0.0.22/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.22/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.22/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.284923 adafri-0.0.22/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.22/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.287880 adafri-0.0.22/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.22/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.22/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.22/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:38:56.254651 adafri-0.0.22/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:38:56.000000 adafri-0.0.22/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-19 01:38:56.000000 adafri-0.0.22/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-19 01:38:56.000000 adafri-0.0.22/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-19 01:38:56.000000 adafri-0.0.22/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-19 01:38:56.289913 adafri-0.0.22/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.22/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.337530 adafri-0.0.23/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:58:30.337058 adafri-0.0.23/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.285354 adafri-0.0.23/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-19 01:58:14.000000 adafri-0.0.23/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.290519 adafri-0.0.23/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.23/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.23/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16188 2023-07-19 01:58:09.000000 adafri-0.0.23/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.291234 adafri-0.0.23/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.23/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.292407 adafri-0.0.23/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.23/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.296055 adafri-0.0.23/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.23/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.23/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.23/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.297759 adafri-0.0.23/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.23/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.299148 adafri-0.0.23/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.23/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.23/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.300268 adafri-0.0.23/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.23/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.301008 adafri-0.0.23/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.23/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.310972 adafri-0.0.23/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    14107 2023-07-19 01:08:51.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3390 2023-07-19 01:05:15.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9109 2023-07-19 01:33:29.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.23/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.320800 adafri-0.0.23/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.23/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1355 2023-07-19 01:13:12.000000 adafri-0.0.23/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2663 2023-07-19 01:13:55.000000 adafri-0.0.23/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.326303 adafri-0.0.23/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.23/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.23/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.328143 adafri-0.0.23/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.23/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.335673 adafri-0.0.23/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.23/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.23/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.23/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-19 01:58:30.287582 adafri-0.0.23/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-19 01:58:30.000000 adafri-0.0.23/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-19 01:58:30.000000 adafri-0.0.23/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-19 01:58:30.000000 adafri-0.0.23/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-19 01:58:30.000000 adafri-0.0.23/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-19 01:58:30.337736 adafri-0.0.23/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.23/setup.py
```

### Comparing `adafri-0.0.22/adafri/utils/response.py` & `adafri-0.0.23/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/utils/utils.py` & `adafri-0.0.23/adafri/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,26 @@
     from urllib.parse import urlencode
     url_parts = list(urlparse.urlparse(input_url))
     query = dict(urlparse.parse_qsl(url_parts[4]))
     query.update(params)
     url_parts[4] = urlencode(query)
     return urlparse.urlunparse(url_parts)
 
+def encode_base64(data: str):
+    string_bytes = data.encode("ascii")
+    base64_bytes = base64.b64encode(string_bytes)
+    base64_string = base64_bytes.decode("ascii")
+    return base64_string;
+
+def decode_base64(data_base64: str):
+    base64_bytes = data_base64.encode("ascii")
+    string_bytes = base64.b64decode(base64_bytes)
+    decoded_string = string_bytes.decode("ascii")
+    return decoded_string
+
 class Crypto:
 
     print(ENCRYPTION_KEY)
     print(hash.hexdigest())
     fernet = Fernet(ENCRYPTION_KEY);
     def encrypt(self, message:str):
         return self.fernet.encrypt(message.encode()).decode();
@@ -34,15 +46,25 @@
     def hash(self, message:str):
         return hashlib.sha256(str(message).encode()).hexdigest();
     
     def generate_id(self, message:str):
         return hashlib.md5(str(message).encode()).hexdigest();
 
     def generate_token(self, message:str):
-        return self.encrypt("token~"+hashlib.md5(str(message).encode()).hexdigest())
+        return encode_base64(self.encrypt("token~"+message))
+    
+    def decrypt_token(self, message:str):
+        try:
+            d = self.decrypt(decode_base64(message));
+            token_split = d.split('~');
+            token = json.loads(token_split[1])
+            return token
+        except:
+            return None;
+
 
 class RequestFields:
     data = 'data';
     fields = 'fields';
 
 def get_request_fields(field_string, fields, default_fields):
     request_fields =[];
```

### Comparing `adafri-0.0.22/adafri/v1/account/models/account.py` & `adafri-0.0.23/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/account/models/account_fields.py` & `adafri-0.0.23/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.23/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.23/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.23/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.23/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.23/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.23/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.23/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.23/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.23/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.23/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/base/firebase_collection.py` & `adafri-0.0.23/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/user/models/user.py` & `adafri-0.0.23/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri/v1/user/models/user_fields.py` & `adafri-0.0.23/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/adafri.egg-info/SOURCES.txt` & `adafri-0.0.23/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.22/setup.py` & `adafri-0.0.23/setup.py`

 * *Files identical despite different names*

