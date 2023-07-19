# Comparing `tmp/ckanext-passwordless-api-1.1.0.tar.gz` & `tmp/ckanext-passwordless-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-passwordless-api-1.1.0.tar", last modified: Tue May 30 17:45:10 2023, max compression
+gzip compressed data, was "ckanext-passwordless-api-1.1.1.tar", last modified: Wed Jul 19 14:24:55 2023, max compression
```

## Comparing `ckanext-passwordless-api-1.1.0.tar` & `ckanext-passwordless-api-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1416 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1060 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/LICENSE
--rw-r--r--   0        0        0     7054 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/README.md
--rw-r--r--   0        0        0      230 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.1.0/ckanext/__init__.py
--rw-r--r--   0        0        0      235 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/__init__.py
--rw-r--r--   0        0        0       43 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/__version__.py
--rw-r--r--   0        0        0    13137 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/logic.py
--rw-r--r--   0        0        0     2403 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/mailer.py
--rw-r--r--   0        0        0     4268 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/plugin.py
--rw-r--r--   0        0        0      488 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/templates/reset_key.txt
--rw-r--r--   0        0        0     1014 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/templates/welcome_user.txt
--rw-r--r--   0        0        0       49 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/tests/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-03 18:09:43.437296 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/tests/test_plugin.py
--rw-r--r--   0        0        0     7658 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/util.py
--rw-r--r--   0        0        0     2203 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     7900 1970-01-01 00:00:00.000000 ckanext-passwordless-api-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-07-19 14:24:32.944273 ckanext-passwordless-api-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1060 2023-05-30 17:44:55.718905 ckanext-passwordless-api-1.1.1/LICENSE
+-rw-r--r--   0        0        0     7054 2023-05-30 17:44:55.718905 ckanext-passwordless-api-1.1.1/README.md
+-rw-r--r--   0        0        0      230 2023-02-27 14:50:27.292968 ckanext-passwordless-api-1.1.1/ckanext/__init__.py
+-rw-r--r--   0        0        0      235 2023-02-27 14:50:27.292968 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-19 14:24:32.944273 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/__version__.py
+-rw-r--r--   0        0        0    13384 2023-07-19 14:24:32.944273 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/logic.py
+-rw-r--r--   0        0        0     2468 2023-07-19 14:24:32.944273 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/mailer.py
+-rw-r--r--   0        0        0     4407 2023-07-19 14:24:32.944273 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/plugin.py
+-rw-r--r--   0        0        0      488 2023-02-27 14:50:27.292968 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/templates/reset_key.txt
+-rw-r--r--   0        0        0     1014 2023-02-27 14:50:27.292968 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/templates/welcome_user.txt
+-rw-r--r--   0        0        0       49 2023-02-27 14:50:27.292968 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/tests/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-03 18:09:47.057341 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/tests/test_plugin.py
+-rw-r--r--   0        0        0     7658 2023-05-30 17:44:55.718905 ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/util.py
+-rw-r--r--   0        0        0     2203 2023-07-19 14:24:32.944273 ckanext-passwordless-api-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7900 1970-01-01 00:00:00.000000 ckanext-passwordless-api-1.1.1/PKG-INFO
```

### Comparing `ckanext-passwordless-api-1.1.0/CHANGELOG.md` & `ckanext-passwordless-api-1.1.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 1.1.1 (2023-07-19)
+
+### Fix
+
+- welcome email logic
+- response error handling
+
 ## 1.1.0 (2023-05-30)
 
 ### Feat
 
 - add option to anonymise usernames
 - add introspect endpoint, verify token only
```

### Comparing `ckanext-passwordless-api-1.1.0/LICENSE` & `ckanext-passwordless-api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.1.0/README.md` & `ckanext-passwordless-api-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/logic.py` & `ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,18 @@
 
     # get existing user from email
     user = util.get_user_from_email(email)
     # log.debug(f'USER is {str(user)})
 
     if not user:
         # A user with this email address doesn't yet exist in CKAN, so create one.
-        user = _create_user(email)
+        new_user_email = _create_user(email)
         log.debug(f"Created user {str(email)}")
+        user = util.get_user_from_email(new_user_email)
+        send_welcome_email(user)
 
     if user:
         # make sure is not deleted
         if user.state == "deleted":
             raise toolkit.ValidationError(
                 {"user": f"User with email {email} was deleted already. Contact Admin."}
             )
@@ -82,40 +84,46 @@
             {"user": "cannot retrieve or create user with given email"}
         )
 
     return {"message": "success"}
 
 
 def _create_user(email):
-    """Create a new user and send welcome email."""
+    """Create a new user and send welcome email.
+
+    Returns the user email.
+    """
     # first check temporary quota
     util.check_new_user_quota()
 
     try:
         data_dict = {
             "email": email.lower(),
             "fullname": util.generate_user_fullname(email),
             "name": util.get_new_username(email),
             "password": util.generate_password(),
         }
