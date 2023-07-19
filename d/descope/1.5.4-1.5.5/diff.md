# Comparing `tmp/descope-1.5.4.tar.gz` & `tmp/descope-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.5.4.tar", max compression
+gzip compressed data, was "descope-1.5.5.tar", max compression
```

## Comparing `descope-1.5.4.tar` & `descope-1.5.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1064 2023-07-05 14:52:31.310171 descope-1.5.4/LICENSE
--rw-r--r--   0        0        0    32364 2023-07-05 14:52:31.310171 descope-1.5.4/README.md
--rw-r--r--   0        0        0      560 2023-07-05 14:52:31.310171 descope-1.5.4/descope/__init__.py
--rw-r--r--   0        0        0      211 2023-07-05 14:52:31.310171 descope-1.5.4/descope/_auth_base.py
--rw-r--r--   0        0        0    21253 2023-07-05 14:52:31.310171 descope-1.5.4/descope/auth.py
--rw-r--r--   0        0        0        0 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     5352 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     6211 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1528 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    11078 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8150 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/password.py
--rw-r--r--   0        0        0     1481 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/saml.py
--rw-r--r--   0        0        0     5128 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6705 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     4266 2023-07-05 14:52:31.310171 descope-1.5.4/descope/common.py
--rw-r--r--   0        0        0    12089 2023-07-05 14:52:31.310171 descope-1.5.4/descope/descope_client.py
--rw-r--r--   0        0        0     1420 2023-07-05 14:52:31.310171 descope-1.5.4/descope/exceptions.py
--rw-r--r--   0        0        0     5809 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/access_key.py
--rw-r--r--   0        0        0     4604 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/audit.py
--rw-r--r--   0        0        0     4155 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/common.py
--rw-r--r--   0        0        0     3904 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/flow.py
--rw-r--r--   0        0        0     3971 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/group.py
--rw-r--r--   0        0        0      959 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/jwt.py
--rw-r--r--   0        0        0     2535 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/permission.py
--rw-r--r--   0        0        0     3098 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/role.py
--rw-r--r--   0        0        0     6386 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/sso_settings.py
--rw-r--r--   0        0        0     3689 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/tenant.py
--rw-r--r--   0        0        0    31376 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/user.py
--rw-r--r--   0        0        0     1710 2023-07-05 14:52:31.310171 descope-1.5.4/descope/mgmt.py
--rw-r--r--   0        0        0     1220 2023-07-05 14:52:59.885985 descope-1.5.4/pyproject.toml
--rw-r--r--   0        0        0    33384 1970-01-01 00:00:00.000000 descope-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-19 14:59:58.737064 descope-1.5.5/LICENSE
+-rw-r--r--   0        0        0    32623 2023-07-19 14:59:58.737064 descope-1.5.5/README.md
+-rw-r--r--   0        0        0      560 2023-07-19 14:59:58.737064 descope-1.5.5/descope/__init__.py
+-rw-r--r--   0        0        0      211 2023-07-19 14:59:58.737064 descope-1.5.5/descope/_auth_base.py
+-rw-r--r--   0        0        0    21253 2023-07-19 14:59:58.741064 descope-1.5.5/descope/auth.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     5352 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     6211 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1528 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    11078 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8150 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1481 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     5128 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6705 2023-07-19 14:59:58.741064 descope-1.5.5/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     4266 2023-07-19 14:59:58.741064 descope-1.5.5/descope/common.py
+-rw-r--r--   0        0        0    12089 2023-07-19 14:59:58.741064 descope-1.5.5/descope/descope_client.py
+-rw-r--r--   0        0        0     1420 2023-07-19 14:59:58.741064 descope-1.5.5/descope/exceptions.py
+-rw-r--r--   0        0        0     5809 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/access_key.py
+-rw-r--r--   0        0        0     4604 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/audit.py
+-rw-r--r--   0        0        0     4196 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/common.py
+-rw-r--r--   0        0        0     3904 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/flow.py
+-rw-r--r--   0        0        0     3971 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/group.py
+-rw-r--r--   0        0        0      959 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/jwt.py
+-rw-r--r--   0        0        0     2535 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/permission.py
+-rw-r--r--   0        0        0     3098 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/role.py
+-rw-r--r--   0        0        0     6860 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     4316 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/tenant.py
+-rw-r--r--   0        0        0    31376 2023-07-19 14:59:58.741064 descope-1.5.5/descope/management/user.py
+-rw-r--r--   0        0        0     1710 2023-07-19 14:59:58.741064 descope-1.5.5/descope/mgmt.py
+-rw-r--r--   0        0        0     1220 2023-07-19 15:00:35.370149 descope-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0    33643 1970-01-01 00:00:00.000000 descope-1.5.5/PKG-INFO
```

### Comparing `descope-1.5.4/LICENSE` & `descope-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/README.md` & `descope-1.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,17 @@
     name="My First Tenant",
     self_provisioning_domains=["domain.com", "another-domain.com"],
 )
 
 # Tenant deletion cannot be undone. Use carefully.
 descope_client.mgmt.tenant.delete("my-custom-id")
 
