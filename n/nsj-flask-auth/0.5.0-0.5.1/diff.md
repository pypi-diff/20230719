# Comparing `tmp/nsj_flask_auth-0.5.0.tar.gz` & `tmp/nsj_flask_auth-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_flask_auth-0.5.0.tar", max compression
+gzip compressed data, was "nsj_flask_auth-0.5.1.tar", max compression
```

## Comparing `nsj_flask_auth-0.5.0.tar` & `nsj_flask_auth-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       72 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/__init__.py
--rw-r--r--   0        0        0    16982 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/auth.py
--rw-r--r--   0        0        0      430 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/caching.py
--rw-r--r--   0        0        0      135 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/exceptions.py
--rw-r--r--   0        0        0      601 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/settings.py
--rw-r--r--   0        0        0      521 2023-07-03 15:18:25.925167 nsj_flask_auth-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 nsj_flask_auth-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.1/nsj_flask_auth/__init__.py
+-rw-r--r--   0        0        0    18395 2023-07-19 12:10:48.179702 nsj_flask_auth-0.5.1/nsj_flask_auth/auth.py
+-rw-r--r--   0        0        0      430 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.1/nsj_flask_auth/caching.py
+-rw-r--r--   0        0        0      184 2023-07-19 12:06:37.612886 nsj_flask_auth-0.5.1/nsj_flask_auth/exceptions.py
+-rw-r--r--   0        0        0      601 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.1/nsj_flask_auth/settings.py
+-rw-r--r--   0        0        0      521 2023-07-19 12:11:39.031425 nsj_flask_auth-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 nsj_flask_auth-0.5.1/PKG-INFO
```

### Comparing `nsj_flask_auth-0.5.0/nsj_flask_auth/auth.py` & `nsj_flask_auth-0.5.1/nsj_flask_auth/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import os
 import logging
 import requests
 
 from typing import List
 from enum import Enum
 from functools import wraps
 from urllib.parse import urljoin
 
 from flask import request, abort, jsonify, g
 
 from nsj_flask_auth.caching import Caching
-from nsj_flask_auth.exceptions import Forbidden, MissingAuthorizationHeader, Unauthorized
+from nsj_flask_auth.exceptions import Forbidden, MissingAuthorizationHeader, Unauthorized, InternalUnauthorized
 from nsj_flask_auth.settings import log_time
 
 
 class Scope(Enum):
     TENANT = 0
     GRUPO_EMPRESARIAL = 1
     EMPRESA = 2
@@ -68,15 +69,19 @@
         self._access_token_header = access_token_header
         self._user_internal_permissions = user_internal_permissions
         self._scope: Scope = scope
         self._user_scope_permissions = user_scope_permissions
         self._app_required_permissions = app_required_permissions
         if caching_service:
             self._cache = Caching(caching_service)
-        self._logger = logging.getLogger(app_name)
+        
+        if "APP_NAME" in os.environ:
+            self._logger = logging.getLogger(os.environ["APP_NAME"])
+        else:
+            self._logger = logging.getLogger(app_name)
 
     def _verify_api_key(self, app_required_permissions: List = None):
         api_key = request.headers.get(self._api_key_header)
 
         if not api_key:
             raise MissingAuthorizationHeader(
                 f"Missing {self._api_key_header} header")
@@ -153,26 +158,30 @@
             user_profile = self._cache.get(email)
 
         if not user_profile:
             url = self._diretorio_base_uri + "/profile/" + email
             headers = {"apikey": self._diretorio_api_key}
             response = requests.get(url, headers=headers)
 
-            if response.status_code != 200:
-                raise Exception("A api-key do sistema não é válida")
+            if response.status_code == 401 or response.status_code == 403:
+                raise InternalUnauthorized("A api-key do sistema não é válida")
+            elif response.status_code != 200:
+                raise Exception(f"Erro desconhecido na recuperação do profile: {response.status_code}. Mensagem: {response.content.decode()}")
         if user_profile:
             return user_profile
 
         url = urljoin(self._diretorio_base_uri, f"/v2/api/profile/{email}")
         headers = {"apikey": self._diretorio_api_key}
 
         response = requests.get(url, headers=headers)
 
-        if response.status_code != 200:
-            raise Exception("A api-key do sistema não é válida")
+        if response.status_code == 401 or response.status_code == 403:
+            raise InternalUnauthorized("A api-key do sistema não é válida")
+        elif response.status_code != 200:
+            raise Exception(f"Erro desconhecido na recuperação do profile: {response.status_code}. Mensagem: {response.content.decode()}")
 
         user_profile = response.json()
 
         if self._cache:
             self._cache.set(email, user_profile)
 
         return user_profile
