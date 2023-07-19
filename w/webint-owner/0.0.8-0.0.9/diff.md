# Comparing `tmp/webint_owner-0.0.8.tar.gz` & `tmp/webint_owner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_owner-0.0.8.tar", max compression
+gzip compressed data, was "webint_owner-0.0.9.tar", max compression
```

## Comparing `webint_owner-0.0.8.tar` & `webint_owner-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      847 2023-03-12 23:27:28.920059 webint_owner-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5351 2023-03-12 23:19:59.557440 webint_owner-0.0.8/webint_owner/__init__.py
--rw-r--r--   0        0        0       37 2023-01-27 00:43:44.008128 webint_owner-0.0.8/webint_owner/templates/__init__.py
--rw-r--r--   0        0        0      261 2023-01-27 00:43:44.012128 webint_owner-0.0.8/webint_owner/templates/claim.html
--rw-r--r--   0        0        0      425 2023-01-27 00:43:44.012128 webint_owner-0.0.8/webint_owner/templates/claimed.html
--rw-r--r--   0        0        0      371 2023-01-27 00:43:44.008128 webint_owner-0.0.8/webint_owner/templates/index.html
--rw-r--r--   0        0        0      246 2023-03-12 23:20:17.865713 webint_owner-0.0.8/webint_owner/templates/signin.html
--rw-r--r--   0        0        0       88 2023-01-27 00:43:44.008128 webint_owner-0.0.8/webint_owner/templates/signout.html
--rw-r--r--   0        0        0      149 2023-01-27 00:43:44.008128 webint_owner-0.0.8/webint_owner/templates/unauthorized.html
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 webint_owner-0.0.8/setup.py
--rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 webint_owner-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      847 2023-03-13 04:06:41.957493 webint_owner-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5285 2023-03-13 03:58:20.294919 webint_owner-0.0.9/webint_owner/__init__.py
+-rw-r--r--   0        0        0       37 2023-01-27 00:43:44.008128 webint_owner-0.0.9/webint_owner/templates/__init__.py
+-rw-r--r--   0        0        0      261 2023-01-27 00:43:44.012128 webint_owner-0.0.9/webint_owner/templates/claim.html
+-rw-r--r--   0        0        0      425 2023-01-27 00:43:44.012128 webint_owner-0.0.9/webint_owner/templates/claimed.html
+-rw-r--r--   0        0        0      371 2023-01-27 00:43:44.008128 webint_owner-0.0.9/webint_owner/templates/index.html
+-rw-r--r--   0        0        0      246 2023-03-12 23:20:17.865713 webint_owner-0.0.9/webint_owner/templates/signin.html
+-rw-r--r--   0        0        0       88 2023-01-27 00:43:44.008128 webint_owner-0.0.9/webint_owner/templates/signout.html
+-rw-r--r--   0        0        0      149 2023-01-27 00:43:44.008128 webint_owner-0.0.9/webint_owner/templates/unauthorized.html
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 webint_owner-0.0.9/setup.py
+-rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 webint_owner-0.0.9/PKG-INFO
```

### Comparing `webint_owner-0.0.8/pyproject.toml` & `webint_owner-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-owner"
-version = "0.0.8"
+version = "0.0.9"
 description = "manage website ownership"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
 packages = [{include="webint_owner"}]
 
 [tool.poetry.plugins."webapps"]
 owner = "webint_owner:app"
```

### Comparing `webint_owner-0.0.8/webint_owner/__init__.py` & `webint_owner-0.0.9/webint_owner/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,29 +83,25 @@
 
 @app.wrap
 def initialize_owner(handler, main_app):
     """Ensure an owner exists and add their details to the transaction."""
     try:
         tx.host.owner = app.model.get_identity()["card"]
     except IndexError:
-        web.header("Content-Type", "text/html")
-        app.model.add_identity("Unnamed")
-        passphrase = " ".join(app.model.update_passphrase())
-        tx.host.owner = tx.user.session = app.model.get_identity()["card"]
-        tx.user.is_owner = True
-        if kiosk := web.form(kiosk=None).kiosk:
-            with open(f"{kiosk}/passphrase", "w") as fp:
-                fp.write(passphrase)
-            raise web.SeeOther("/")
-        raise web.Created(app.view.claimed(tx.origin, passphrase), tx.origin)
-    is_owner = tx.user.session.get("uid", [None])[0] == "/"
-    try:
-        tx.user.is_owner = is_owner
-    except (AttributeError, KeyError, IndexError):
-        tx.user.is_owner = False
+        if secret := web.form(secret=None).secret:
+            if main_app.cfg.get("SECRET") != secret:
+                raise web.BadRequest("bad secret")
+            app.model.add_identity("Unnamed")
+            passphrase = " ".join(app.model.update_passphrase())
+            tx.host.owner = tx.user.session = app.model.get_identity()["card"]
+            tx.user.is_owner = True
+            web.header("Content-Type", "text/html")
+            raise web.Created(app.view.claimed(tx.origin, passphrase), tx.origin)
+        raise web.NotFound("no identity initialized")
+    tx.user.is_owner = tx.user.session.get("uid", [None])[0] == "/"
     yield
 
 
 @app.wrap
 def authorize_owner(handler, main_app):
     """Manage access to owner-only resources."""
     if not tx.user.is_owner and tx.request.method.lower() in getattr(
```

### Comparing `webint_owner-0.0.8/setup.py` & `webint_owner-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['owner = webint_owner:app']}
 
 setup_kwargs = {
     'name': 'webint-owner',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'manage website ownership',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

