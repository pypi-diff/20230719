# Comparing `tmp/libtimed-0.2.0.tar.gz` & `tmp/libtimed-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.2.0.tar", max compression
+gzip compressed data, was "libtimed-0.2.1.tar", max compression
```

## Comparing `libtimed-0.2.0.tar` & `libtimed-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-19 08:42:12.677515 libtimed-0.2.0/LICENSE
--rw-r--r--   0        0        0      750 2023-07-19 08:42:12.677515 libtimed-0.2.0/README.md
--rw-r--r--   0        0        0     1281 2023-07-19 08:42:14.549555 libtimed-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9387 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/models.py
--rw-r--r--   0        0        0     4533 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6026 2023-07-19 08:42:12.681515 libtimed-0.2.0/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 libtimed-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-19 10:23:55.899385 libtimed-0.2.1/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-19 10:23:55.899385 libtimed-0.2.1/README.md
+-rw-r--r--   0        0        0     1281 2023-07-19 10:23:56.743418 libtimed-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1061 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9387 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/models.py
+-rw-r--r--   0        0        0     4533 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6026 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 libtimed-0.2.1/PKG-INFO
```

### Comparing `libtimed-0.2.0/LICENSE` & `libtimed-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.0/README.md` & `libtimed-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.0/pyproject.toml` & `libtimed-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
```

### Comparing `libtimed-0.2.0/src/libtimed/__init__.py` & `libtimed-0.2.1/src/libtimed/__init__.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.0/src/libtimed/models.py` & `libtimed-0.2.1/src/libtimed/models.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.0/src/libtimed/oidc.py` & `libtimed-0.2.1/src/libtimed/oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def __init__(self, client_id, sso_url, sso_realm, auth_path):
         self.client_id = client_id
         self.sso_url = sso_url
         self.sso_realm = sso_realm
         self.auth_path = auth_path
 
     def autoconfig(self):
-        data = requests.get(f"{self.sso_ur}l/auth/realms/{self.sso_realm}/.well-known/openid-configuration").json()
+        data = requests.get(f"{self.sso_url}/auth/realms/{self.sso_realm}/.well-known/openid-configuration").json()
         self.authorization_endpoint = data["authorization_endpoint"]
         self.token_endpoint = data["token_endpoint"]
 
     def start_browser_flow(self):
         # construct the authorization request
         auth_url = f"{self.authorization_endpoint}?client_id={self.client_id}&response_type=code&scope=openid&redirect_uri=http://localhost:5000/{self.auth_path}"
         # start a temporary web server
```

### Comparing `libtimed-0.2.0/src/libtimed/transforms.py` & `libtimed-0.2.1/src/libtimed/transforms.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.0/PKG-INFO` & `libtimed-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

