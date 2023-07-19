# Comparing `tmp/libtimed-0.1.0.tar.gz` & `tmp/libtimed-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.1.0.tar", max compression
+gzip compressed data, was "libtimed-0.2.0.tar", max compression
```

## Comparing `libtimed-0.1.0.tar` & `libtimed-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-18 07:55:06.174247 libtimed-0.1.0/LICENSE
--rw-r--r--   0        0        0      750 2023-07-18 07:55:06.174247 libtimed-0.1.0/README.md
--rw-r--r--   0        0        0     1281 2023-07-18 07:55:06.902252 libtimed-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-07-18 07:55:06.174247 libtimed-0.1.0/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9387 2023-07-18 07:55:06.174247 libtimed-0.1.0/src/libtimed/models.py
--rw-r--r--   0        0        0     4302 2023-07-18 07:55:06.174247 libtimed-0.1.0/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6026 2023-07-18 07:55:06.174247 libtimed-0.1.0/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 libtimed-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-19 08:42:12.677515 libtimed-0.2.0/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-19 08:42:12.677515 libtimed-0.2.0/README.md
+-rw-r--r--   0        0        0     1281 2023-07-19 08:42:14.549555 libtimed-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1061 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9387 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/models.py
+-rw-r--r--   0        0        0     4533 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6026 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 libtimed-0.2.0/PKG-INFO
```

### Comparing `libtimed-0.1.0/LICENSE` & `libtimed-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.1.0/README.md` & `libtimed-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.1.0/pyproject.toml` & `libtimed-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.1.0"
+version = "0.2.0"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
```

### Comparing `libtimed-0.1.0/src/libtimed/__init__.py` & `libtimed-0.2.0/src/libtimed/__init__.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.1.0/src/libtimed/models.py` & `libtimed-0.2.0/src/libtimed/models.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.1.0/src/libtimed/oidc.py` & `libtimed-0.2.0/src/libtimed/oidc.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,20 +37,25 @@
 
     # disable logging as it is too verbose
     def log_message(self, *args, **kwargs):
         pass
 
 
 class OIDCClient:
-    def __init__(self, client_id, authorization_endpoint, token_endpoint, auth_path):
+    def __init__(self, client_id, sso_url, sso_realm, auth_path):
         self.client_id = client_id
-        self.authorization_endpoint = authorization_endpoint
-        self.token_endpoint = token_endpoint
+        self.sso_url = sso_url
+        self.sso_realm = sso_realm
         self.auth_path = auth_path
 
+    def autoconfig(self):
+        data = requests.get(f"{self.sso_ur}l/auth/realms/{self.sso_realm}/.well-known/openid-configuration").json()
+        self.authorization_endpoint = data["authorization_endpoint"]
+        self.token_endpoint = data["token_endpoint"]
+
     def start_browser_flow(self):
         # construct the authorization request
         auth_url = f"{self.authorization_endpoint}?client_id={self.client_id}&response_type=code&scope=openid&redirect_uri=http://localhost:5000/{self.auth_path}"
         # start a temporary web server
         server = http.server.HTTPServer(("localhost", 5000), OIDCHTTPRequestHandler)
         # open the browser to the authorization URL
         webbrowser.open_new(auth_url)
@@ -112,14 +117,15 @@
 
     def authorize(self):
         cached_token = self.keyring_get()
         if cached_token:
             if self.check_expired(cached_token):
                 return cached_token
 
+        self.autoconfig()
         if self.start_browser_flow():
             token = self.get_token()
             if not token:
                 return False
             self.keyring_set(token)
             return token
         else:
```

### Comparing `libtimed-0.1.0/src/libtimed/transforms.py` & `libtimed-0.2.0/src/libtimed/transforms.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.1.0/PKG-INFO` & `libtimed-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