+# Load tenant by id
+tenant_resp = descope_client.mgmt.tenant.load("my-custom-id")
+
 # Load all tenants
 tenants_resp = descope_client.mgmt.tenant.load_all()
 tenants = tenants_resp["tenants"]
     for tenant in tenants:
         # Do something
 ```
 
@@ -625,14 +628,16 @@
     domain="tenant-users.com" # Users authentication with this domain will be logged in to this tenant
 )
 
 # Alternatively, configure using an SSO metadata URL
 descope_client.mgmt.sso.configure_via_metadata(
     tenant_id, # Which tenant this configuration is for
     idp_metadata_url="https://idp.com/my-idp-metadata",
+    redirect_url="", # Redirect URL will have to be provided in every authentication call
+    domain="" # Remove the current domain configuration if a value was previously set
 )
 
 # Map IDP groups to Descope roles, or map user attributes.
 # This function overrides any previous mapping (even when empty). Use carefully.
 descope_client.mgmt.sso.mapping(
     tenant_id, # Which tenant this mapping is for
     role_mappings = [RoleMapping(["IDP_ADMIN"], "Tenant Admin")],
```

### Comparing `descope-1.5.4/descope/__init__.py` & `descope-1.5.5/descope/__init__.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/auth.py` & `descope-1.5.5/descope/auth.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/enchantedlink.py` & `descope-1.5.5/descope/authmethod/enchantedlink.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/magiclink.py` & `descope-1.5.5/descope/authmethod/magiclink.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/oauth.py` & `descope-1.5.5/descope/authmethod/oauth.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/otp.py` & `descope-1.5.5/descope/authmethod/otp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/password.py` & `descope-1.5.5/descope/authmethod/password.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/saml.py` & `descope-1.5.5/descope/authmethod/saml.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/totp.py` & `descope-1.5.5/descope/authmethod/totp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/authmethod/webauthn.py` & `descope-1.5.5/descope/authmethod/webauthn.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/common.py` & `descope-1.5.5/descope/common.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/descope_client.py` & `descope-1.5.5/descope/descope_client.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/exceptions.py` & `descope-1.5.5/descope/exceptions.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/access_key.py` & `descope-1.5.5/descope/management/access_key.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/audit.py` & `descope-1.5.5/descope/management/audit.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/common.py` & `descope-1.5.5/descope/management/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class MgmtV1:
     # tenant
     tenant_create_path = "/v1/mgmt/tenant/create"
     tenant_update_path = "/v1/mgmt/tenant/update"
     tenant_delete_path = "/v1/mgmt/tenant/delete"
+    tenant_load_path = "/v1/mgmt/tenant"
     tenant_load_all_path = "/v1/mgmt/tenant/all"
 
     # user
     user_create_path = "/v1/mgmt/user/create"
     user_update_path = "/v1/mgmt/user/update"
     user_delete_path = "/v1/mgmt/user/delete"
     user_delete_all_test_users_path = "/v1/mgmt/user/test/delete/all"