-        user = toolkit.get_action("user_create")(
+        user_dict = toolkit.get_action("user_create")(
             context={"ignore_auth": True}, data_dict=data_dict
         )
-        send_welcome_email(user)
     except SQLAlchemyError as error:
         exception_message = f"{error}"
         log.error(f"Failed to create user: {error}")
         if exception_message.find("quota") >= 0:
             raise DataError from error(
                 "Error creating a new user, daily new user quota exceeded"
             )
         else:
             raise DataError from error("Internal error creating a new user")
+    except Exception as e:
+        log.error(e)
+        log.error("Error creating new user")
+        raise Exception from e
 
-    return user
+    return user_dict.get("email")
 
 
 def request_api_token(
     context,  #: Context,
     data_dict,  #: DataDict,
 ):
     """Get API token for a user, if reset key valid.
```

### Comparing `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/mailer.py` & `ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/mailer.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 
 def send_user_reset_key(user):
     """Send the login token email."""
     mailer.create_reset_key(user)
     if reset_key := user.reset_key:
         # Strip b'' wrapping
         reset_key = reset_key[2:-1]
-    # log.debug("passwordless_send_reset_link user = " + str(user))
     body = _get_user_reset_key_body(user.as_dict(), reset_key)
     subject = f"Access token: {reset_key}"
+    log.debug(f"Sending user reset key to user: {str(user.email)}")
     mailer.mail_user(user, subject, body)
 
 
 def _get_user_reset_key_body(user: dict, reset_key):
     """Render the login token email."""
+    log.debug("Building user reset token email from template")
+
     if display_name := user.get("fullname"):
         pass
     elif display_name := user.get("name"):
         pass
     else:
         display_name = user.get("email")
     extra_vars = {
@@ -42,24 +44,23 @@
     )
     return render(reset_key_template, extra_vars)
 
 
 def send_welcome_email(user):
     """Send the welcome email."""
     body = _get_welcome_email_body(user.as_dict())
-    subject = "Welcome to {}".format(config.get("ckan.site_title"))
-
-    # log.debug(
-    #     f"passwordless_mailer: Welcome email subject: '{subject}',  body: \n {body}"
-    # )
+    subject = f"Welcome to {config.get('ckan.site_title')}"
+    log.debug(f"Sending welcome email to user: {str(user.email)}")
     mailer.mail_user(user, subject, body)
 
 
 def _get_welcome_email_body(user: dict):
     """Render the welcome email."""
+    log.debug("Building welcome email from template")
+
     extra_vars = {
         "site_title": config.get("ckan.site_title"),
         "site_url": config.get("ckan.site_url"),
         "guidelines_url": config.get("passwordless_api.guidelines_url", None),
         "policies_url": config.get("passwordless_api.policies_url", None),
         "site_org": config.get("ckan.site_org", "our organization"),
         "email_to": config.get("email_to"),
```

### Comparing `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/plugin.py` & `ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,15 +83,17 @@
                 return response
 
             try:
                 # token present in both renew_api_token and get_user
                 if not (token := load_json(response.data).get("result").get("token")):
                     return response
             except Exception as e:
-                return e
+                # Required to bypass errors and continue loading
+                log.warning(f"passwordless token load error: {e}")
+                return response
 
             log.debug(
                 "Adding cookie to response with vars: "
                 f"key={self.cookie_name} | value={token} | "
                 f"max_age={self.cookie_expiry} | domain={self.cookie_domain} | "
                 f"secure={self.cookie_secure} | httponly={self.cookie_http_only} | "
                 f"samesite={self.cookie_samesite}"
```

### Comparing `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/templates/welcome_user.txt` & `ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/templates/welcome_user.txt`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/tests/test_plugin.py` & `ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/util.py` & `ckanext-passwordless-api-1.1.1/ckanext/passwordless_api/util.py`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.1.0/pyproject.toml` & `ckanext-passwordless-api-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-version = "1.1.0"
+version = "1.1.1"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."ckan.plugins"]
 passwordless_api = "ckanext.passwordless_api.plugin:PasswordlessAPIPlugin"
 
@@ -61,15 +61,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest-ckan>=0.0.12",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.0"
+version = "1.1.1"
 version_files = [
     "pyproject.toml:version",
     "ckanext/passwordless_api/__version__.py",
     "docs/openapi.yaml:version",
 ]
 
 [tool.isort]
```

### Comparing `ckanext-passwordless-api-1.1.0/PKG-INFO` & `ckanext-passwordless-api-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-passwordless_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extension to allow paswordless login to the CKAN API
 License: MIT
 Keywords: CKAN,passwordless,token,auth
 Author-email: Sam Woodcock <sam.woodcock@protonmail.com>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ckanext-passwordless_api Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: ckanext-passwordless_api Version: 1.1.1 Summary:
 Extension to allow paswordless login to the CKAN API License: MIT Keywords:
 CKAN,passwordless,token,auth Author-email: Sam Woodcock
 woodcock@protonmail.com> Requires-Python: >=3.8 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```

