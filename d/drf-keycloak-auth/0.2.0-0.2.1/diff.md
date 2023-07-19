# Comparing `tmp/drf_keycloak_auth-0.2.0.tar.gz` & `tmp/drf_keycloak_auth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_keycloak_auth-0.2.0.tar", last modified: Mon Jul  3 02:22:52 2023, max compression
+gzip compressed data, was "drf_keycloak_auth-0.2.1.tar", last modified: Wed Jul 19 11:43:59 2023, max compression
```

## Comparing `drf_keycloak_auth-0.2.0.tar` & `drf_keycloak_auth-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:22:52.452438 drf_keycloak_auth-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5347 2023-07-03 02:22:52.452438 drf_keycloak_auth-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:22:52.450438 drf_keycloak_auth-0.2.0/drf_keycloak_auth/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    10919 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2638 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/keycloak.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:22:52.451438 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5347 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 02:22:52.000000 drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:22:52.452438 drf_keycloak_auth-0.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1142 2023-07-03 02:22:48.000000 drf_keycloak_auth-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 11:43:59.018394 drf_keycloak_auth-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5347 2023-07-19 11:43:59.017394 drf_keycloak_auth-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 11:43:59.016394 drf_keycloak_auth-0.2.1/drf_keycloak_auth/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    11993 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/keycloak.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 11:43:59.017394 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5347 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 11:43:59.018394 drf_keycloak_auth-0.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1142 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/setup.py
```

### Comparing `drf_keycloak_auth-0.2.0/LICENSE` & `drf_keycloak_auth-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.2.0/PKG-INFO` & `drf_keycloak_auth-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_keycloak_auth
-Version: 0.2.0
+Version: 0.2.1
 Summary: A convenience libary for authenticating users from Keycloak access tokens
 Home-page: https://gitlab.com/ecocommons-australia/lib/drf-keycloak-auth
 Author: EcoCommons Australia
 Author-email: ecocommons@griffith.edu.au
 License: MIT
 Keywords: drf,django,rest_framework,djangorestframework,authentication,python3,keycloak
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drf_keycloak_auth-0.2.0/README.md` & `drf_keycloak_auth-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.2.0/drf_keycloak_auth/authentication.py` & `drf_keycloak_auth-0.2.1/drf_keycloak_auth/authentication.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ add a keycloak authentication class specific to Django Rest Framework """
 from typing import Tuple, Dict, List
 import logging
+import re
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.contrib.auth.models import AnonymousUser, update_last_login, Group
 from django.contrib.auth import get_user_model
 from rest_framework import (
     authentication,
     exceptions,
@@ -89,26 +90,52 @@
         """ raises if not active """
         is_active = decoded_token.get('active', False)
         if not is_active:
             raise AuthenticationFailed(
                 'invalid or expired token'
             )
 
+    def _add_realm_prefix(self, value: str) -> str:
+        """ Add 'REALM_NAME:' prefix to a string value.
+            This only works if KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME is True.
+            
+            Checks to ensure the prefix is not already added.
+            :param value: The string to prefix
+            :returns: Prefixed string
+        """
+        if not api_settings.KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME:
+            return value
+
+        if not self.keycloak_openid.realm_name:
+            log.warning(f"Cannot add realm prefix. Realm missing!")
+            return value
+
+        prefix = str(self.keycloak_openid.realm_name)+':'
+        if re.search('^'+prefix, value):
+            log.debug(f"Value '{str(value)}' already has realm prefix")
+            return value
+
+        return prefix+str(value)
+
     def _map_keycloak_to_django_fields(self, decoded_token: dict) -> dict:
+        """ Map Keycloak access_token fields to Django User attributes """
         django_fields = {}
-        keycloak_username_field = \
+        kc_username_field = \
             api_settings.KEYCLOAK_FIELD_AS_DJANGO_USERNAME
 
         if (
-            keycloak_username_field
+            kc_username_field
             and
-            isinstance(keycloak_username_field, str)
+            isinstance(kc_username_field, str)
         ):
             django_fields['username'] = \
-                decoded_token.get(keycloak_username_field, '')
+                self._add_realm_prefix(decoded_token.get(kc_username_field, ''))
+
+        # ecocommons_user.CustomUser field
+        django_fields['realm'] = str(self.keycloak_openid.realm_name)
 
         django_fields['email'] = decoded_token.get('email', '')
 
         # django stores first_name and last_name as empty strings
         # by default, not None
         django_fields['first_name'] = \
             decoded_token.get('given_name', '')
@@ -144,21 +171,23 @@
         sub = decoded_token['sub']
         django_fields = self._map_keycloak_to_django_fields(decoded_token)
 
         user = None
         try:
             user = User.objects.get(**{django_uuid_field: sub})
             user = self._update_user(user, django_fields)
+
         except ObjectDoesNotExist:
             log.warning(
                 'KeycloakAuthentication._handle_local_user | '
-                f'ObjectDoesNotExist: {sub} does not exist'
+                f'ObjectDoesNotExist: {sub} does not exist - creating'
             )
 
         if user is None:
+            # Add uuid field and create
             django_fields.update(**{django_uuid_field: sub})
             user = User.objects.create_user(**django_fields)
 
         update_last_login(sender=None, user=user)
         return user
 
     def _get_roles(
@@ -307,9 +336,8 @@
 
         except Exception as e:
             log.error(
                 'KeycloakMultiAuthentication.authenticate | '
                 f'Exception: {e})'
             )
 
-
         return credentials
```

### Comparing `drf_keycloak_auth-0.2.0/drf_keycloak_auth/keycloak.py` & `drf_keycloak_auth-0.2.1/drf_keycloak_auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.2.0/drf_keycloak_auth/permissions.py` & `drf_keycloak_auth-0.2.1/drf_keycloak_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.2.0/drf_keycloak_auth/settings.py` & `drf_keycloak_auth-0.2.1/drf_keycloak_auth/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,30 +15,44 @@
 
 DEFAULTS = {
     'KEYCLOAK_MULTI_OIDC_JSON': (
         json.loads(os.getenv('KEYCLOAK_MULTI_OIDC_JSON'))
         if os.getenv('KEYCLOAK_MULTI_OIDC_JSON')
         else None
     ),
+    
     'KEYCLOAK_SERVER_URL': os.getenv('KEYCLOAK_SERVER_URL'),
+
     'KEYCLOAK_REALM': os.getenv('KEYCLOAK_REALM'),
+
     'KEYCLOAK_CLIENT_ID': os.getenv('KEYCLOAK_CLIENT_ID'),
+
     'KEYCLOAK_CLIENT_SECRET_KEY': os.getenv('KEYCLOAK_CLIENT_SECRET_KEY'),
+
     'KEYCLOAK_AUTH_HEADER_PREFIX':
         os.getenv('KEYCLOAK_AUTH_HEADER_PREFIX', 'Bearer'),
+
     'KEYCLOAK_ROLE_SET_PREFIX':
         os.getenv('KEYCLOAK_ROLE_SET_PREFIX', 'role:'),
+
     'KEYCLOAK_MANAGE_LOCAL_USER':
         os.getenv('KEYCLOAK_MANAGE_LOCAL_USER', True),
+
     'KEYCLOAK_MANAGE_LOCAL_GROUPS':
         os.getenv('KEYCLOAK_MANAGE_LOCAL_GROUPS', False),
+
     'KEYCLOAK_DJANGO_USER_UUID_FIELD':
         os.getenv('KEYCLOAK_DJANGO_USER_UUID_FIELD', 'pk'),
+
     'KEYCLOAK_FIELD_AS_DJANGO_USERNAME':
         os.getenv('KEYCLOAK_FIELD_AS_DJANGO_USERNAME', 'preferred_username'),
+
+    'KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME':
+        os.getenv('KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME', True),
+
     'KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF': (
         [x.strip() for x in KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF.split(',')]
         if KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF
         else ['admin']  # can be list, tuple or set
     )
 }
```

### Comparing `drf_keycloak_auth-0.2.0/drf_keycloak_auth.egg-info/PKG-INFO` & `drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-keycloak-auth
-Version: 0.2.0
+Version: 0.2.1
 Summary: A convenience libary for authenticating users from Keycloak access tokens
 Home-page: https://gitlab.com/ecocommons-australia/lib/drf-keycloak-auth
 Author: EcoCommons Australia
 Author-email: ecocommons@griffith.edu.au
 License: MIT
 Keywords: drf,django,rest_framework,djangorestframework,authentication,python3,keycloak
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drf_keycloak_auth-0.2.0/setup.py` & `drf_keycloak_auth-0.2.1/setup.py`

 * *Files identical despite different names*