```

### Comparing `descope-1.5.4/descope/management/flow.py` & `descope-1.5.5/descope/management/flow.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/group.py` & `descope-1.5.5/descope/management/group.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/jwt.py` & `descope-1.5.5/descope/management/jwt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/permission.py` & `descope-1.5.5/descope/management/permission.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/role.py` & `descope-1.5.5/descope/management/role.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/management/sso_settings.py` & `descope-1.5.5/descope/management/sso_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,27 +73,27 @@
 
     def configure(
         self,
         tenant_id: str,
         idp_url: str,
         entity_id: str,
         idp_cert: str,
-        redirect_url: str = None,
-        domain: str = None,
+        redirect_url: str,
+        domain: str,
     ) -> None:
         """
         Configure SSO setting for a tenant manually. Alternatively, `configure_via_metadata` can be used instead.
 
         Args:
         tenant_id (str): The tenant ID to be configured
         idp_url (str): The URL for the identity provider.
         entity_id (str): The entity ID (in the IDP).
         idp_cert (str): The certificate provided by the IDP.
-        redirect_url (str): An Optional Redirect URL after successful authentication.
-        domain (str): An optional domain used to associate users authenticating via SSO with this tenant
+        redirect_url (str): The Redirect URL to use after successful authentication, or empty string to reset it.
+        domain (str): domain used to associate users authenticating via SSO with this tenant, or empty string to reset it.
 
         Raise:
         AuthException: raised if configuration operation fails
         """
         self._auth.do_post(
             MgmtV1.sso_settings_path,
             SSOSettings._compose_configure_body(
@@ -102,28 +102,34 @@
             pswd=self._auth.management_key,
         )
 
     def configure_via_metadata(
         self,
         tenant_id: str,
         idp_metadata_url: str,
+        redirect_url: str,
+        domain: str,
     ):
         """
         Configure SSO setting for am IDP metadata URL. Alternatively, `configure` can be used instead.
 
         Args:
         tenant_id (str): The tenant ID to be configured
         idp_metadata_url (str): The URL to fetch SSO settings from.
+        redirect_url (str): The Redirect URL to use after successful authentication, or empty string to reset it.
+        domain (str): domain used to associate users authenticating via SSO with this tenant, or empty string to reset it.
 
         Raise:
         AuthException: raised if configuration operation fails
         """
         self._auth.do_post(
             MgmtV1.sso_metadata_path,
-            SSOSettings._compose_metadata_body(tenant_id, idp_metadata_url),
+            SSOSettings._compose_metadata_body(
+                tenant_id, idp_metadata_url, redirect_url, domain
+            ),
             pswd=self._auth.management_key,
         )
 
     def mapping(
         self,
         tenant_id: str,
         role_mappings: List[RoleMapping] = None,
@@ -153,34 +159,38 @@
 
     @staticmethod
     def _compose_configure_body(
         tenant_id: str,
         idp_url: str,
         entity_id: str,
         idp_cert: str,
-        redirect_url: str = None,
-        domain: str = None,
+        redirect_url: str,
+        domain: str,
     ) -> dict:
         return {
             "tenantId": tenant_id,
             "idpURL": idp_url,
             "entityId": entity_id,
             "idpCert": idp_cert,
             "redirectURL": redirect_url,
             "domain": domain,
         }
 
     @staticmethod
     def _compose_metadata_body(
         tenant_id: str,
         idp_metadata_url: str,
+        redirect_url: str,
+        domain: str,
     ) -> dict:
         return {
             "tenantId": tenant_id,
             "idpMetadataURL": idp_metadata_url,
+            "redirectURL": redirect_url,
+            "domain": domain,
         }
 
     @staticmethod
     def _compose_mapping_body(
         tenant_id: str,
         role_mapping: List[RoleMapping],
         attribute_mapping: AttributeMapping,
```

### Comparing `descope-1.5.4/descope/management/tenant.py` & `descope-1.5.5/descope/management/tenant.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,14 +82,39 @@
 
         Raise:
         AuthException: raised if creation operation fails
         """
         uri = MgmtV1.tenant_delete_path
         self._auth.do_post(uri, {"id": id}, pswd=self._auth.management_key)
 
+    def load(
+        self,
+        id: str,
+    ) -> dict:
+        """
+        Load tenant by id.
+
+        Args:
+        id (str): The ID of the tenant to load.
+
+        Return value (dict):
+        Return dict in the format
+             {"id": <id>, "name": <name>, "selfProvisioningDomains": []}
+        Containing the loaded tenant information.
+
+        Raise:
+        AuthException: raised if load operation fails
+        """
+        response = self._auth.do_get(
+            uri=MgmtV1.tenant_load_path,
+            params={"id": id},
+            pswd=self._auth.management_key,
+        )
+        return response.json()
+
     def load_all(
         self,
     ) -> dict:
         """
         Load all tenants.
 
         Return value (dict):
```

### Comparing `descope-1.5.4/descope/management/user.py` & `descope-1.5.5/descope/management/user.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/descope/mgmt.py` & `descope-1.5.5/descope/mgmt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.4/pyproject.toml` & `descope-1.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.5.4"
+version = "1.5.5"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
@@ -32,15 +32,15 @@
 [tool.poetry.group.dev.dependencies]
 mock = "5.0.2"
 pre-commit = "2.21.0"
 Flask = "2.2.5"
 flake8 = "5.0.4"
 flake8-bugbear = "22.12.6"
 pytest-cov = "4.1.0"
-pytest = "7.3.2"
+pytest = "7.4.0"
 black = "23.3.0"
 liccheck = "0.9.1"
 isort = "5.11.4"
 pep8-naming = "0.13.3"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
```

### Comparing `descope-1.5.4/PKG-INFO` & `descope-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.5.4
+Version: 1.5.5
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -490,14 +490,17 @@
     name="My First Tenant",
     self_provisioning_domains=["domain.com", "another-domain.com"],
 )
 
 # Tenant deletion cannot be undone. Use carefully.
 descope_client.mgmt.tenant.delete("my-custom-id")
 
+# Load tenant by id
+tenant_resp = descope_client.mgmt.tenant.load("my-custom-id")
+
 # Load all tenants
 tenants_resp = descope_client.mgmt.tenant.load_all()
 tenants = tenants_resp["tenants"]
     for tenant in tenants:
         # Do something
 ```
 
@@ -651,14 +654,16 @@
     domain="tenant-users.com" # Users authentication with this domain will be logged in to this tenant
 )
 
 # Alternatively, configure using an SSO metadata URL
 descope_client.mgmt.sso.configure_via_metadata(
     tenant_id, # Which tenant this configuration is for
     idp_metadata_url="https://idp.com/my-idp-metadata",
+    redirect_url="", # Redirect URL will have to be provided in every authentication call
+    domain="" # Remove the current domain configuration if a value was previously set
 )
 
 # Map IDP groups to Descope roles, or map user attributes.
 # This function overrides any previous mapping (even when empty). Use carefully.
 descope_client.mgmt.sso.mapping(
     tenant_id, # Which tenant this mapping is for
     role_mappings = [RoleMapping(["IDP_ADMIN"], "Tenant Admin")],
```