@@ -316,16 +325,18 @@
             "Content-Type": "application/x-www-form-urlencoded",
         }
 
         url = urljoin(self._diretorio_base_uri, "v2/api/validate")
 
         response = requests.post(url, data=data, headers=headers)
 
-        if response.status_code != 200:
-            raise Unauthorized("A api-key do sistema não é válida")
+        if response.status_code == 401 or response.status_code == 403:
+            raise InternalUnauthorized("A api-key do sistema não é válida")
+        elif response.status_code != 200:
+            raise Exception(f"Erro desconhecido na validação do profile: {response.status_code}. Mensagem: {response.content.decode()}")
 
         if self._cache:
             self._cache.set(api_key, response.json())
 
         return response.json()
 
     @log_time('Pegar permissões por funções')
@@ -341,16 +352,18 @@
         if not permissions:
             url = urljoin(
                 self._diretorio_base_uri, f"v2/api/funcoes/{function_id}/permissoes"
             )
             headers = {"apikey": self._diretorio_api_key}
             response = requests.get(url, headers=headers)
 
-            if response.status_code != 200:
-                raise Unauthorized("A api-key do sistema não é válida")
+            if response.status_code == 401 or response.status_code == 403:
+                raise InternalUnauthorized("A api-key do sistema não é válida")
+            elif response.status_code != 200:
+                raise Exception(f"Erro desconhecido na recuperação das permissões do profile: {response.status_code}. Mensagem: {response.content.decode()}")
 
             permissions = response.json()
 
             if self._cache:
                 self._cache.set(function_id, permissions)
 
         return permissions
@@ -385,14 +398,16 @@
                     return func(*args, **kwargs)
                 except Forbidden as e:
                     return self._format_erro(403, f"{e}")
                 except MissingAuthorizationHeader as e:
                     return self._format_erro(401, f"{e}")
                 except Unauthorized as e:
                     return self._format_erro(401, f"{e}")
+                except InternalUnauthorized as e:
+                    return self._format_erro(500, f"{e}")
                 except Exception as e:
                     self._logger.exception(
                         f"Erro na autenticação/autorização. Mensagem: {e}")
                     return self._format_erro(500, f"{e}")
 
             return wrapper
 
@@ -423,14 +438,16 @@
                     return func(*args, **kwargs)
                 except Forbidden as e:
                     return self._format_erro(403, f"{e}")
                 except MissingAuthorizationHeader as e:
                     return self._format_erro(401, f"{e}")
                 except Unauthorized as e:
                     return self._format_erro(401, f"{e}")
+                except InternalUnauthorized as e:
+                    return self._format_erro(500, f"{e}")
                 except Exception as e:
                     self._logger.exception(
                         f"Erro na autenticação/autorização. Mensagem: {e}")
                     return self._format_erro(500, f"{e}")
 
             return wrapper
 
@@ -461,14 +478,16 @@
                     return func(*args, **kwargs)
                 except Forbidden as e:
                     return self._format_erro(403, f"{e}")
                 except MissingAuthorizationHeader as e:
                     return self._format_erro(401, f"{e}")
                 except Unauthorized as e:
                     return self._format_erro(401, f"{e}")
+                except InternalUnauthorized as e:
+                    return self._format_erro(500, f"{e}")
                 except Exception as e:
                     self._logger.exception(
                         f"Erro na autenticação/autorização. Mensagem: {e}")
                     return self._format_erro(500, f"{e}")
 
             return wrapper
```

### Comparing `nsj_flask_auth-0.5.0/nsj_flask_auth/settings.py` & `nsj_flask_auth-0.5.1/nsj_flask_auth/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_auth-0.5.0/pyproject.toml` & `nsj_flask_auth-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsj-flask-auth"
-version = "0.5.0"
+version = "0.5.1"
 description = "Modulo básico para autenticação de aplicações Flask no contexto da Nasajon"
 authors = ["Lucas Assis <lucasassis@nasajon.com.br>", "Sergio Silva <sergiosilva@nasajon.com.br>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Flask = "*"
 requests = "*"
```

### Comparing `nsj_flask_auth-0.5.0/PKG-INFO` & `nsj_flask_auth-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-flask-auth
-Version: 0.5.0
+Version: 0.5.1
 Summary: Modulo básico para autenticação de aplicações Flask no contexto da Nasajon
 Author: Lucas Assis
 Author-email: lucasassis@nasajon.com.br
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

